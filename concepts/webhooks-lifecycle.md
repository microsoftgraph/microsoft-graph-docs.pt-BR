---
title: Reduzir assinaturas ausentes e alterar notificações
description: Os aplicativos que estão se inscrevendo para alterar as notificações de recursos podem ter suas assinaturas removidas e perder algumas notificações de alteração. Os aplicativos devem implementar a lógica para detectar e recuperar da perda e retomar o fluxo de notificação de alteração contínua.
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: 2bbce70adc5de7b1b1f17cf63d679a6d116680fd
ms.sourcegitcommit: 709d2e3069765c2e570ac1128847c165ab233aa8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2022
ms.locfileid: "62184063"
---
# <a name="reduce-missing-subscriptions-and-change-notifications"></a>Reduzir assinaturas ausentes e alterar notificações

Os aplicativos que estão se inscrevendo para alterar as notificações de recursos podem ter suas assinaturas removidas e perder algumas notificações de alteração. Os aplicativos devem implementar a lógica para detectar e recuperar da perda e retomar o fluxo de notificação de alteração contínua.

Determinados eventos podem fazer que a assinatura seja removida. Esses eventos incluem:

- A senha do usuário foi redefinida
- Dispositivo do usuário está fora de conformidade
-   Conta do usuário foi revogada

Quando ocorre um evento, o Microsoft Graph envia uma notificação de ciclo de vida especial `subscriptionRemoved`.

O Microsoft Graph também envia outra notificação do ciclo de vida, `missed`, caso não seja possível entregar uma notificação de alteração a um aplicativo.

Uma assinatura de um aplicativo para modificar as notificações deve ouvir os sinais `subscriptionRemoved` e `missed` e fazer o seguinte:

- Após receber uma notificação de `subscriptionRemoved` ciclo de vida, o aplicativo deve recriar a assinatura para manter um fluxo contínuo.
- Ao receber uma notificação de `missed` ciclo de vida, o aplicativo deve ressincronizar os dados de recurso usando o Microsoft Graph.

Para receber notificações de ciclo de vida, você pode usar o ponto de extremidade existente **notificationUrl** que já recebe notificações de alteração, ou você pode registrar um **lifecycleNotificationUrl** separado para receber `subscriptionRemoved` e `missed` notificações de ciclo de vida em um ponto de extremidade separado.

As notificações de ciclo de vida têm suporte para as assinaturas criadas nesses tipos de recurso:

- [Mensagem][] do Outlook
- [Evento][] do Outlook
- [Contato][] pessoal do Outlook
- [chatMessage][] do Teams

Para outros tipos de recurso, você ainda poderá fornecer um `lifecycleNotificationUrl` ao criar a assinatura e o aplicativo receberá as notificações do ciclo de vida sempre que o recurso implementá-la.

## <a name="creating-a-subscription"></a>Criar uma assinatura

Ao criar uma assinatura, você deve especificar um ponto de extremidade de notificação separado usando a propriedade **lifecycleNotificationUrl**. Se você especificar o ponto de extremidade, todos os tipos de atuais e futuros de notificações de ciclo de vida serão entregues lá. Caso contrário, as notificações do ciclo de vida `subscriptionRemoved` e `missed` não serão entregues. Esse ponto de extremidade pode ser o mesmo que a **notificationUrl**.

