---
title: Atualizar chat
description: Atualize a propriedade policyViolation de um chat.
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e3a5fa4703ccf04a13c4575d2131b9834f5154f7
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848015"
---
# <a name="update-chatmessage"></a>Atualizar chat

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Atualizar um objeto [chat](../resources/chatMessage.md) . Somente a propriedade **policyViolation** de um **chat** pode ser atualizada.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | Sem suporte. |
|Delegada (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Chat. UpdatePolicyViolation. All para uma mensagem de chat.</br>ChannelMessage. UpdatePolicyViolation. All para uma mensagem de canal. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/(team-id)/channels/{channel-id}/chatMessages/{message-id}
PATCH /users/(user-id)/chats/{chatThread-id}/chatMessages/{message-id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:----------|
| Autorização  | {token} de portador. Obrigatório. |
| Content-Type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON de um objeto [chat](../resources/chatMessage.md) , especificando apenas a propriedade **policyViolation** .

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará uma `200 OK` resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação

Veja a seguir um exemplo da solicitação para atualizar a propriedade **policyViolation** em uma mensagem de canal do Microsoft Teams.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "chatMessage.PatchPolicyViolation.All"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/e1234567-e123-4276-55555-6232b0e3a89a/channels/a7654321-e321-0000-0000-123b0e3a00a/messages/19%3Aa21b0b0c05194ebc9e30000000000f61%40thread.skype
Content-Type: application/json
Content-Length: 248

{
  "policyViolation": {
    "policyTip": {
      "generalText" : "This item has been blocked by the administrator.",
      "complianceUrl" : "https://contoso.com/dlp-policy-page",
      "matchedConditionDescriptions" : ["Credit Card Number"]
    },
    "verdictDetails" : "AllowOverrideWithoutJustification,AllowFalsePositiveOverride",
    "dlpAction" : "BlockAccess"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/chatmessagepatchpolicyviolationall-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/chatmessagepatchpolicyviolationall-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/chatmessagepatchpolicyviolationall-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

<!-- {
  "blockType": "response",
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessage.UpdatePolicyViolation.All",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
