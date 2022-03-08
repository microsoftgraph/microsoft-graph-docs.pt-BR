---
title: Alterar notificações para recursos do Outlook no Microsoft Graph
description: Saiba como obter notificações de alterações (criar, atualizar e excluir) para recursos no Outlook usando as APIs do Microsoft Graph
author: abheek-das
ms.localizationpriority: high
ms.prod: outlook
ms.custom: scenarios:getting-started
ms.openlocfilehash: 04361ff86fc4106d0792b43b2ea7638a41e04b7c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337888"
---
# <a name="change-notifications-for-outlook-resources-in-microsoft-graph"></a>Alterar notificações para recursos do Outlook no Microsoft Graph

A API do Microsoft Graph permite que você assine alterações em um recurso, incluindo a criação, atualização ou exclusão do recurso, e receba notificações por meio de webhooks. Uma [assinatura](/graph/api/resources/webhooks) especifica os tipos desejados de alterações para monitorar um recurso específico e uma URL de um ponto de extremidade para receber notificações dessas alterações. Configurar uma assinatura reduz a sobrecarga de consultar e comparar recursos para deduzir quaisquer alterações. Opcionalmente, você pode especificar na solicitação de assinatura para criptografar e incluir como parte de uma notificação os dados do recurso que foram alterados, salvando uma chamada à API subsequente separada para obter o conteúdo do recurso.

Há um limite máximo de 1000 assinaturas ativas para recursos do Outlook por caixa de correio para todos os aplicativos. Você pode assinar alterações em contatos, eventos ou mensagens na caixa de correio.

## <a name="subscribe-to-changes-in-contacts-calendar-or-mail"></a>Assinar alterações em contatos, calendário ou email

Para assinar as notificações de alteração dos recursos do Outlook, primeiro crie uma [assinatura](/graph/api/resources/subscription).

Os recursos do Outlook a seguir dão suporte a assinaturas com ou sem dados de recurso no conteúdo [alterar notificação](/graph/api/resources/changenotification).

- [contato](/graph/api/resources/contact)
- [event](/graph/api/resources/event)
- [message](/graph/api/resources/message)

## <a name="create-a-subscription"></a>Criar uma assinatura

