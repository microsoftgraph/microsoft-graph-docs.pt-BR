---
title: Criar chat
description: Use esta API para criar um novo chat.
localization_priority: Normal
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cb9f939e6c58ce83ad1386e9303d95978e0a6d58
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261448"
---
# <a name="create-chatmessage"></a>Criar chat

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Criar uma nova [mensagem](../resources/chatmessage.md) no [chat](../resources/chat.md)especificado.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Chat. ReadWrite |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /chats/{id}/messages
POST /users/{id}/chats/{id}/messages
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Authorization | Portador {código} |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON do objeto [chat](../resources/chatmessage.md) .

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [chat](../resources/chatmessage.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "create_chatmessage_from_chat"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels/{id}/messages
Content-type: application/json

{
  "body": {
     "content" : "Hello world"
  }
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> [!NOTE]
> O objeto de resposta mostrado aqui pode ser reduzido para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chatMessage"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "id-value",
  "replyToId": "replyToId-value",
  "from": {
    "application": null,
    "device": null,
    "user": {
      "id": "87ea812c-8816-40e9-b770-5c165fa31397",
      "displayName": "Test User"
    }
  },
  "messageType": "message",
  "body": {
     "content": "Hello world",
     "contentType": "text"
  }
}
```
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK

# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_chat-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_chat-Javascript-snippets.md)]
# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_chatmessage_from_chat-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create chatMessage",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/chat-post-messages.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/chat-post-messages.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/chat-post-messages.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)"
  ]
}-->
