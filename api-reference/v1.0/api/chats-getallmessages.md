---
title: 'chats: getAllMessages'
description: Obter mensagens de todos os chats nos quais um usuário é um participante.
author: RamjotSingh
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 998be54216d3e961b89527f39bd657ac63dd2c3e
ms.sourcegitcommit: 70b3caded085ba8ef15e389f81fa005506f1e2fb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2021
ms.locfileid: "61131905"
---
# <a name="chats-getallmessages"></a>chats: getAllMessages

Namespace: microsoft.graph

Obtenha todas [mensagens](../resources/chatmessage.md) de todos os [chats](../resources/chat.md) em que um usuário é participante, incluindo chats individuais, chats em grupo e chats de reunião.

[!INCLUDE [teams-model-A-and-B-disclaimer](../../includes/teams-model-A-and-B-disclaimer.md)]

## <a name="permissions"></a>Permissões

As seguintes permissões são obrigatórias para chamar esta API. Para saber mais, incluindo como escolher as permissões, consulte [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)| Sem suporte. |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo | Chat.Read.All, Chat.ReadWrite.All |

> [!NOTE]
> Antes de chamar essa API com permissões de aplicativo, você deve solicitar acesso. Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->
``` http
GET /users/{id | user-principal-name}/chats/getAllMessages
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Você pode usar `model` parâmetro de consulta, que suporta os valores `A` e `B`, com base nos requisitos preferenciais de licenciamento e pagamento, como mostrado nos exemplos a seguir.  

```http
GET /users/{id | user-principal-name}/chats/getAllMessages?model=A
GET /users/{id | user-principal-name}/chats/getAllMessages?model=B
```
Se nenhum `model` for especificado, [modo de avaliação](/graph/teams-licenses#evaluation-mode-default-requirements) será usado.

Esta operação também suporta [parâmetros de faixa de datas](/graph/query-parameters) para personalizar a resposta, como mostrado no exemplo a seguir.

``` http
GET /users/{id}/chats/getAllMessages?$top=50&$filter=lastModifiedDateTime gt 2020-06-04T18:03:11.591Z and lastModifiedDateTime lt 2020-06-05T21:00:09.413Z
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório. |

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [event](../resources/chatmessage.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chat_getallmessages_1"
}-->
``` http
GET https://graph.microsoft.com/v1.0/users/0b4f1cf6-54c8-4820-bbb7-2a1f4257ade5/chats/getAllMessages?$top=2
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chat-getallmessages-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chat-getallmessages-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chat-getallmessages-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/chat-getallmessages-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/chat-getallmessages-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage",
  "isCollection": true
} -->
``` http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(chatMessage)",
    "@odata.count": 2,
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/users('0b4f1cf6-54c8-4820-bbb7-2a1f4257ade5')/chats/getallMessages?$top=2&$skiptoken=U2tpcFZhbHVlPTIjTWFpbGJveEZvbGRlcj1NYWlsRm9sZGVycy9UZWFtc01lc3NhZ2VzRGF0YQ%3d%3d",
    "value": [
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "id": "1621973534864",
            "replyToId": null,
            "etag": "1621973534864",
            "messageType": "message",
            "createdDateTime": "2021-05-25T20:12:14.864Z",
            "lastModifiedDateTime": "2021-05-25T20:12:14.864Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": "19:3c9e92a344704332bbf5bda58f4d37b1@thread.v2",
            "importance": "normal",
            "locale": "en-us",
            "webUrl": null,
            "channelIdentity": null,
            "policyViolation": null,
            "eventDetail": null,
            "from": {
                "application": null,
                "device": null,
                "user": {
                    "id": "0b4f1cf6-54c8-4820-bbb7-2a1f4257ade5",
                    "displayName": "user1 a",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "Hello user2, user 3"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        },
        {
            "@odata.type": "#microsoft.graph.chatMessage",
            "id": "1622762567488",
            "replyToId": null,
            "etag": "1622762567488",
            "messageType": "message",
            "createdDateTime": "2021-06-03T23:22:47.488Z",
            "lastModifiedDateTime": "2021-06-03T23:22:47.488Z",
            "lastEditedDateTime": null,
            "deletedDateTime": null,
            "subject": null,
            "summary": null,
            "chatId": "19:0b4f1cf6-54c8-4820-bbb7-2a1f4257ade5_0d7c63d3-1306-4eec-8f21-588a70fb6ef1@unq.gbl.spaces",
            "importance": "normal",
            "locale": "en-us",
            "webUrl": null,
            "channelIdentity": null,
            "policyViolation": null,
            "eventDetail": null,
            "from": {
                "application": null,
                "device": null,
                "user": {
                    "id": "0b4f1cf6-54c8-4820-bbb7-2a1f4257ade5",
                    "displayName": "user1 a",
                    "userIdentityType": "aadUser"
                }
            },
            "body": {
                "contentType": "text",
                "content": "hi user2"
            },
            "attachments": [],
            "mentions": [],
            "reactions": []
        }
    ]
}
```
