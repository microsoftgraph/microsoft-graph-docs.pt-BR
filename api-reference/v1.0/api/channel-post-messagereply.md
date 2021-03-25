---
title: Responder a uma mensagem em um canal
description: Responder a uma mensagem existente em um canal.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0e56d43e84dc7ba2cc47fd30ac47e9cb2fdcc8ea
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202251"
---
# <a name="reply-to-a-message-in-a-channel"></a>Responder a uma mensagem em um canal

Namespace: microsoft.graph

Crie uma nova resposta a [um chatMessage](../resources/chatmessage.md) em um canal [especificado](../resources/channel.md).


## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | ChannelMessage.Send, Group.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Teamwork.Migrate.All |

> **Observação**: as permissões de aplicativo só *são* suportadas para [migração](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).
No futuro, a Microsoft pode exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados importados.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/messages/{message-id}/replies
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON de um [objeto message.](../resources/chatmessage.md) Somente a propriedade body é obrigatória, outras propriedades são opcionais.

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `201 Created` o código de resposta com a [mensagem](../resources/chatmessage.md) que foi criada.

## <a name="examples"></a>Exemplos

### <a name="example-1-create-a-new-reply-to-a-chatmessage"></a>Exemplo 1: Criar uma nova resposta para um chatMessage

#### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

<!-- {
  "blockType": "request",
  "name": "post_reply_message"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages/1590776551682/replies
Content-type: application/json

{
  "body": {
    "contentType": "html",
    "content": "Hello World"
  }
}
```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 160

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages('1590776551682')/replies/$entity",
    "id": "1591039710682",
    "replyToId": "1590776551682",
    "etag": "1591039710682",
    "messageType": "message",
    "createdDateTime": "2019-02-04T19:58:15.511Z",
    "lastModifiedDateTime": "2019-05-04T19:58:15.511Z",
    "lastEditedDateTime": null,
    "deleted": false,
    "subject": null,
    "summary": null,
    "importance": "normal",
    "locale": "en-us",
    "policyViolation": null,
    "from": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
            "displayName": "Joh Doe",
            "userIdentityType": "aadUser"
        }
    },
    "body": {
        "contentType": "html",
        "content": "Hello World"
    },
    "attachments": [],
    "mentions": [],
    "reactions": []
}
```

### <a name="example-2-import-messages"></a>Exemplo 2: Importar mensagens

> **Observação**: o escopo `Teamwork.Migrate.All` de permissão é necessário para este cenário.

#### <a name="request"></a>Solicitação

O exemplo a seguir mostra como importar mensagens back-in-time usando `createDateTime` as chaves e no corpo da `from` solicitação.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/messages/1590776551682/replies

{
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "from":{
      "user":{
         "id":"8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
         "displayName":"Joh Doe"
      }
   },
   "body":{
      "contentType":"html",
      "content":"Hello World"
   }
}

```

#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->
```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')/messages('1590776551682')/replies/$entity",
   "id":"1591039710682",
   "replyToId":"1590776551682",
   "etag":"1591039710682",
   "messageType":"message",
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "lastModifiedDateTime":null,
   "deleted":false,
   "subject":null,
   "summary":null,
   "importance":"normal",
   "locale":"en-us",
   "policyViolation":null,
   "from":{
      "application":null,
      "device":null,
      "conversation":null,
      "user":{
         "id":"8c0a1a67-50ce-4114-bb6c-da9c5dbcf6ca",
         "displayName":"Joh Doe",
         "userIdentityType":"aadUser"
      }
   },
   "body":{
      "contentType":"html",
      "content":"Hello World"
   },
   "attachments":[ ],
   "mentions":[ ],
   "reactions":[ ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create a reply message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
