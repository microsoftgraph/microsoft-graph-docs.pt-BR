---
title: Reduzir assinaturas ausentes e alterar as notificações de recursos do Outlook (versão prévia)
description: O Outlook pode suspender a entrega de notificações de alteração devido a eventos de segurança como a redefinição de senha do usuário. Eventos de ciclo de vida especiais – `subscriptionRemoved` e `missed` precisam ser tratados para garantir a entrega ininterrupta de notificações de alteração.
author: baywet
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 8b2174ea14dd7e3d6af7f0b4a447c4e5afa6fce1
ms.sourcegitcommit: 4fa554d92a684d7720db1bd96befb9dea8d6ba5f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/30/2020
ms.locfileid: "44429625"
---
# <a name="reduce-missing-subscriptions-and-change-notifications-for-outlook-resources-preview"></a>Reduzir assinaturas ausentes e alterar as notificações de recursos do Outlook (versão prévia) 

Os aplicativos que se inscrevem nas notificações de alteração dos recursos do Outlook podem receber suas assinaturas removidas e perder algumas notificações de alteração. Os aplicativos devem implementar a lógica para detectar e recuperar da perda e retomar o fluxo de notificação de alteração contínua.

Determinados eventos no Outlook podem fazer que a assinatura seja removida. Esses eventos incluem:

- A senha do usuário foi redefinida
- Dispositivo do usuário está fora de conformidade
-   Conta do usuário foi revogada

Quando ocorre um evento, o Outlook envia uma notificação de ciclo de vida especial `subscriptionRemoved`.

O Outlook também enviará outra notificação do ciclo de vida, `missed` caso uma notificação de alteração não possa ser entregue a um aplicativo.

Um aplicativo inscrever-se em notificações de alteração para recursos do Outlook, como **mensagem** e **evento**, deve escutar os `subscriptionRemoved` sinais e `missed` fazer o seguinte:

- Após receber uma `subscriptionRemoved` notificação de ciclo de vida, o aplicativo deve recriar a inscrição para manter um fluxo contínuo.
- Ao receber uma `missed` notificação de ciclo de vida, o aplicativo deve sincronizar novamente os dados de recursos usando o Microsoft Graph.

Para receber notificações do ciclo de vida, você pode usar o ponto de extremidade do **notificationUrl** existente que já recebe notificações de alteração ou pode registrar um **lifecycleNotificationUrl** separado para receber `subscriptionRemoved` e `missed` notificar as notificações de ciclo de vida em um ponto de extremidade separado.

## <a name="creating-a-subscription"></a>Criar uma assinatura

Ao criar uma assinatura, você pode especificar um ponto de extremidade separado usando a propriedade **lifecycleNotificationUrl** . Se você especificar o ponto de extremidade, todos os tipos de atuais e futuros de notificações de ciclo de vida serão entregues lá. Caso contrário, `subscriptionRemoved` e `missed` as notificações de ciclo de vida serão entregues ao **notificationUrl** existente para todas as assinaturas existentes.

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

