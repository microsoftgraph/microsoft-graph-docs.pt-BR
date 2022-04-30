---
title: Obter notificações de alteração para mensagens nos canais e bate-papos do Teams usando o Microsoft Graph
description: As notificações de alterações te habilitam a ouvir as alterações nas mensagens no canal ou no chat
author: RamjotSingh
ms.localizationpriority: high
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: c9bd130ce01738ae03cb0521b85774e974240055
ms.sourcegitcommit: dae41f5828677b993ba89f38c1d1c42d91c0ba02
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/29/2022
ms.locfileid: "65133325"
---
# <a name="get-change-notifications-for-messages-in-teams-channels-and-chats-using-microsoft-graph"></a>Obter notificações de alteração para mensagens nos canais e bate-papos do Teams usando o Microsoft Graph

As notificações de alteração habilitam você a inscrever-se para receber alterações (criar, atualizar e excluir) de mensagens em um canal ou chat. As notificações da alteração fornecem um modelo de baixa latência, permitindo que você mantenha uma assinatura. Você também pode obter os dados do recurso nas notificações e, portanto, evitar chamar a API para obter a carga útil.

## <a name="subscribe-to-changes-at-the-tenant-level"></a>Assinar para receber alterações no nível do locatário

Para acompanhar todas as alterações relacionadas a mensagens em um locatário, você pode usar assinaturas em um nível de locatário para mensagens de canal e chat. Isso requer que você crie duas assinaturas: uma para acompanhar todas as mensagens nos [canais](/graph/api/resources/channel?preserve-view=true) e outra para acompanhar todas as mensagens nos [chats](/graph/api/resources/chat?preserve-view=true).

### <a name="subscribe-to-messages-across-all-channels"></a>Assine para receber mensagens em todos os canais

Para obter notificações de alteração para todas as mensagens e respostas nos canais de um locatário, inscreva-se em `/teams/getAllMessages`. Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.

[!INCLUDE [teams-model-A-and-B-disclaimer](../includes/teams-model-A-and-B-disclaimer.md)]

#### <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              | Versões com suporte |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte. | Sem suporte. |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    | Sem suporte. |
|Aplicativo | ChannelMessage.Read.All | beta, v1.0 |

#### <a name="example"></a>Exemplo

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/getAllMessages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="subscribe-to-messages-across-all-chats"></a>Assine para receber mensagens em chats

Para obter notificações de alteração para todas as mensagens em chats em um locatário, assine em `/chats/getAllMessages`. Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.

[!INCLUDE [teams-model-A-and-B-disclaimer](../includes/teams-model-A-and-B-disclaimer.md)]

#### <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              | Versões com suporte |
|:--------------------|:---------------------------------------------------------|:-------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte. | Sem suporte. |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    | Sem suporte. |
|Aplicativo | Chat.Read.All | beta, v1.0 |

#### <a name="example"></a>Exemplo

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated,deleted",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/getAllMessages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-messages-in-a-channel"></a>Assine em mensagens em um canal

Para acompanhar mensagens e respostas em um canal, você pode criar uma assinatura de notificação de alteraração no nível do canal. Para fazer isso, assine em `/teams/{team-id}/channels/{channel-id}/messages`. Esse recurso oferece suporte à [inclusão de dados de recursos](webhooks-with-resource-data.md) na notificação no modo *delegado* e *somente no aplicativo*.

As assinaturas no nível do canal também oferecem suporte à pesquisa baseada em palavras-chave por meio do parâmetro de consulta `$search`.

### <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |Com suporte na versão |
|:--------------------|:---------------------------------------------------------|:--------------------|
|Delegado (conta corporativa ou de estudante) | ChannelMessage.Read.All | beta, v1.0 |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    | Sem suporte. |
|Aplicativo | ChannelMessage.Read.Group*, ChannelMessage.Read.All  | beta, v1.0 |

>**Nota:** As permissões marcadas com * são suportadas como parte do [consentimento específico do recurso](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

### <a name="example-1-subscribe-to-all-messages-and-replies-in-a-channel"></a>Exemplo 1: assinar em todas as mensagens (e respostas) em um canal

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}/channels/{channel-id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-2-subscribe-to-messages-and-replies-in-a-channel-that-contain-certain-text"></a>Exemplo 2: assinar para receber mensagens (e respostas) em um canal que contém determinado texto

A solicitação a seguir enviará mensagens que contêm `Hello` ao banco de dados do assinante.

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}/channels/{channel-id}/messages?$search=Hello",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-3-subscribe-to-messages-and-replies-in-a-channel-without-resource-data"></a>Exemplo 3: assinar para receber mensagens (e respostas) em um canal sem dados de recursos

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}/channels/{channel-id}/messages",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-4-subscribe-to-messages-and-replies-in-a-channel-that-mention-a-specific-user"></a>Exemplo 4: assinar para receber mensagens (e respostas) em um canal que menciona um usuário específico

