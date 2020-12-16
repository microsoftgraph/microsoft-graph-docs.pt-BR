---
title: Obter notificações de alteração para mensagens nos canais e bate-papos do Teams usando o Microsoft Graph
description: As notificações de alterações te habilitam a ouvir as alterações nas mensagens no canal ou no chat
author: RamjotSingh
localization_priority: Priority
ms.prod: microsoft-teams
ms.custom: scenarios:getting-started
ms.openlocfilehash: 12d8bfd49ebc71b6cb82cccd9525a3706cd570fd
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690610"
---
# <a name="get-change-notifications-for-messages-in-teams-channels-and-chats-using-microsoft-graph"></a>Obter notificações de alteração para mensagens nos canais e bate-papos do Teams usando o Microsoft Graph

As notificações de alteração habilitam você a assinar para receber alterações (criar, atualizar e excluir) de [ mensagens ](/graph/api/resources/chatMessage?preserve-view=true) em um [ canal ](/graph/api/resources/channel?preserve-view=true) ou [chat](/graph/api/resources/chat?preserve-view=true). As notificações de alteração fornecem um modelo de baixa latência, permitindo que você mantenha uma [assinatura](/graph/api/resources/webhooks?preserve-view=true). Você também pode obter os dados do recurso nas notificações e, portanto, evitar chamar a API para obter o conteúdo.

>**Observação:** o tempo máximo que uma assinatura pode durar é 60 minutos; entretanto, as assinaturas podem ser renovadas até que o chamador tenha permissão para acessar o recurso.

## <a name="subscribe-to-changes-at-the-tenant-level"></a>Assinar para receber alterações no nível do locatário

Para acompanhar todas as alterações relacionadas a mensagens em um locatário, você pode usar assinaturas em um nível de locatário para mensagens de canal e chat. Isso requer que você crie duas assinaturas: uma para acompanhar todas as mensagens nos [canais](/graph/api/resources/channel?preserve-view=true) e outra para acompanhar todas as mensagens nos [chats](/graph/api/resources/chat?preserve-view=true).

### <a name="subscribe-to-messages-across-channels"></a>Assine para receber mensagens em todos os canais

Para obter notificações de alteração para todas as mensagens e respostas nos canais de um locatário, assine em `/teams/getAllMessages`. Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.

#### <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte. |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | ChannelMessage.Read.All |

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

### <a name="subscribe-to-messages-across-chats"></a>Assinar para receber mensagens em chats

Para obter notificações de alteração para todas as mensagens em chats em um locatário, assine em `/chats/getAllMessages`. Este recurso oferece suporte a [ incluindo dados de recursos ](webhooks-with-resource-data.md) na notificação.

#### <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Sem suporte. |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Chat.Read.All |

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

Para acompanhar mensagens e respostas em um canal, você pode criar uma assinatura de notificação de alteraração no nível do canal. Para fazer isso, assine em `/teams{id}/channels/{id}/messages`. Este recurso oferece suporte à [inclusão de dados de recursos](webhooks-with-resource-data.md) na notificação no *modo somente de aplicativo*.

As assinaturas no nível do canal também oferecem suporte à pesquisa baseada em palavras-chave por meio do parâmetro de consulta `$search`.

### <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | ChannelMessage.Read.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | ChannelMessage.Read.All, ChannelMessage.Read.Group* |

>**Observação:** ChannelMessage.Read.Group é suportado como parte do [consentimento específico do recurso](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

### <a name="example-1-subscribe-to-all-messages-and-replies-in-a-channel"></a>Exemplo 1: assinar em todas as mensagens (e respostas) em um canal

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/teams/{id}/channels/{id}/messages",
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
  "resource": "/teams/{id}/channels/{id}/messages?$search=Hello",
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
  "resource": "/teams/{id}/channels/{id}/messages",
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
  "resource": "/teams/{id}/channels/{id}/messages?$filter=mentions/any(u: u/mentioned/user/id eq '9a6eb4d1-826b-48b1-9627-b50836c8fee9')",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="subscribe-to-messages-in-a-chat"></a>Assinar para receber mensagens em um chat

Para acompanhar mensagens em um chat, você pode criar uma assinatura de notificação de alteração em um nível de chat. Para fazer isso, assine em `/chats{id}/messages`. Este recurso oferece suporte à [inclusão de dados de recursos](webhooks-with-resource-data.md) na notificação no *modo somente de aplicativo*.

As assinaturas no nível do chat também oferecem suporte à pesquisa baseada em palavras-chave por meio do parâmetro de consulta `$search`.

> **Observação:** assinar para receber mensagens em um chat que esteja atualmente em pré-visualização.

### <a name="permissions"></a>Permissões

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | Chat.Read |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Chat.Read.All |

### <a name="example-1-subscribe-to-messages-in-a-chat"></a>Exemplo 1: assinar para receber mensagens em um chat

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json

{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "resource": "/chats/{id}/messages",
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
  "resource": "/chats/{id}/messages?$search=Hello",
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
  "resource": "/chats/{id}/messages",
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
  "resource": "/chats/{id}/messages?$filter=mentions/any(u: u/mentioned/user/id eq '9a6eb4d1-826b-48b1-9627-b50836c8fee9')",
  "includeResourceData": false,
  "expirationDateTime": "2019-09-19T11:00:00.0000000Z",
  "clientState": "{secretClientState}"
}
```

## <a name="see-also"></a>Confira também
- [Notificações de alteração do Microsoft Graph](webhooks.md)
- [Visão geral da API do Microsoft Teams](teams-concept-overview.md)