Para [criar uma assinatura](webhooks.md#creating-a-subscription), especifique o recurso do Outlook e o tipo de alterações (criação, atualização ou exclusão) para os quais você deseja receber notificações. Veja um [exemplo](#example-1-create-a-subscription-to-get-change-notifications-without-resource-data-when-the-user-receives-a-new-message).

### <a name="request-permissions"></a>Solicitar permissões

[!INCLUDE [outlook-subscription-notes](../includes/outlook-subscription-notes.md)]

Dependendo do recurso, a permissão especificada na tabela a seguir é a menos privilegiada necessária para chamar essa API.

| Resource| Trajetórias dos recursos com suporte| Delegado (conta corporativa ou de estudante)| Delegada (conta pessoal da Microsoft)| Aplicativo|
|:--------|:------------------------|:----------------------------------|:--------------------------------------|:-----------|
|[contato](/graph/api/resources/contact) | Alterações em todas as mensagens na caixa de correio de um usuário: <br>`/me/contacts`<br>`/users/{id}/contacts`<br>Alterações nos contatos no contactFolder de um usuário:<br>`/users/{id}/contactFolders/{id}/contacts` | Contacts.Read | Contacts.Read | Contacts.Read |
|[event](/graph/api/resources/event)     | Alterações em todas as mensagens na caixa de correio de um usuário: <br>`/me/events`<br>`/users/{id}/events` | Calendars.Read | Calendars.Read | Calendars.Read |
|[message](/graph/api/resources/message) | Alterações em todas as mensagens na caixa de correio de um usuário: <br>`/me/messages`<br>`/users/{id}/messages`<br>Alterações nas mensagens na mailFolder de um usuário:<br>`/users/{id}/mailFolders/{id}/messages` | Mail.ReadBasic, Mail.Read | Mail.ReadBasic, Mail.Read | Mail.ReadBasic, Mail.Read |

### <a name="include-resource-data-in-notification-payload-preview"></a>Incluir dados de recurso no conteúdo de notificação (versão prévia)

> [!NOTE]
> As notificações com dados de recursos para recursos do Outlook estão atualmente disponíveis apenas no ponto de extremidade do Microsoft Graph beta. 

Para incluir dados de recursos em uma notificação de alteração, você **deve** especificar as propriedades a seguir, além daquelas que você normalmente inclui ao [criar uma assinatura](webhooks.md#creating-a-subscription):

- **includeResourceData**: Defina essa propriedade como `true` para solicitar explicitamente os dados do recurso.
- **resource**: Essa propriedade especifica a URL do recurso. Certifique-se de usar o parâmetro de consulta `$select` para especificar as propriedades de recurso do Outlook a serem incluídas na carga de notificação.
  > **Observação:** Não inclua na URL `$top`, `$skip`, `$orderby`, `$select=Body,UniqueBody`e `$expand` diferentes de **singleValueExtendedProperties** ou **multiValueExtendedProperties**.
- **encryptionCertificate**: Essa propriedade contém apenas a chave pública que o Microsoft Graph usa para criptografar dados de recurso. Mantenha a chave privada correspondente para [descriptografar o conteúdo](webhooks-with-resource-data.md#decrypting-resource-data-from-change-notifications).
- **encryptionCertificateId**: Essa propriedade é seu próprio identificador para o certificado. Use esse ID para corresponder a cada notificação de alteração cujo certificado foi utilizado para descriptografia.

Consulte um [exemplo](#example-2-create-a-subscription-to-get-change-notifications-with-resource-data-when-the-user-receives-a-new-message-preview) para assinar a alteração de notificações com dados de recurso do recurso **mensagem**.


### <a name="refine-the-conditions-for-a-notification"></a>Refinar as condições para uma notificação
Você pode refinar ainda mais as condições de uma notificação usando o parâmetro de consulta `$filter`. Veja um [exemplo](#example-3-create-a-subscription-to-get-change-notifications-with-resource-data-for-a-message-based-on-a-condition-preview).

Uma aplicação comum de `$filter` é ser notificado após uma alteração em uma propriedade de recurso específica. Por exemplo, você pode usar `$filter` para assinar mensagens não lidas em uma pasta (a propriedade **isRead** é `false`) e inclui todos os tipos de alteração:
- Uma mensagem adicionada ou marcada como não lida na pasta dispararia uma notificação `Created`.
- Ler uma mensagem ou marcá-la como lida na pasta dispararia uma notificação `Deleted`.
- Uma alteração em qualquer propriedade, diferente de **isRead**, de um recurso **mensagem** na pasta dispararia uma notificação `Updated`.

Se você não usar um `$filter` ao criar a assinatura:
- Adicionar uma mensagem à pasta resultaria em uma notificação `Created`.
- Ler uma mensagem na pasta, marcar a mensagem como lida ou alterar qualquer outra propriedade de uma mensagem nessa pasta resultaria em uma notificação `Updated`.
- Excluir a mensagem resultaria em uma notificação `Delete`.

### <a name="subscribe-to-lifecycle-notifications"></a>Assinar notificações de ciclo de vida
Os recursos **contato**, **evento** e **mensagem** do Outlook também dão suporte à assinatura de notificações de ciclo de vida. As notificações de ciclo de vida são necessárias caso seu aplicativo tenha suas assinaturas removidas ou perca algumas notificações de alteração. Os aplicativos devem implementar a lógica para detectar e recuperar da perda e retomar o fluxo de notificação de alteração contínua. Para saber mais, consulte [assinatura de notificações de ciclo de vida](webhooks-lifecycle.md).

### <a name="keep-track-of-subscription-lifetime"></a>Acompanhar o tempo de vida da assinatura
Certifique-se de [estender](/graph/api/subscription-update) uma assinatura antes que ela expire. O tempo de vida máximo de uma assinatura sem dados de recursos do Outlook é de 4230 minutos (menos de 3 dias) e 1 dia com dados de recurso. 

Se você perder a permissão concedida anteriormente para uma assinatura e a assinatura expirar enquanto isso, solicite permissão novamente para [criar](/graph/api/subscription-post-subscriptions) uma nova assinatura.

## <a name="receive-notification-payloads"></a>Receber cargas de notificação

Dependendo da sua assinatura, as notificações podem incluir dados de recursos. As assinaturas com dados de recurso permitem que você obtenha o conteúdo do recurso junto com a notificação, evitando a sobrecarga de uma chamada à API separada para obter os dados de recursos alterados.

### <a name="receive-notifications-with-resource-data-preview"></a>Receber notificações com dados de recurso (versão prévia)

A seguir, um exemplo da carga de uma notificação com dados de recurso de um recurso **mensagem**. As propriedades **resource** e **resourceData** correspondem à instância **mensagem** que disparou a notificação. Use a propriedade **encryptedContent** para descriptografar os dados do recurso.

```json
{
    "value": [
      {
        "subscriptionId": "dfd11b2f-8222-4189-9545-4205c95d6235",
        "subscriptionExpirationDateTime": "2021-12-31T16:16:44.9907405+05:30",
        "changeType": "created",
        "resource": "Users('722effaf-0433-4272-9ac4-d5ec11c3cd77')/messages('AAMkAGUwNjQ4ZjIxLTQ3Y2Y8AAA=')",
        "clientState": "<<--SpecifiedClientState-->>",
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
        "encryptedContent": {
          "data": "<<--EncryptedContent-->>",
          "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",        
          "dataSignature": "Qw/9ubWeUYJPWWXvNiGgct2FkNG2MXTRm/BLUpJM66k=",
          "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
          "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "resourceData": {
          "@odata.type": "#microsoft.graph.message",
          "@odata.id": "Users('722effaf-0433-4272-9ac4-d5ec11c3cd77')/messages('AAMkAGUwNjQ4ZjIxLTQ3Y2Y8AAA=')",
          "@odata.etag": "W/\"CQAAABYAAACQ2fKdhq8oSKEDSVrdi3lRAAGDUR8n\"",
          "id": "AAMkAGUwNjQ4ZjIxLTQ3Y2Y8AAA="
        }
      }
    ]
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

Para obter detalhes sobre como validar tokens e descriptografar a carga útil, consulte [Definir notificações de alteração que incluem dados de recursos](webhooks-with-resource-data.md).

A seguir está um exemplo de uma carga de notificação descriptografada. A carga descriptografada está em conformidade com o esquema [message](/graph/api/resources/message?view=graph-rest-beta&preserve-view=true) do Outlook. A carga é semelhante à retornada por uma operação[GET](/graph/api/message-get?view=graph-rest-beta&preserve-view=true). No entanto, a carga de notificação contém apenas as propriedades especificadas com um parâmetro `$select` na propriedade **resource** da assinatura. Cargas de notificação de outros recursos do Outlook, como [contato](/graph/api/resources/contact?view=graph-rest-beta&preserve-view=true) e [eventos](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) seguem seus respectivos esquemas. 

```json
{
    "receivedDateTime@odata.type":"#DateTimeOffset",
    "receivedDateTime":"2021-12-30T10:53:35Z",
    "subject":"TEST MESSAGE FOR RICH NOTIFICATIONS",
    "bodyPreview":"Hello,\r\n\r\nWhat\u2019s up?\r\n\r\nThanks\r\nMegan",
    "importance@odata.type":"#microsoft.graph.importance",
    "importance":"normal",
    "from": {
        "@odata.type":"#microsoft.graph.recipient",
        "emailAddress": {
            "@odata.type":"#microsoft.graph.emailAddress",
            "name":"Megan Brown",
            "address":"Megan.Brown@microsoft.com"
        }
    }
}
```

### <a name="receive-notifications-without-resource-data"></a>Receber notificações sem dados de recurso

Notificações sem dados de recurso fornecem informações suficientes para fazer chamadas GET para obter o recurso. As assinaturas para notificações sem dados de recursos não exigem um certificado de criptografia, porque os dados reais dos recursos não são enviados.

O exemplo a seguir mostra a carga de uma notificação que corresponde a um recurso **mensagem** do Outlook. Ela inclui as propriedades **resource** e **resourceData**, que representam o recurso que disparou a notificação. Use as propriedades **resource** e **@odata.id** para fazer chamadas para o Microsoft Graph e obter o conteúdo do recurso.

> **Observe** As chamadas GET sempre retornarão o estado atual do recurso. Se o recurso for alterado entre o momento em que a notificação é enviada e a hora em que o recurso é recuperado, a operação retornará o estado do recurso na recuperação.


```json
"value": [
 {
   "subscriptionId": "c6126aa3-0ed8-412f-a988-71e6cee627c4",
   "subscriptionExpirationDateTime": "2022-01-02T03:12:18.2257768+05:30",
   "changeType": "created",    
   "resource": "Users/622eaaff-0683-4862-9de4-f2ec83c2bd98/Messages/AAMkAGUwNjQ4ZjIxAAA=",
   "resourceData": {      
     "@odata.type": "#Microsoft.Graph.Message",
     "@odata.id": "Users/622eaaff-0683-4862-9de4-f2ec83c2bd98/Messages/AAMkAGUwNjQ4ZjIAAA=",
     "@odata.etag": "W/\"CQAAABYAAACQ2fKdhq8oSKEDSVrdi3lRAAGDUUXn\"",
     "id": "AAMkAGUwNjQ4ZjIxAAA="
   },
   "clientState": "<<--SpecifiedClientState-->>",
   "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
 }
]
```


## <a name="examples"></a>Exemplos

### <a name="example-1-create-a-subscription-to-get-change-notifications-without-resource-data-when-the-user-receives-a-new-message"></a>Exemplo 1: Criar uma assinatura para receber notificações de alteração sem dados de recurso quando o usuário receber uma nova mensagem
O exemplo a seguir solicita uma notificação para uma mensagem que está sendo criada na caixa de correio do usuário.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "create_subscription_withoutresourcedata_for_message_resource"
}-->

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-type: application/json

{
    "changeType": "created",
    "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    "resource": "users/622eaaff-0683-4862-9de4-f2ec83c2bd98/messages",
    "expirationDateTime": "2021-07-07T21:42:18.2257768+00:00",
    "clientState": "secretClientState"
}
```

#### <a name="response"></a>Resposta
Este é um exemplo de resposta. 
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
    "id": "5522bd62-7c96-4530-85b0-00b916f6151a",
    "resource": "users/622eaaff-0683-4862-9de4-f2ec83c2bd98/messages",
    "applicationId": "507c3b9a-67b8-463d-88a2-15a8cefb2111",
    "changeType": "created",
    "clientState": "secretClientState",
    "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    "notificationQueryOptions": null,
    "notificationContentType": null,
    "lifecycleNotificationUrl": null,
    "expirationDateTime": "2022-01-01T21:42:18.2257768Z",
    "creatorId": "a4c7bd34-4f3b-46b7-a25d-b63c1e2a2842",
    "includeResourceData": null,
    "latestSupportedTlsVersion": "v1_2",
    "encryptionCertificate": null,
    "encryptionCertificateId": null,
    "notificationUrlAppId": null
}
```

### <a name="example-2-create-a-subscription-to-get-change-notifications-with-resource-data-when-the-user-receives-a-new-message-preview"></a>Exemplo 2: Criar uma assinatura para receber notificações de alteração com dados de recurso quando o usuário receber uma nova mensagem (versão prévia)
O exemplo a seguir assina notificações com dados de recurso para uma mensagem que está sendo criada na caixa de correio do usuário. As propriedades do recurso **message** a ser incluído na carga de notificação são especificadas usando o parâmetro de consulta `$select`.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "create_subscription_withresourcedata_for_message_resource"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{ 
    "changeType": "created",
    "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    "resource": "users/622eaaff-0683-4862-9de4-f2ec83c2bd98/messages?$select=Subject,bodyPreview,importance,receivedDateTime,from",
    "expirationDateTime": "2022-01-01T21:42:18.2257768+00:00",
    "clientState": "secretClientValue",
    "includeResourceData": true,
    "encryptionCertificate": "MIIDMzCCAhugAwIBAgIQE7D+++Dk1hKQBqWA==",
    "encryptionCertificateId": "testCertificateId"
}
```

#### <a name="response"></a>Resposta
Este é um exemplo de resposta. 
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
    "id": "178eec5f-cf3c-4e7e-8a9c-8640deb5b5c5",
    "resource": "users/622eaaff-0683-4862-9de4-f2ec83c2bd98/messages?$select=Subject,bodyPreview,importance,receivedDateTime,from",
    "applicationId": "507c3b9a-67b8-463d-88a2-15a8cefb2111",
    "changeType": "created",
    "clientState": "secretClientValue",
    "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    "notificationQueryOptions": null,
    "notificationContentType": null,
    "lifecycleNotificationUrl": null,
    "expirationDateTime": "2022-01-01T12:32:35.1582696Z",
    "creatorId": "a4c7bd34-4f3b-46b7-a25d-b63c1e2a2842",
    "includeResourceData": true,
    "latestSupportedTlsVersion": "v1_2",
    "encryptionCertificate": "MIIDMzCCAhugAwIBAgIQE7D+++Dk1hKQBqWA==",
    "encryptionCertificateId": "testCertificateId",
    "notificationUrlAppId": null
}
```

### <a name="example-3-create-a-subscription-to-get-change-notifications-with-resource-data-for-a-message-based-on-a-condition-preview"></a>Exemplo 3: Criar uma assinatura para obter notificações de alteração com dados de recurso para uma mensagem com base em uma condição (versão prévia)
O exemplo a seguir assina notificações com dados de recurso para uma mensagem que está sendo criada na pasta Rascunhos, contendo um ou mais anexos e de alta importância.

#### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "create_subscription_withresourcedata_for_message_resource_basedonfilter"
}-->

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-type: application/json

{ 
    "changeType": "created",
    "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    "resource": "me/mailfolders('Drafts')/messages?$select=Subject,bodyPreview&$filter=hasAttachments eq true AND importance eq 'High'",
    "expirationDateTime": "2022-01-01T21:42:18.2257768+00:00",
    "clientState": "secretClientValue",
    "includeResourceData": true,
    "encryptionCertificate": "MIIDMzCCAhugAwIBAgIQE7D+++Dk1hKQBqWA==",
    "encryptionCertificateId": "testCertificateId"
}
```

#### <a name="response"></a>Resposta
Este é um exemplo de resposta. 
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions/$entity",
    "id": "239dbc5f-cf3c-4e7e-8c9c-3340abc5b5c5",
    "resource": "me/mailfolders('Drafts')/messages?$select=Subject,bodyPreview&$filter=hasAttachments eq true AND importance eq 'High'",
    "applicationId": "507c3b9a-67b8-463d-88a2-15a8cefb2111",
    "changeType": "created",
    "clientState": "secretClientValue",
    "notificationUrl": "https://webhook.azurewebsites.net/api/send/myNotifyClient",
    "notificationQueryOptions": null,
    "notificationContentType": null,
    "lifecycleNotificationUrl": null,
    "expirationDateTime": "2022-01-20T12:32:35.1582696Z",
    "creatorId": "a4c7bd34-4f3b-46b7-a25d-b63c1e2a2842",
    "includeResourceData": true,
    "latestSupportedTlsVersion": "v1_2",
    "encryptionCertificate": "MIIDMzCCAhugAwIBAgIQE7D+++Dk1hKQBqWA==",
    "encryptionCertificateId": "testCertificateId",
    "notificationUrlAppId": null
}
```

## <a name="see-also"></a>Confira também
- [Notificações de alteração do Microsoft Graph](webhooks.md)
- [Configurar notificações de alteração que incluam dados de recurso](webhooks-with-resource-data.md)
- [Visão geral da API de email do Outlook](outlook-mail-concept-overview.md)
- [visão geral da API de contatos do Outlook](outlook-contacts-concept-overview.md)
- [Visão geral da API do calendário do Outlook](outlook-calendar-concept-overview.md)
