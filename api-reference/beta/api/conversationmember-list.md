---
title: Listar conversationMembers
description: Recuperar um membro de um bate-papo.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
ms.openlocfilehash: 034332ddf3a8575e82dd7f199d53b6e2d93a7b44
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261100"
---
# <a name="list-conversationmembers"></a>Listar conversationMembers

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Listar todos os [membros da conversa](../resources/conversationmember.md) em um [bate-papo](../resources/chat.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|---------|-------------|
|Delegado (conta corporativa ou de estudante)|Chat.Read, Chat.ReadWrite|
|Delegado (conta pessoal da Microsoft)|Sem suporte|
|Aplicativo| Chat.Read.All, Chat.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members
GET /users/{id}/chats/{id}/members
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais

Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se bem sucedido, este método retorna um código de resposta `200 OK` e uma lista de objetos [conversationMember](../resources/conversationmember.md) no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/me/chats/{id}/members
```

##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

>**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d%40unq.gbl.spaces')/members",
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "roles": [],
            "displayName": "John Doe",
            "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "email": null
        }
    ]
}
```
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/get_conversation_member-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_conversation_member-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objective-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_conversation_member-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation: member list",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/conversationmember-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/conversationmember-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/conversationmember-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
