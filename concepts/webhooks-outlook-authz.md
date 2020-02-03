---
title: Reduzir assinaturas ausentes e notificações de recursos do Outlook (visualização)
description: O Outlook pode suspender a entrega de notificações de alteração devido a eventos de segurança como a redefinição de senha do usuário. Eventos com ciclo de vida especial – `subscriptionRemoved` e `missed` -precisam ser tratados para garantir a entrega contínua de notificações.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: ad690749db14bdb8994e1bfe85b0b312029657a2
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2020
ms.locfileid: "41651775"
---
# <a name="reduce-missing-subscriptions-and-notifications-for-outlook-resources-preview"></a>Reduzir assinaturas ausentes e notificações de recursos do Outlook (visualização) 

Assinatura de aplicativos para notificações de recursos do Outlook podem ter suas assinaturas removidas e perder algumas notificações. Os aplicativos devem implementar a lógica para detectar e se recuperar da perda e retomar um fluxo de notificação contínuo.

Determinados eventos no Outlook podem fazer que a assinatura seja removida. Esses eventos incluem:

- A senha do usuário foi redefinida
- Dispositivo do usuário está fora de conformidade
-   Conta do usuário foi revogada

Quando ocorre um evento, o Outlook envia uma notificação especial de ciclo de vida, `subscriptionRemoved`.

O Outlook também envia outra notificação de ciclo de vida, `missed`, se não for possível entregar uma notificação em um aplicativo.

Uma assinatura de um aplicativo para notificações de recursos do Outlook, como **mensagem** e **evento**, deve ouvir os sinais `subscriptionRemoved` e `missed` e fazer o seguinte:

- Após receber uma `subscriptionRemoved` notificação, o aplicativo deve recriar a assinatura para manter um fluxo contínuo.
- Ao receber uma `missed` notificação, o aplicativo deve ressincronizar os dados de recursos usando o Microsoft Graph.

Para receber notificações de ciclo de vida, você pode usar o ponto de extremidade **notificationUrl** existente que já recebe notificações de recurso, ou registrar um **lifecycleNotificationUrl** separado para receber notificações `subscriptionRemoved` e `missed` em um ponto de extremidade separado.

## <a name="creating-a-subscription"></a>Criar uma assinatura

Ao criar uma assinatura, você pode especificar um ponto de extremidade de notificação separado usando a propriedade**lifecycleNotificationUrl**. Se você especificar o ponto de extremidade, todos os tipos de notificações de ciclo de vida atuais e futuros serão entregues lá. Caso contrário, as notificações `subscriptionRemoved` e `missed` serão entregues nas **notificationUrl** existentes para todas as assinaturas existentes.

> **Observação:** a propriedade **lifecycleNotificationUrl** só pode ser definida ou lida usando as APIs beta do Microsoft Graph. No entanto, as assinaturas criadas usando as APIs beta são armazenadas no mesmo ambiente de produção que as assinaturas criadas usando v1.0, para que você possa implementar o novo fluxo do Outlook, além de suas assinaturas, usando APIs v1.0.

> As assinaturas criadas por meio das APIs do v 1.0 receberão notificações do ciclo de vida. 

