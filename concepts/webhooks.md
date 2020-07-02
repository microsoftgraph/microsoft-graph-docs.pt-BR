---
title: Configurar notificações para alterações nos dados de usuário
description: The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients. A client is a web service that configures its own URL to receive change notifications. Client apps use change notifications to update their state upon changes.
author: baywet
ms.prod: non-product-specific
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 7db6b2498d039a4f6474b530023a9f4c0e199119
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "44989776"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a>Configurar notificações para alterações nos dados de usuário

The Microsoft Graph API uses a webhook mechanism to deliver change notifications to clients. A client is a web service that configures its own URL to receive change notifications. Client apps use change notifications to update their state upon changes.

Depois que o Microsoft Graph aceita a solicitação de assinatura, ele envia notificações de alteração para a URL especificada na assinatura. O aplicativo então realiza ações de acordo com sua lógica comercial. Por exemplo, ele busca mais dados, atualiza o cache e as exibições, etc.


> [!VIDEO https://www.youtube-nocookie.com/embed/rC1bunenaq4]
 
> [!div class="nextstepaction"]
> [Tutorial: usar notificações de alteração e controlar alterações com o Microsoft Graph](/learn/modules/msgraph-changenotifications-trackchanges)

Por padrão, as notificações de alteração não contêm dados de recursos, exceto o `id`. Se o aplicativo exigir dados de recursos, ele poderá fazer chamadas para as APIs do Microsoft Graph para obter o recurso completo. Este artigo usa o recurso **User** como um exemplo para trabalhar com notificações de alteração.

Um aplicativo também pode se inscrever para alterar notificações que incluem dados de recursos, para evitar a necessidade de fazer chamadas de API adicionais para acessar os dados. Esses aplicativos precisarão implementar um código extra para lidar com os requisitos de tais notificações, especificamente: responder às notificações do ciclo de vida da assinatura, validar a autenticidade das notificações e descriptografar os dados do recurso. Mais tipos de recursos terão suporte para esse tipo de notificações no futuro. Para saber mais sobre como trabalhar com essas notificações, confira [Configurar notificações de alteração que incluem dados de recurso (visualização)](webhooks-with-resource-data.md).

## <a name="supported-resources"></a>Recursos com suporte

Usando a API do Microsoft Graph, um aplicativo pode se inscrever para alterações nos seguintes recursos:

- [Mensagem][] do Outlook
- [Evento][] do Outlook
- [Contato][] pessoal do Outlook
- [user][]
- [group][]
- [Conversa][] de grupo do Microsoft 365
- Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _qualquer pasta_ no OneDrive pessoal do usuário
- Conteúdo dentro da hierarquia do tipo de recurso [driveItem][] de _pasta raiz_ no OneDrive for Business
- [Alerta][] de segurança
- Teams [callRecord][]
- [chatMessage][] do Teams (visualização)

Você pode criar uma assinatura para uma pasta de específica do Outlook, como a Caixa de Entrada: `me/mailFolders('inbox')/messages`

Ou para um recurso de nível superior:,,,, `/me/messages` `/me/contacts` `/me/events` `users` `groups` ou`/communications/callRecords`

Ou para uma instância de recurso específica: `users/{id}`, `groups/{id}`, `groups/{id}/conversations`

Ou para alguma pasta no OneDrive pessoal de um usuário: `/drives/{id}/root`
`/drives/{id}/root/subfolder`

Ou para a pasta raiz de uma unidade do SharePoint/OneDrive for Business: `/drive/root`

Ou para um novo alerta da [API de Segurança](security-concept-overview.md): `/security/alerts?$filter=status eq 'newAlert'`, `/security/alerts?$filter=vendorInformation/provider eq 'ASC'`

### <a name="azure-ad-resource-limitations"></a>Limitações de recursos do Microsoft Azure AD

Determinadas limites se aplicam aos recursos baseados no Azure AD (usuários, grupos) e gerarão erros se forem excedidos:

> **Observação**: Esses limites não se aplicam aos recursos de serviços diferente do Azure AD. Por exemplo, um aplicativo pode criar muito mais assinaturas para `message` ou recursos `event` que são aceitos pelo serviço Exchange Online como parte do Microsoft Graph.

- Cotas máximas de assinaturas:

  - Por aplicativo (para todos os locatários combinados): 50.000 total de assinaturas
  - Por locatário (para todos os aplicativos combinados): 1000 total de assinaturas em todos os aplicativos
  - Combinação por aplicativo e locatário: 100 assinaturas no total

Quando qualquer limite for excedido, as tentativas de criar uma assinatura resultarão em uma [resposta de erro](errors.md)  -  `403 Forbidden` . A propriedade `message` explicará qual limite foi excedido.

- Não há suporte a locatários do Microsoft Azure AD B2C.

- A notificação Changfe para entidades de usuário não tem suporte para contas pessoais da Microsoft.

- Existe um [problema conhecido](known-issues.md#change-notifications) nas assinaturas de usuários e grupos.

### <a name="outlook-resource-limitations"></a>Limitações de recursos do Outlook

Ao se inscrever em recursos do Outlook, tais como **mensagens**, **eventos** ou **contatos**, se você decidir usar o *nome UPN* em um caminho de recurso, a solicitação de assinatura pode falhar caso o UPN contenha um apóstrofo. Considere usar IDs de usuário de GUID em vez de UPNs para evitar esse problema. Por exemplo, em vez de usar o caminho de recursos:

`/users/sh.o'neal@contoso.com/messages`

Use: 

`/users/{guid-user-id}/messages`

## <a name="subscription-lifetime"></a>Tempo de vida da assinatura

As assinaturas têm tempo de vida limitado. Os aplicativos precisam renovar suas assinaturas antes do tempo de expiração. Caso contrário, será preciso criar uma nova assinatura. Confira a lista de prazos máximos em [Prazo máximo de assinatura por tipo de recurso](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type).

Os aplicativos também podem cancelar a assinatura a qualquer momento para parar de receber notificações de alteração.

## <a name="managing-subscriptions"></a>Gerenciar assinaturas

Os clientes podem criar, renovar e excluir assinaturas.

### <a name="creating-a-subscription"></a>Criar uma assinatura

Creating a subscription is the first step to start receiving change notifications for a resource. The subscription process is as follows:

1. O cliente envia uma solicitação de assinatura (POST) para um recurso específico.

1. O Microsoft Graph verifica a solicitação.

    - Se a solicitação for válida, o Microsoft Graph enviará um token de validação para a URL de notificação.
    - Se a solicitação for inválida, o Microsoft Graph enviará uma resposta de erro com um código e detalhes.

1. O cliente envia o token de validação de volta para o Microsoft Graph.

1. O Microsoft Graph envia uma resposta de volta para o cliente.

O cliente deve armazenar a ID da assinatura para correlacionar notificações de alteração à assinatura.

#### <a name="subscription-request-example"></a>Exemplo de solicitação de assinatura

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/notificationClient",
  "resource": "/me/mailfolders('inbox')/messages",
  "expirationDateTime": "2016-03-20T11:00:00.0000000Z",
  "clientState": "SecretClientState"
}
```

As propriedades `changeType`, `notificationUrl`, `resource` e `expirationDateTime` são obrigatórias. Confira os valores e as definições de propriedade em [tipo de recurso de assinatura](/graph/api/resources/subscription?view=graph-rest-1.0).

A propriedade `resource` especifica o recurso que será monitorado para detectar alterações. Por exemplo, você pode criar uma assinatura para uma pasta de email específica: `me/mailFolders('inbox')/messages` ou em nome de um usuário, atribuído com uma autorização do administrador: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`.

Embora `clientState` não seja necessário, você deve incluí-lo para estar em conformidade com o processo de tratamento de notificação de alterações recomendado. A definição dessa propriedade permitirá que você confirme se as notificações de alteração recebidas são originadas do serviço do Microsoft Graph. Por esse motivo, o valor da propriedade deve continuar em segredo e deve ser conhecido somente por seu aplicativo e pelo serviço do Microsoft Graph.

Se tiver êxito, o Microsoft Graph retornará um código `201 Created` e um objeto [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) no corpo.

#### <a name="notification-endpoint-validation"></a>Validação de ponto de extremidade de notificação

O Microsoft Graph valida o ponto de extremidade de notificação fornecido na propriedade `notificationUrl` da solicitação de assinatura antes de criar a assinatura. O processo de validação ocorre da seguinte maneira:

1. O Microsoft Graph envia uma solicitação POST para a URL de notificação:

    ``` http
    Content-Type: text/plain; charset=utf-8
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > **Importante:** como `validationToken` é um parâmetro de consulta, ele deve ser decodificado corretamente pelo cliente, de acordo com as práticas de codificação HTTP. Se o cliente não decodificar o token e usar o valor codificado na próxima etapa (resposta), a validação falhará. Além disso, o cliente deve tratar o valor de token como opaco, pois o formato de token pode ser alterado no futuro, sem aviso prévio.

1. O cliente deve fornecer uma resposta com as seguintes características em até 10 segundos:

    - Um código de status 200 (OK).
    - O tipo de conteúdo deve ser `text/plain`.
    - O corpo deve incluir o token de validação fornecido pelo Microsoft Graph.

O cliente deve descartar o token de validação depois de o fornecer na resposta.

Além disso, você pode usar a [coleção do Microsoft Graph Postman](use-postman.md) para confirmar que o ponto de extremidade implementa a solicitação de validação. A solicitação de **Validação de Assinaturas** na pasta **Diversos** fornece testes de unidade que validam a resposta fornecida por seu ponto de extremidade.  

![resultados do teste de resposta de validação](images/change-notifications/validation-request-tests-results.png)

### <a name="renewing-a-subscription"></a>Renovar uma assinatura

O cliente pode renovar uma assinatura com uma data de expiração específica de até três dias desde a hora da solicitação. A propriedade `expirationDateTime` é obrigatória.

#### <a name="subscription-renewal-example"></a>Exemplo de renovação de assinatura

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

Se tiver êxito, o Microsoft Graph retornará um código `200 OK` e um objeto [subscription](/graph/api/resources/subscription?view=graph-rest-1.0) no corpo. O objeto subscription inclui o novo valor de `expirationDateTime`.

### <a name="deleting-a-subscription"></a>Excluindo uma assinatura

O cliente pode parar de receber notificações de alteração excluindo a assinatura usando sua ID.

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

Se tiver êxito, o Microsoft Graph retornará um código `204 No Content`.

## <a name="change-notifications"></a>Notificações de alteração

Com uma assinatura de cliente para alterações em um recurso, o Microsoft Graph envia uma `POST` solicitação para a URL de notificação sempre que o recurso é alterado. Ele envia notificações somente para alterações do tipo especificado na assinatura, por exemplo, `created` .

> **Observação:** Se um cliente tiver várias assinaturas que monitoram o mesmo recurso e usarem a mesma URL de notificação, o Microsoft Graph poderá enviar várias notificações de alteração que correspondam a diferentes assinaturas, cada uma mostrando a ID de assinatura correspondente. Não há garantia de que todas as notificações de alteração na `POST` solicitação pertencem a uma única assinatura.

### <a name="change-notification-example"></a>Exemplo de notificação de alteração

Esta seção mostra um exemplo de uma notificação para a criação de mensagens. Quando o usuário recebe um email, o Microsoft Graph envia uma notificação de alteração, conforme mostrado no exemplo a seguir.
Observe que a notificação está em uma coleção representada no `value` campo. Consulte [changeNotificationCollection](/graph/api/resources/changenotificationcollection) para obter detalhes da carga de notificação. 

Quando muitas alterações ocorrem, o Microsoft Graph pode enviar várias notificações que correspondem a diferentes assinaturas na mesma `POST` solicitação.

```json
{
  "value": [
    {
      "id": "lsgTZMr9KwAAA",
      "sequenceNumber": 10,
      "subscriptionId":"{subscription_guid}",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@{tenant_guid}/messages/{long_id_string}",
      "tenantId": "84bd8158-6d4d-4958-8b9f-9d6445542f95",
      "resourceData":
      {
        "@odata.type":"#Microsoft.Graph.Message",
        "@odata.id":"Users/{user_guid}@{tenant_guid}/Messages/{long_id_string}",
        "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
        "id":"{long_id_string}"
      }
    }
  ]
}
```

### <a name="processing-the-change-notification"></a>Processando a notificação de alteração

Seu processo deve processar todas as notificações de alteração recebidas. Veja a seguir as tarefas mínimas que seu aplicativo deve executar para processar uma notificação de alteração:

1. Envie um código de status `202 - Accepted` na sua resposta para o Microsoft Graph. Se o Microsoft Graph não receber um código de classe 2xx, ele tentará publicar a notificação de alteração diversas vezes, por um período de cerca de 4 horas; Após isso, a notificação de alteração será cancelada e não será entregue.

    > **Observação:** Envie um `202 - Accepted` código de status assim que receber a notificação de alteração, mesmo antes de validar sua autenticidade. Você está apenas confirmando o recebimento da notificação de alteração e evitando tentativas desnecessárias. O tempo limite atual é de 30 segundos, mas pode ser reduzido no futuro para otimizar o desempenho do serviço. Se a URL de notificação não responder dentro de 30 segundos para mais de 10% das solicitações do Microsoft Graph em um período de 10 minutos, todas as notificações a seguir serão atrasadas e repetidas por um período de 4 horas. Se uma URL de notificação não responder dentro de 30 segundos por mais de 20% das solicitações do Microsoft Graph em um período de 10 minutos, todas as notificações a seguir serão descartadas.

1. Validar a propriedade `clientState`. Ela deve corresponder ao valor enviado originalmente com a solicitação de criação da assinatura.

    > **Observação:** Se isso não for verdadeiro, você não deve considerar essa uma notificação de alteração válida. É possível que a notificação de alteração não tenha origem no Microsoft Graph e tenha sido enviada por um ator invasor. Você também deve investigar onde a notificação de alteração provém e tomar as medidas apropriadas.

1. Atualize seu aplicativo com base na sua lógica comercial.

Repita para outras notificações de alteração na solicitação.

## <a name="code-samples"></a>Exemplos de código

Os exemplos de código a seguir estão disponíveis no GitHub.

- [Módulo de Treinamento do Microsoft Graph - Usar notificações de alteração e controlar alterações com o Microsoft Graph](https://github.com/microsoftgraph/msgraph-training-changenotifications)
- [Exemplo de webhooks do Microsoft Graph para Node.js](https://github.com/microsoftgraph/nodejs-webhooks-rest-sample)
- [Exemplo de Webhooks do Microsoft Graph para o ASP.NET Core](https://github.com/microsoftgraph/aspnetcore-webhooks-sample)
- [Exemplo de Webhooks do Microsoft Graph para Java Spring](https://github.com/microsoftgraph/java-spring-webhooks-sample)

## <a name="firewall-configuration"></a>Configuração do firewall

Opcionalmente, você pode configurar o firewall que protege a URL de notificação para permitir conexões de entrada somente pelo Microsoft Graph. Isso permite que você reduza mais exposição a notificações de alteração inválidas que são enviadas para sua URL de notificação. Essas notificações de alteração inválidas podem estar tentando disparar a lógica personalizada que você implementou. Para obter uma lista completa de endereços IP usados pelo Microsoft Graph para fornecer notificações de alteração, consulte [pontos de extremidade adicionais para o microsoft 365](https://docs.microsoft.com/office365/enterprise/additional-office365-ip-addresses-and-urls).

> **Observação:** Os endereços IP listados que são usados para fornecer notificações de alteração podem ser atualizados a qualquer momento sem aviso prévio.

## <a name="see-also"></a>Confira também

- [Tipo de recurso de assinatura](/graph/api/resources/subscription?view=graph-rest-1.0)
- [Obter assinatura](/graph/api/subscription-get?view=graph-rest-1.0)
- [Criar assinatura](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- tipo de recurso [changeNotification](/graph/api/resources/changenotification?view=graph-rest-beta)
- tipo de recurso [changeNotificationCollection](/graph/api/resources/changenotificationcollection?view=graph-rest-beta)
- [Tutorial de controle de alterações e notificações de alteração](/learn/modules/msgraph-changenotifications-trackchanges)
- [Notificações do ciclo de vida (visualização)](/graph/concepts/webhooks-outlook-authz.md)

[contato]: /graph/api/resources/contact?view=graph-rest-1.0
[conversa]: /graph/api/resources/conversation?view=graph-rest-1.0
[driveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[event]: /graph/api/resources/event?view=graph-rest-1.0
[group]: /graph/api/resources/group?view=graph-rest-1.0
[message]: /graph/api/resources/message?view=graph-rest-1.0
[user]: /graph/api/resources/user?view=graph-rest-1.0
[alert]: /graph/api/resources/alert?view=graph-rest-1.0
[callRecord]: /graph/api/resources/callrecords-callrecord?view=graph-rest-1.0
[chatMessage]: /graph/api/resources/chatmessage