### <a name="subscription-request-example"></a>Exemplo de solicitação de assinatura

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/users/{id}/messages",
  "expirationDateTime": "2020-03-20T11:00:00.0000000Z",
  "clientState": "<secretClientState>"
}
```
 
> [!IMPORTANT]
> Use o mesmo nome de host (FQDN) para ambas as notificações URLs. 

É necessário validar ambos os pontos de extremidade conforme descrito em [Gerenciar assinaturas](webhooks.md#managing-subscriptions). Se você quiser usar a mesma URL para os dois pontos de extremidade, você receberá e responderá a duas solicitações de validação.

> **Observação:** Não é possível atualizar (`PATCH`) as assinaturas existentes para adicionar a propriedade **lifecycleNotificationUrl**. Você deve remover essas assinaturas existentes, criar novas assinaturas e especificar a propriedade **lifecycleNotificationUrl**. As assinaturas existentes sem uma propriedade **lifecycleNotificationUrl** não receberão as `subscriptionRemoved` e `missed` notificações.

## <a name="responding-to-subscriptionremoved-notifications"></a>Responder a notificações subscriptionRemoved

A notificação de `subscriptionRemoved` ciclo de vida informa que uma assinatura foi removida e deve ser recriada, se você quiser continuar a receber as notificações de alteração. 

Você pode criar uma assinatura de longa duração (três dias) e as notificações de alteração começarão a fluir para o **notificationUrl**. No entanto, as condições de acesso aos dados de recursos podem mudar ao longo do tempo. Por exemplo, pode ocorrer um evento no serviço que exija que o aplicativo autentique novamente o usuário. Nesse caso, o fluxo é:

1. O serviço detecta que uma assinatura precisa ser removida do Microsoft Graph.
    
    Não há cadência definida para esses eventos. Eles podem ocorrer com frequência para alguns recursos e quase nunca para outros.

2. O Microsoft Graph envia uma notificação `subscriptionRemoved` de ciclo de vida para **lifecycleNotificationUrl** (se especificado).  

3. Você pode responder a essa notificação do ciclo de vida criando uma nova assinatura para o mesmo recurso. Para fazer isso, é necessário apresentar um token de acesso válido; em alguns casos, isso significa que o aplicativo precisa reautenticar o usuário para obter um novo token de acesso válido.

4. Se você criar uma nova assinatura com êxito, as notificações de alteração de recurso começarão a fluir novamente. No entanto, se houver falha (por exemplo, o aplicativo não pode obter um token de acesso válido), as notificações de alteração não serão enviadas.

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
- A notificação de ciclo de vida não contém informações sobre um recurso específico, porque ela não está relacionada a uma alteração de recurso, mas a alteração de estado da assinatura.
- Assim como notificações de alteração, notificações de ciclo de vida devem ser agrupadas (na matriz **valor**), cada com uma possivelmente valores diferentes **lifecycleEvent**. Processe cada notificação de ciclo de vida no lote adequadamente.

> **Observação:** para obter uma descrição completa dos dados enviados quando as notificações de alteração forem entregues, confira [changeNotificationCollection](/graph/api/resources/changenotificationcollection).

### <a name="actions-to-take"></a>Ações a serem executadas

1. [Confirme](webhooks.md#change-notifications) o recebimento da notificação do ciclo de vida respondendo à chamada do POST com `202 - Accepted`.
2. [Validar](webhooks.md#change-notifications) a autenticidade da notificação do ciclo de vida.
3. Certifique-se de que o aplicativo tenha um token de acesso válido para a próxima etapa. 
  > **Observação**: se você estiver usando uma das [bibliotecas de autenticação](/azure/active-directory/develop/reference-v2-libraries), elas farão isso para você ao reutilizar um token de cache válido ou obtendo um novo token, inclusive pedindo ao usuário para fazer logon novamente (com uma nova senha). Observe que a obtenção de um novo token pode falhar, pois as condições de acesso podem ser alteradas e o chamador não poderá mais acessar os dados de recursos. 

4. Criar uma nova assinatura usando o processo padrão descrito [aqui](webhooks.md#subscription-request-example).

  > **Observação:** essa ação pode falhar, porque as verificações de autorização realizadas pelo sistema podem recusar o aplicativo ou o acesso do usuário ao recurso. Pode ser necessário que o aplicativo obtenha um novo token de acesso do usuário para reautorizar uma assinatura com êxito. Você pode tentar essa ações mais tarde, a qualquer momento; por exemplo, quando as condições de acesso mudarem. Quaisquer alterações de recursos no período de quando a notificação de ciclo de vida foi enviada até quando o aplicativo recriou a assinatura com êxito, serão perdidas. O aplicativo precisará buscar essas alterações sozinho.

5. Depois de criar a nova assinatura, sincronizar todos os dados de recurso ausentes desde a última vez que você recebeu uma notificação para esse recurso, Por exemplo: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`

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
- A notificação de ciclo de vida não contém informações sobre um recurso específico, porque ela não está relacionada a uma alteração de recurso, mas a alteração de estado da assinatura.
- Assim como notificações de alteração, notificações de ciclo de vida podem ser agrupadas (na matriz **valor**), cada com uma possivelmente valores diferentes **lifecycleEvent**. Processe cada notificação de ciclo de vida no lote adequadamente.