### <a name="subscription-request-example"></a>Exemplo de solicitação de assinatura

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/users/{id}/messages",
  "expirationDateTime": "2019-03-20T11:00:00.0000000Z",
  "clientState": "<secretClientState>"
}
```
 
> **Importante:** Use o mesmo nome de host para ambas as notificações URLs. 

> **Observação:** é preciso validar os dois pontos de extremidade da notificação, conforme descrito em [Gerenciar assinaturas](webhooks.md#managing-subscriptions).
Se você quiser usar a mesma URL para os dois pontos de extremidade você receberá e responderá a duas solicitações de validação.

> **Observação:** Não é possível atualizar (`PATCH`) as assinaturas existentes para adicionar a propriedade **lifecycleNotificationUrl**. Você deve remover essas assinaturas existentes, criar novas assinaturas e especificar a propriedade **lifecycleNotificationUrl**. Assinaturas existentes, sem a propriedade **lifecycleNotificationUrl** receberão a `subscriptionRemoved` e `missed` notificações pelas **notificationUrl**. 

## <a name="responding-to-subscriptionremoved-notifications"></a>Responder a notificações subscriptionRemoved

A `subscriptionRemoved` notificação informa que uma assinatura foi removida e deve ser recriada, se você quiser continuar a receber notificações. 

Você pode criar uma assinatura de longa duração (3 dias) e notificações de dados do recurso começarão a fluir para a **notificationUrl**. No entanto, as condições de acesso aos dados de recursos podem mudar ao longo do tempo. Por exemplo, pode ocorrer um evento no serviço do Outlook que requeira que o aplicativo para que o usuário seja autenticado novamente. Nesse caso, o fluxo é:

1. Outlook detecta que uma assinatura precisa ser removido do Microsoft Graph.
    
    Não há cadência definida para esses eventos. Eles podem ocorrer com frequência para alguns recursos e quase nunca para outros.

2. O Microsoft Graph envia uma `subscriptionRemoved` notificação para a **lifecycleNotificationUrl** (se especificado), ou uma **notificationUrl**.  

3. Você pode responder a essa notificação criando uma nova assinatura para o mesmo recurso. Para fazer isso, é necessário apresentar um token de acesso válido; em alguns casos, isso significa que o aplicativo precisa reautenticar o usuário para obter um novo token de acesso válido.

4. Se você criar uma nova assinatura com êxito, as notificações de recurso começarão a fluir novamente. No entanto, se você falhar (por exemplo, o aplicativo não pode obter um token de acesso válido), as notificações do recurso não serão enviadas.

5. Depois de criar uma nova assinatura, você pode sincronizar os dados de recursos para identificar alterações ausentes.

### <a name="subscriptionremoved-notification-example"></a>exemplo de notificação subscriptionRemoved

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2019-03-20T11:00:00.0000000Z",
      "tenantId": "<tenant_guid>",
      "clientState":"<secretClientState>",
      "lifecycleEvent": "subscriptionRemoved"
    }
  ]
}
```

Alguns aspectos a serem observados neste tipo de notificação:
- O `"lifecycleEvent": "subscriptionRemoved"` campo designa essa notificação como relacionada à remoção de assinatura. Outros tipos de notificações de ciclo de vida também são possíveis, e novos serão disponibilizados no futuro.
- A notificação não contém informações sobre um recurso específico, porque ela não está relacionada a uma alteração de recurso, mas a alteração de estado da assinatura.
- Assim como as notificações de recursos, as notificações de ciclo de vida podem estar em lote juntas (na matriz **valor**), cada uma com valores **lifecycleEvent** possivelmente diferentes. Processe cada notificação no lote de acordo.

### <a name="actions-to-take"></a>Ações a serem executadas