Para obter notificações somente para mensagens em que um usuário específico foi mencionado, você pode especificar a ID do usuário (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` nesse exemplo) na consulta.

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{team-id}/channels/{channel-id}/messages?$filter=mentions/any(u: u/mentioned/user/id eq '9a6eb4d1-826b-48b1-9627-b50836c8fee9')",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-messages-in-a-chat"></a>Assinar para receber mensagens em um chat

Para acompanhar mensagens em um chat, você pode criar uma assinatura de notificação de alteração em um nível de chat. Para fazer isso, assine em `/chats/{chat-id}/messages`. Esse recurso oferece suporte à [inclusão de dados de recursos](webhooks-with-resource-data.md) na notificação no modo *delegado* e *somente no aplicativo*.

As assinaturas no nível do chat também oferecem suporte à pesquisa baseada em palavras-chave por meio do parâmetro de consulta `$search`.

> **Observação:** a assinatura para receber mensagens em um chat atualmente está em pré-visualização.

### <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              | Com suporte na versão |
|:--------------------|:---------------------------------------------------------|:---------------------|
|Delegada (conta corporativa ou de estudante) | Chat.Read | beta, v1.0 |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    | Sem suporte. |
|Aplicativo | ChatMessage.Read.Chat*, Chat.Read.All | beta, v1.0 |

>**Nota:** As permissões marcadas com * são suportadas como parte do [consentimento específico do recurso](/microsoftteams/platform/graph-api/rsc/resource-specific-consent) apenas para a versão beta atualmente.

### <a name="example-1-subscribe-to-messages-in-a-chat"></a>Exemplo 1: assinar para receber mensagens em um chat

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{chat-id}/messages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-2-subscribe-to-messages-in-a-chat-that-contain-certain-text"></a>Exemplo 2: assinar para receber mensagens em um chat que contenham determinado texto

A solicitação a seguir enviará mensagens que contêm `Hello` ao banco de dados do assinante.

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{chat-id}/messages?$search=Hello",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-3-subscribe-to-messages-and-replies-in-a-chat-without-resource-data"></a>Exemplo 3: assinar para receber mensagens (e respostas) em um chat sem dados de recursos

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{chat-id}/messages",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

### <a name="example-4-subscribe-to-message-in-a-chat-in-which-a-specific-user-is-mentioned"></a>Exemplo 4: assinar para receber mensagem em um chat no qual um usuário específico for mencionado

Para obter notificações somente para mensagens em que um usuário específico foi mencionado, você pode especificar a ID do usuário (`9a6eb4d1-826b-48b1-9627-b50836c8fee9` nesse exemplo) na consulta.

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{chat-id}/messages?$filter=mentions/any(u: u/mentioned/user/id eq '9a6eb4d1-826b-48b1-9627-b50836c8fee9')",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-changes-at-the-user-level"></a>Assinar para receber alterações no nível do usuário

Para rastrear mensagens em todos os chats de que um determinado usuário faz parte, você pode criar uma assinatura de notificação de alteração no nível do usuário. Para fazer isso, assine o `/users/{user-id}/chats/getAllMessages`. Esse recurso dá suporte [à inclusão de dados de recursos](webhooks-with-resource-data.md) na notificação nos modos *delegado* e *somente aplicativo*.

As assinaturas de mensagens de chat no nível do usuário também suportam a pesquisa baseada em palavra-chave por meio do parâmetro de consulta `$search`.

> **Observação:** no futuro, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados acessados por meio da API.

### <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              | Com suporte na versão |
|:--------------------|:---------------------------------------------------------|:---------------------|
|Delegado (conta corporativa ou de estudante) | Chat.Read, Chat.ReadWrite | beta |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    | Sem suporte. |
|Aplicativo | Chat.Read.All, Chat.ReadWrite.All | beta |

### <a name="example-subscribe-to-messages-across-all-chats-a-particular-user-is-part-of"></a>Exemplo: assine para receber mensagens em todos os chats de que um usuário específico faz parte

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated,deleted",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/users/{user-id}/chats/getAllMessages",
  "includeResourceData": true,
  "encryptionCertificate": "{base64encodedCertificate}",
  "encryptionCertificateId": "{customId}",
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```
## <a name="notification-payloads"></a>Notificação de conteúdo

Dependendo da sua assinatura, você pode receber a notificação com dados de recursos ou sem ele. Assinar com dados de recursos permite que você receba a carga da mensagem junto com a notificação, removendo a necessidade de ligar de volta e obter o conteúdo.

### <a name="notifications-with-resource-data"></a>Notificações com dados de recursos

Para notificações com dados de recursos, a carga se parece com a seguinte. Este conteúdo é para uma mensagem enviada em um bate-papo.

```json
{
    "value": [{
        "subscriptionId": "10493aa0-4d29-4df5-bc0c-ef742cc6cd7f",
        "changeType": "created",
        "clientState": "<<--SpecifiedClientState-->>",
        "subscriptionExpirationDateTime": "2021-02-02T10:30:34.9097561-08:00",
        "resource": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')",
        "resourceData": {
            "id": "1612289765949",
            "@odata.type": "#Microsoft.Graph.chatMessage",
            "@odata.id": "chats('19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces')/messages('1612289765949')"
        },
        "encryptedContent": {
            "data": "<<--EncryptedContent-->",
            "dataKey": "<<--EnryptedDataKeyUsedForEncryptingContent-->>",
            "encryptionCertificateId": "<<--IdOfTheCertificateUsedForEncryptingDataKey-->>",
            "encryptionCertificateThumbprint": "<<--ThumbprintOfTheCertificateUsedForEncryptingDataKey-->>"
        },
        "tenantId": "<<--TenantForWhichNotificationWasSent-->>"
    }],
    "validationTokens": ["<<--ValidationTokens-->>"]
}
```

Para obter detalhes sobre como validar tokens e descriptografar a carga útil, consulte [Definir notificações de alteração que incluem dados de recursos](webhooks-with-resource-data.md).

A carga de notificação descriptografada parece com a seguinte. A carga está de acordo com o esquema [chatMessage](/graph/api/resources/chatMessage?preserve-view=true). A carga é semelhante à devolvida pelas operações GET.

```json
{
  "id": "1612289992105",
  "replyToId": null,
  "etag": "1612289992105",
  "messageType": "message",
  "createdDateTime": "2021-02-02T18:19:52Z",
  "lastModifiedDateTime": "2021-02-02T18:19:52.105Z",
  "lastEditedDateTime": null,
  "deletedDateTime": null,
  "subject": null,
  "summary": null,
  "chatId": "19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_97f62344-57dc-409c-88ad-c4af14158ff5@unq.gbl.spaces",
  "importance": "normal",
  "locale": "en-us",
  "webUrl": null,
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
      "displayName": "Ramjot Singh",
      "userIdentityType": "aadUser"
    },
    "conversation": null
  },
  "body": {
    "contentType": "text",
    "content": "test"
  },
  "channelIdentity": null,
  "attachments": [],
  "mentions": [],
  "policyViolation": null,
  "reactions": [],
  "replies": [],
  "hostedContents": []
}
```

### <a name="notifications-without-resource-data"></a>Notificações sem dados de recursos

Notificações sem dados de recursos dão informações suficientes para fazer chamadas GET para obter o conteúdo da mensagem. As assinaturas para notificações sem dados de recursos não exigem um certificado de criptografia (porque os dados reais dos recursos não são enviados).

A carga parece ser a seguinte. Este conteúdo é para uma mensagem enviada em um canal.

```json
 {
  "subscriptionId": "9f9d1ed0-c9cc-42e7-8d80-a7fc4b0cda3c",
  "changeType": "created",
  "tenantId": "<<--TenantForWhichNotificationWasSent-->>",
  "clientState": "<<--SpecifiedClientState-->>",
  "subscriptionExpirationDateTime": "2021-02-02T11:26:41.0537895-08:00",
  "resource": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')",
  "resourceData": {
    "id": "1612293113399",
    "@odata.type": "#Microsoft.Graph.chatMessage",
    "@odata.id": "teams('fbe2bf47-16c8-47cf-b4a5-4b9b187c508b')/channels('19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2')/messages('1612293113399')"
  }
}
```

As propriedades **recurso** e **@odata.id** podem ser usados para fazer chamadas para o Microsoft Graph para obter o conteúdo para a mensagem. As chamadas GET sempre retornarão o estado atual da mensagem. Se a mensagem for alterada entre quando a notificação for enviada e quando a mensagem for recuperada, a operação retornará a mensagem atualizada.

## <a name="see-also"></a>Confira também
- [Notificações de alteração do Microsoft Graph](webhooks.md)
- [Visão geral da API do Microsoft Teams](teams-concept-overview.md)