> **Observação:** para obter uma descrição completa dos dados enviados quando as notificações de alteração forem entregues, confira [changeNotificationCollection](/graph/api/resources/changenotificationcollection).

### <a name="actions-to-take"></a>Ações a serem executadas

1. [Confirme](webhooks.md#change-notifications) o recebimento da notificação do ciclo de vida respondendo à chamada do POST com `202 - Accepted`.
    - Se você ignorar esses sinais, não faça mais nada. Caso contrário:
2. [Validar](webhooks.md#change-notifications) a autenticidade da notificação do ciclo de vida.
3. Executaremos ressincronização de dados completa para identificar as alterações que não foram entregues como notificações. 

## <a name="responding-to-reauthorizationrequired-notifications"></a>Respondendo a notificações reauthorizationRequired

Quando receber uma notificação `reauthorizationRequired` de ciclo de vida, você deve reautorizar a inscrição para manter o fluxo de dados.

Você pode criar uma assinatura de longa duração dependendo da [duração máxima da assinatura com suporte para o recurso](/graph/api/resources/subscription#maximum-length-of-subscription-per-resource-type), o que permite que as notificações de alteração fluam para o **notificationUrl**. Se as condições de acesso forem alteradas após a criação da assinatura ou o Microsoft Graph detectar que o fluxo de notificação pode ser interrompido em um futuro próximo, o Microsoft Graph poderá exigir que você reautorize a assinatura para provar que você ainda tem acesso aos dados do recurso. A seguir estão exemplos de condições que podem afetar o acesso aos dados:

- Um administrador de locatários pode revogar as permissões do seu aplicativo para ler um recurso.
- Em um cenário interativo, o usuário que fornece o token de autenticação ao seu aplicativo pode estar sujeito a políticas dinâmicas com base em vários fatores, como o local, o estado do dispositivo ou a avaliação de risco. Por exemplo, se o usuário alterar o seu local físico, pode ser que ele não tenha mais permissão para acessar os dados e seu aplicativo não conseguirá autorizar novamente a assinatura. Para saber mais sobre políticas dinâmicas que controlam o acesso, confira [Políticas de acesso condicional do Azure AD](/azure/active-directory/conditional-access/overview). 
- Seu token de acesso expira. Isso só se aplica a notificações que incluem dados de recursos.
- A assinatura expira antes de renová-la.

Antes que qualquer uma dessas condições se torne verdadeira, Microsoft Graph enviará um desafio de autorização para o **lifecycleNotificationUrl**. O intervalo dessas notificações é ilustrado abaixo:

```csharp
    //The following code is for illustrative purposes only
    var TokenTimeToExpirationInMinutes=(TokenExpirationTime-CurrentTime)/4;
    if((TokenTimeToExpirationInMinutes)<=180 && TokenTimeToExpirationInMinutes>60){
        //Microsoft Graph will send reauthorizationRequired notification
        TokenTimeToExpirationInMinutes=TokenTimeToExpirationInMinutes/2;
    }
    elseif(TokenTimeToExpirationInMinutes<60 && TokenTimeToExpirationInMinutes>=0){
            //Microsoft Graph will send reauthorizationRequired notification every 15 mins
            TokenTimeToExpirationInMinutes=TokenTimeToExpirationInMinutes-15;
    }else{
      //Microsoft Graph will stop sending reauthorizationRequired notifications
    }
```

As etapas a seguir representam o fluxo de um desafio de autorização para uma assinatura ativa:

1. O Microsoft Graph exige que uma assinatura seja autorizada novamente.
    
    Os motivos para isso podem variar de recurso para recurso e podem mudar com o tempo. Você deve responder a um evento de nova autorização, não importa o que o causou.

2. O Microsoft Graph envia uma notificação de desafio de autorização para **lifecycleNotificationUrl**.

    Observe que o fluxo de notificações de alterações pode continuar por um tempo, dando a você tempo extra para responder. No entanto, eventualmente a alteração na entrega de notificação fará uma pausa até você executar a ação necessária.

3. Responda a esta notificação do ciclo de vida de duas maneiras:
    - Autorizar a assinatura novamente. Isso não estende a data de validade da assinatura.
    - Renove a assinatura. Isso reautoriza e estende a data de validade.

    Observação: ambas as ações exigem que você apresente um token de autenticação válido, semelhante [criar uma nova assinatura](webhooks.md#creating-a-subscription) ou [renovar uma assinatura antes de sua expiração](webhooks.md#renewing-a-subscription).

4. Se você autorizar novamente ou renovar com êxito a inscrição, as notificações de alteração continuarão. Caso contrário, as notificações de alteração permanecerão pausadas. Observe que o Microsoft Graph descartará as notificações quatro horas depois que elas forem pausadas.

### <a name="reauthorizationrequired-notification-payload-example"></a>exemplo de conteúdo de notificação reauthorizationRequired

```json
{
  "value": [
    {
      "lifecycleEvent": "reauthorizationRequired",
      "subscriptionId": "e3898f08-5cd0-4a6a-80fc-6addbfb73b7b",
      "subscriptionExpirationDateTime": "2019-09-18T00:52:45.9696658+00:00",
      "clientState": "{secret client state}",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95"
    }
  ]
}
```

Alguns aspectos a serem observados neste tipo de notificação:

- O campo `"lifecycleEvent": "reauthorizationRequired"` identifica essa notificação como um desafio de autorização. `missed` e `subscriptionRemoved` notificações **lifecycleEvent** também são suportadas.
- A notificação de ciclo de vida não contém informações sobre um recurso específico, porque ela não está relacionada a uma alteração de recurso, mas a alteração de estado da assinatura.

> **Observação:** para obter uma descrição completa dos dados enviados quando as notificações de alteração forem entregues, confira [changeNotificationCollection](/graph/api/resources/changenotificationcollection).

### <a name="actions-to-take"></a>Ações a serem executadas

1. [Confirme](webhooks.md#change-notifications) o recebimento da notificação do ciclo de vida respondendo à chamada do POST com `202 - Accepted`.
2. [Validar](webhooks.md#change-notifications) a autenticidade da notificação do ciclo de vida.
3. Certifique-se de que o aplicativo tenha um token de acesso válido para a próxima etapa. 
  > **Observação**: se você estiver usando uma das [bibliotecas de autenticação](/azure/active-directory/develop/reference-v2-libraries), elas farão isso para você ao reutilizar um token de cache válido ou obtendo um novo token, inclusive pedindo ao usuário para fazer logon novamente (com uma nova senha). Observe que a obtenção de um novo token pode falhar, pois as condições de acesso podem ser alteradas e o chamador não poderá mais acessar os dados de recursos. 

4. Chamar uma das duas APIs a seguir. Se a chamada da API for bem-sucedida, o fluxo de notificação de mudança será retomado.

    - Chame a ação `/reauthorize` para autorizar novamente a assinatura sem estender a data de vencimento:
        ```http
        POST  https://graph.microsoft.com/beta/subscriptions/{id}/reauthorize
        Content-type: application/json
        ```
    - Execute uma ação de renovação regular para autorizar novamente e renovar a assinatura ao mesmo tempo:
        ```http
        PATCH https://graph.microsoft.com/beta/subscriptions/{id}
        Content-Type: application/json

        {
           "expirationDateTime": "2019-09-21T11:00:00.0000000Z"
        }
        ```

      A renovação pode falhar, porque as verificações de autorização realizadas pelo sistema podem recusar o aplicativo ou o acesso do usuário ao recurso. Pode ser necessário que o aplicativo obtenha um novo token de acesso do usuário para reautorizar com êxito uma assinatura. 
      
      Você pode tentar essa ações mais tarde, a qualquer momento e obter êxito se as condições de acesso mudarem. As notificações sobre as alterações de recursos que acontecem entre o tempo de envio da notificação do ciclo de vida e o momento em que o aplicativo cria a assinatura novamente, seriam perdidas. Nesses casos, o aplicativo deve buscar essas mudanças separadamente.

### <a name="additional-information"></a>Informações adicionais

As informações a seguir podem ajudá-lo a entender os desafios de autorização:

- Os desafios de autorização não substituem a necessidade de renova uma assinatura de alteração de recursos antes de expirar. 

    Embora você possa optar por renovar uma assinatura quando recebe um desafio de autorização, o Microsoft Graph pode não desafiar todas as suas assinaturas. Por exemplo, uma assinatura que não possui nenhuma atividade e não possui notificações de alterações com entrega pendente pode não sinalizar nenhum desafio para uma nova autorização do seu aplicativo. Certifique-se de [renovar assinaturas](webhooks.md#renewing-a-subscription) antes de expirarem.

- A frequência dos desafios de autorização está sujeita a mudanças.

    Não faça suposições sobre a frequência dos desafios de autorização. Essas notificações do ciclo de vida informam quando você deve executar as ações, evitando que você precise rastrear quais assinaturas requerem uma nova autorização. Esteja pronto para lidar com os desafios de autorização de vez em quando, para todas as assinaturas até raramente para apenas algumas das suas assinaturas.

## <a name="future-proof-the-code-handling-lifecycle-notifications"></a>À prova de futuro o código lidar com as notificações de ciclo de vida

No futuro, o Microsoft Graph adicionará mais tipos de notificações de ciclo de vida da assinatura. Elas serão publicadas no mesmo ponto de extremidade: **lifecycleNotificationUrl**, mas terão um valor diferente sob **lifecycleEvent** e podem conter um esquema e propriedades ligeiramente diferentes, específicas para o cenário para o qual serão enviadas.

Você deve implementar seu código de forma à prova de futuro, para que ele não seja interrompido quando Microsoft Graph novos tipos de notificações de ciclo de vida. Recomendamos a seguinte abordagem:

1. Identifique explicitamente cada notificação do ciclo de vida como um evento que você oferece suporte, usando a propriedade **lifecycleEvent**. Por exemplo, procure a `"lifecycleEvent": "subscriptionRemoved"` propriedade para identificar um evento específico e tratá-lo.

2. Fique atento aos anúncios de notificações de ciclo de vida para novos cenários. Pode haver mais tipos de notificações de ciclo de vida no futuro.

3. Em seu aplicativo ignore todos os eventos de ciclo de vida que o aplicativo não reconhece e registre-os para obter conhecimento.

4. Se desejar, procure a documentação relacionada às novas notificações de ciclo de vida e implemente o suporte para elas conforme necessário.

## <a name="see-also"></a>Confira também

- [Tipo de recurso de assinatura](/graph/api/resources/subscription)
- [Obter assinatura](/graph/api/subscription-get)
- [Criar assinatura](/graph/api/subscription-post-subscriptions)
- [Excluir assinatura](/graph/api/subscription-delete)
- [Atualizar assinatura](/graph/api/subscription-update)


[contato]: /graph/api/resources/contact
[event]: /graph/api/resources/event
[message]: /graph/api/resources/message
[chatMessage]: /graph/api/resources/chatmessage