1. [Aceite](webhooks.md#notifications) o recebimento da notificação respondendo a chamada POSTAGEM com `202 - Accepted`.
2. [Validar](webhooks.md#notifications) a autenticidade da notificação.
3. Certifique-se de que o aplicativo tenha um token de acesso válido para a próxima etapa. 
  > **Observação**: se você estiver usando uma das [bibliotecas de autenticação](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), elas farão isso para você ao reutilizar um token de cache válido ou obtendo um novo token, inclusive pedindo ao usuário para fazer logon novamente (com uma nova senha). Observe que a obtenção de um novo token pode falhar, pois as condições de acesso podem ser alteradas e o chamador não poderá mais acessar os dados de recursos. 

4. Criar uma nova assinatura usando o processo padrão descrito [aqui](webhooks.md#subscription-request-example).

  > **Observação:** essa ação pode falhar, porque as verificações de autorização realizadas pelo sistema podem recusar o aplicativo ou o acesso do usuário ao recurso. Pode ser necessário que o aplicativo obtenha um novo token de acesso do usuário para reautorizar uma assinatura com êxito. Você pode tentar essa ações mais tarde, a qualquer momento; por exemplo, quando as condições de acesso mudarem. Quaisquer alterações de recursos no período de tempo quando a notificação de ciclo de vida foi enviada até quando o aplicativo recriou a assinatura com êxito, serão perdidas. O aplicativo precisará buscar essas alterações sozinho.

5. Depois de criar a nova assinatura, sincronizar todos os dados de recurso ausentes desde a última hora conhecida que você recebeu uma notificação para esse recurso, Por exemplo: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`

## <a name="responding-to-missed-notifications"></a>Responder notificações perdidas

Esses sinais informam que algumas notificações podem não ter sido entregues. Você deve ignorar ou lidar com esses sinais são.

### <a name="notification-example"></a>Exemplo de notificação

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2019-03-20T11:00:00.0000000Z",
      "tenantId": "<tenant_guid>",
      "clientState":"<secretClientState>",
      "lifecycleEvent": "missed"
    }
  ]
}
```

Alguns aspectos a serem observados neste tipo de notificação:
- O `"lifecycleEvent": "missed"` campo designa isso como um sinal de notificações perdidas. Outros tipos de notificações de ciclo de vida também são possíveis, e novos serão disponibilizados no futuro.
- A notificação não contém informações sobre um recurso específico, porque ela não está relacionada a uma alteração de recurso, mas a alteração de estado da assinatura.
- Semelhante às notificações de recursos, as notificações de ciclo de vida podem estar em lote juntas (na matriz **valor**), cada uma com valores **lifecycleEvent** possivelmente diferentes. Processe cada notificação no lote de acordo.

### <a name="actions-to-take"></a>Ações a serem executadas

1. [Aceite](webhooks.md#notifications) o recebimento da notificação respondendo a chamada POSTAGEM com `202 - Accepted`.
    - Caso você ignore estes sinais, não faça nada. Caso contrário:
2. [Validar](webhooks.md#notifications) a autenticidade da notificação.
3. Executaremos ressincronização de dados completa para identificar as alterações que não foram entregues como notificações. 


## <a name="future-proof-the-code-handling-life-cycle-notifications"></a>Proteja a longo prazo o tratamento de código das notificações do ciclo de vida

No futuro, o Microsoft Graph adicionará mais tipos de notificações de ciclo de vida da assinatura. Elas serão publicadas no mesmo ponto de extremidade: **lifecycleNotificationUrl**, mas terão um valor diferente sob **lifecycleEvent** e podem conter um esquema e propriedades ligeiramente diferentes, específicas para o cenário para o qual serão enviadas.

Você deve fortalecer seu código para que não pare quando o Microsoft Graph apresentar novos tipos de notificações de ciclo de vida. Recomendamos as seguintes abordagens:

1. Identificar explicitamente cada notificação como um evento suportado, usando a propriedade **lifecycleEvent**. Por exemplo, procure a `"lifecycleEvent": "subscriptionRemoved"` propriedade para identificar um evento específico e tratá-lo.

2. Assista aos comunicados de notificações para ver novos cenários. Pode haver mais tipos de notificações de ciclo de vida no futuro.

3. Em seu aplicativo, ignore todos os eventos de ciclo de vida que o aplicativo não reconhece e acesse-os para obter conhecimento.

4. Se desejar, procure a documentação relacionada às novas notificações de ciclo de vida e implemente o suporte para elas conforme necessário.

## <a name="see-also"></a>Confira também

- [Tipo de recurso de assinatura](/graph/api/resources/subscription?view=graph-rest-1.0)
- [Obter assinatura](/graph/api/subscription-get?view=graph-rest-1.0)
- [Criar assinatura](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [Excluir assinatura](/graph/api/subscription-delete?view=graph-rest-1.0)
- [Atualizar assinatura](/graph/api/subscription-update?view=graph-rest-1.0)
