---
title: Criar chatMessage em um canal
description: Crie um novo chatMessage no canal especificado.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 791bf418a525d09c0386b29d2914319f03c7e90b
ms.sourcegitcommit: d02c438bcd58e8f64bfcd5fba0b40e436b46570e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/04/2021
ms.locfileid: "50101906"
---
# <a name="create-chatmessage-in-channel"></a>Criar chatMessage no canal

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [chatMessage](../resources/chatmessage.md) no canal [especificado.](../resources/channel.md)

> **Observação:** é uma violação dos termos [de uso usar](/legal/microsoft-apis/terms-of-use) o Microsoft Teams como um arquivo de log. Enviar apenas mensagens que as pessoas lerão.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | ChannelMessage.Send, Group.ReadWrite.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Teamwork.Migrate.All |

> **Observação:** As permissões de aplicativo só *são* suportadas para [migração.](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)

<!-- markdownlint-disable MD024 -->
<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD022 -->
<!-- markdownlint-disable MD025 -->

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/channels/{id}/messages
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | Portador {código}. Obrigatório. |
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON de um [objeto chatMessage.](../resources/chatmessage.md) Somente a propriedade body é obrigatória, outras propriedades são opcionais.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna `201 Created` um código de resposta e um novo objeto [chatMessage](../resources/chatmessage.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-create-a-message-in-a-specified-channel"></a>Exemplo 1: Criar uma mensagem em um canal especificado

Para obter uma lista mais abrangente de exemplos, consulte [Criar chatMessage em um canal ou chat.](chatmessage-post.md)

### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_channel"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
    "content": "Hello World"
  }
}
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-chatmessage-from-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-chatmessage-from-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-chatmessage-from-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-chatmessage-from-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('123456-1234-1234-1234-123456789123')/channels('19%123456789012345678901236%40thread.skype')/messages/$entity",
    "id": "id-value",
    "replyToId": null,
    "etag": "id-value",
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
            "id": "id-value",
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

### <a name="example-2-import-messages-text-only"></a>Exemplo 2: Importar mensagens (somente texto)

> **Observação:** o escopo `Teamwork.Migrate.All` de permissão é necessário para este cenário.

#### <a name="request"></a>Solicitação
<!-- { "blockType": "ignored" } -->
O exemplo a seguir mostra como importar mensagens de back-in-time usando as `createDateTime` chaves no corpo da `from` solicitação.

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/messages

{
   "replyToId":null,
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
         "id":"id-value",
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

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 200 OK

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams('teamId')/channels('channelId')/messages/$entity",
   "id":"id-value",
   "replyToId":null,
   "etag":"id-value",
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
         "id":"id-value",
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

### <a name="example-3-import-messages-with-inline-images"></a>Exemplo 3: Importar mensagens com imagens em linha

> [!NOTE]
> Atualmente, as imagens em linha são o único tipo de mídia suportado pelo esquema de API de mensagem de importação.

> **Observação:** o escopo `Teamwork.Migrate.All` de permissão é necessário para este cenário.

#### <a name="request"></a>Solicitação
<!-- { "blockType": "ignored" } -->
O exemplo a seguir mostra como importar mensagens de back-in-time contendo imagens em linha usando as teclas e o `createDateTime` `from` corpo da solicitação.

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/messages

{
   "createdDateTime":"2019-02-04T19:58:15.511Z",
   "from":{
      "user":{
         "id":"id-value",
         "displayName":"John Doe",
         "userIdentityType":"aadUser"
      }
   },
{
   "body":{
      "contentType":"html",
      "content":"<div><div>\n<div><span><img height=\"250\" src=\"../hostedContents/1/$value\" width=\"176.2295081967213\" style=\"vertical-align:bottom; width:176px; height:250px\"></span>\n\n</div>\n\n\n</div>\n</div>"
   },
   "hostedContents":[
      {
         "@microsoft.graph.temporaryId":"1",
         "contentBytes":"iVBORw0KGgoAAAANSUhEUgAAANcAAAExCAYAAADvFzeeAAAXjklEQVR4Ae2d/XNU1RnH+9e0FFrA0RCIyaS8hRA0HV5KbS1gHRgVpjMClY4GHJ3yYm1HCmXaWttaaZUZtIIFKYi8lFAkvOQ9u5vN225IARVBbX9/Os9NbrLZbMjmhCfJPX5+2Lmb3T25y3O+n/M599x7w9f+++UXwoMakIF7n4GvUdR7X1RqSk01A8CFuZm5GGUAuIwKi72wF3ABF+YyygBwGRUWc2Eu4AIuzGWUAeAyKizmwlzABVyYyygDwGVUWMyFuYALuDCXUQaAy6iwmAtzARdwfWXMdeuzT+TGxz3Sfb1LunrapL07IW3pePDQ5/qavqef0c+OdYAELuAac4jGGkLL9rdvfyo9N9ODQAqBGmmrwGlb/R0u3xG4gMspOC5hG882CoRaaCSA8n1ff9doIQMu4PIOrus3u+8ZVNnw6e/Od5AALuDKOyz5hmqiPnfnzi1J9bSbgRWCpvvQfY307wQu4BoxJCOFaDK8rwsQmQsUIQhWW93XSIsewAVckYdLQ24F0Ui/926AARdwRRounZ6Np7GyYdN9DzdFBC7gijRc43GMlQ1U9s/6HXJNjYELuHI<<-----Removed----->>>>",
         "contentType":"image/png"
      }
   ]
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
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#teams('teamId')/channels('channelId')/messages/$entity",
   "id":"id-value",
   "replyToId":null,
   "etag":"id-value",
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
         "id":"id-value",
         "displayName":"Joh Doe",
         "userIdentityType":"aadUser"
      }
   },
   "body":{
      "contentType":"html",
      "content":"<div><div>\n<div><span><img height=\"250\" src=\"https://graph.microsoft.com/teams/teamId/channels/channelId/messages/id-value/hostedContents/hostedContentId/$value\" width=\"176.2295081967213\" style=\"vertical-align:bottom; width:176px; height:250px\"></span>\n\n</div>\n\n\n</div>\n</div>"
   },
   "attachments":[ ],
   "mentions":[ ],
   "reactions":[ ]
}

```

## <a name="see-also"></a>Confira também

* [Importar mensagens de plataforma de terceiros para o Teams usando o Microsoft Graph](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [Create channel](channel-post.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Send message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