> **Observação:** Você precisa validar os dois pontos de extremidade, conforme descrito em [Managing subscriptions](webhooks.md#managing-subscriptions).
Se você quiser usar a mesma URL para os dois pontos de extremidade você receberá e responderá a duas solicitações de validação.

> **Observação:** Não é possível atualizar (`PATCH`) as assinaturas existentes para adicionar a propriedade **lifecycleNotificationUrl**. Você deve remover essas assinaturas existentes, criar novas assinaturas e especificar a propriedade **lifecycleNotificationUrl**. As assinaturas existentes sem a propriedade **lifecycleNotificationUrl** receberão as `subscriptionRemoved` notificações de ciclo de `missed` vida e por meio do **notificationUrl**. 

## <a name="responding-to-subscriptionremoved-notifications"></a>Responder a notificações subscriptionRemoved

A `subscriptionRemoved` notificação de ciclo de vida informa que uma assinatura foi removida e deve ser recriada, se você quiser continuar recebendo notificações de alteração. 

Você pode criar uma assinatura de longa vida (3 dias) e as notificações de alteração começarão a fluir para o **notificationUrl**. No entanto, as condições de acesso aos dados de recursos podem mudar ao longo do tempo. Por exemplo, pode ocorrer um evento no serviço do Outlook que requeira que o aplicativo para que o usuário seja autenticado novamente. Nesse caso, o fluxo é:

1. Outlook detecta que uma assinatura precisa ser removido do Microsoft Graph.
    
    Não há cadência definida para esses eventos. Eles podem ocorrer com frequência para alguns recursos e quase nunca para outros.

2. O Microsoft Graph envia uma `subscriptionRemoved` notificação de ciclo de vida para o **lifecycleNotificationUrl** (se especificado) ou para o **notificationUrl**.  

3. Você pode responder a essa notificação de ciclo de vida criando uma nova assinatura para o mesmo recurso. Para fazer isso, é necessário apresentar um token de acesso válido; em alguns casos, isso significa que o aplicativo precisa reautenticar o usuário para obter um novo token de acesso válido.

4. Se você criar uma nova assinatura com êxito, as notificações de alteração começarão a fluir novamente. No entanto, se você falhar (por exemplo, o aplicativo não pode obter um token de acesso válido), as notificações de alteração não serão enviadas.

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
- A notificação de ciclo de vida não contém informações sobre um recurso específico, pois ela não está relacionada a uma alteração de recurso, mas à alteração de estado de assinatura.
- Semelhante às notificações de alteração, as notificações de ciclo de vida podem ser encadeados juntas (na matriz de **valor** ), cada uma com um valor possivelmente diferente de **lifecycleEvent** . Processe a cada notificação de ciclo de vida no lote.

> **Observação:** para obter uma descrição completa dos dados enviados quando as notificações de alteração são entregues, consulte [changeNotificationCollection](/graph/api/resources/changenotificationcollection).

### <a name="actions-to-take"></a>Ações a serem executadas

1. [Confirme](webhooks.md#change-notifications) o recebimento da notificação de ciclo de vida, respondendo à chamada post com `202 - Accepted` .
2. [Validar](webhooks.md#change-notifications) a autenticidade da notificação de ciclo de vida.
3. Certifique-se de que o aplicativo tenha um token de acesso válido para a próxima etapa. 
  > **Observação**: se você estiver usando uma das [bibliotecas de autenticação](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries), elas farão isso para você ao reutilizar um token de cache válido ou obtendo um novo token, inclusive pedindo ao usuário para fazer logon novamente (com uma nova senha). Observe que a obtenção de um novo token pode falhar, pois as condições de acesso podem ser alteradas e o chamador não poderá mais acessar os dados de recursos. 

4. Criar uma nova assinatura usando o processo padrão descrito [aqui](webhooks.md#subscription-request-example).

  > **Observação:** essa ação pode falhar, porque as verificações de autorização realizadas pelo sistema podem recusar o aplicativo ou o acesso do usuário ao recurso. Pode ser necessário que o aplicativo obtenha um novo token de acesso do usuário para reautorizar uma assinatura com êxito. Você pode tentar essa ações mais tarde, a qualquer momento; por exemplo, quando as condições de acesso mudarem. Qualquer alteração de recurso no período de tempo a partir da qual a notificação de ciclo de vida foi enviada, quando o aplicativo recriar a assinatura com êxito, será perdido. O aplicativo precisará buscar essas alterações sozinho.

5. Após criar a nova assinatura, sincronize quaisquer dados de recurso ausentes do último tempo conhecido em que você recebeu uma notificação de alteração para este recurso; por exemplo:`GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`

## <a name="responding-to-missed-notifications"></a>Responder notificações perdidas

Esses sinais informam que algumas notificações de alteração podem não ter sido entregues. Você deve ignorar ou lidar com esses sinais são.

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
- O `"lifecycleEvent": "missed"` campo designa isso como um sinal sobre notificações de alteração perdidas. Outros tipos de notificações de ciclo de vida também são possíveis, e novos serão disponibilizados no futuro.
- A notificação de ciclo de vida não contém informações sobre um recurso específico, pois ela não está relacionada a uma alteração de recurso, mas à alteração de estado de assinatura.
- Semelhante às notificações de alteração, as notificações de ciclo de vida podem ser encadeados juntas (na matriz de **valor** ), cada uma com um valor possivelmente diferente de **lifecycleEvent** . Processe a cada notificação de ciclo de vida no lote.

> **Observação:** para obter uma descrição completa dos dados enviados quando as notificações de alteração são entregues, consulte [changeNotificationCollection](/graph/api/resources/changenotificationcollection).

### <a name="actions-to-take"></a>Ações a serem executadas

1. [Confirme](webhooks.md#change-notifications) o recebimento da notificação de ciclo de vida, respondendo à chamada post com `202 - Accepted` .
    - Caso você ignore estes sinais, não faça nada. Caso contrário:
2. [Validar](webhooks.md#change-notifications) a autenticidade da notificação de ciclo de vida.
3. Executaremos ressincronização de dados completa para identificar as alterações que não foram entregues como notificações. 


## <a name="future-proof-the-code-handling-lifecycle-notifications"></a>À prova de futuro o código lidar com as notificações de ciclo de vida

No futuro, o Microsoft Graph adicionará mais tipos de notificações de ciclo de vida de assinatura. Elas serão publicadas no mesmo ponto de extremidade: **lifecycleNotificationUrl**, mas terão um valor diferente sob **lifecycleEvent** e podem conter um esquema e propriedades ligeiramente diferentes, específicas para o cenário para o qual serão enviadas.

Você deve implementar o código á prova de futuro para que não pare quando o Microsoft Graph apresentar novos tipos de notificações de ciclo de vida. Recomendamos as seguintes abordagens:

1. Identifique explicitamente cada notificação de ciclo de vida como um evento que você suporta, usando a propriedade **lifecycleEvent** . Por exemplo, procure a `"lifecycleEvent": "subscriptionRemoved"` propriedade para identificar um evento específico e tratá-lo.

2. Assista aos comunicados de notificações de ciclo de vida para o novo scenarions. Talvez haja mais tipos de notificações de ciclo de vida no futuro.

3. Em seu aplicativo, ignore qualquer notificação de ciclo de vida que o aplicativo não reconhece e registre-o para obter conscientização.

4. Se desejar, procure a documentação relacionada às novas notificações de ciclo de vida e implemente o suporte para elas conforme necessário.

## <a name="see-also"></a>Confira também

- [Tipo de recurso de assinatura](/graph/api/resources/subscription?view=graph-rest-1.0)
- [Obter assinatura](/graph/api/subscription-get?view=graph-rest-1.0)
- [Criar assinatura](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [Excluir assinatura](/graph/api/subscription-delete?view=graph-rest-1.0)
- [Atualizar assinatura](/graph/api/subscription-update?view=graph-rest-1.0)
