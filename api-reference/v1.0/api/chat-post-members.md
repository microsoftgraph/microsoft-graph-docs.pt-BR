---
title: Adicionar membro a um chat
description: Adicione um conversationMember a um chat.
author: bhartono
doc_type: apiPageType
ms.localizationpriority: medium
ms.prod: microsoft-teams
ms.openlocfilehash: d97e27a21ae71fb9c32629d841d84070a4bebdbb
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61000667"
---
# <a name="add-member-to-a-chat"></a>Adicionar membro a um chat

Namespace: microsoft.graph

Adicione um [conversationMember](../resources/conversationmember.md) a um [chat](../resources/chat.md).

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|---------|-------------|
|Delegado (conta corporativa ou de estudante)| ChatMember.ReadWrite, Chat.ReadWrite |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo| ChatMember.ReadWrite.All, Chat.ReadWrite.All |

<!-- { "blockType": "ignored"} -->
```http
POST /chats/{chat-id}/members
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
|Content-Type|application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça uma representação JSON do objeto [conversationMember](../resources/conversationmember.md).

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um header location que fornece um caminho `201 Created` de URL para o objeto membro recém-criado.

## <a name="examples"></a>Exemplos

### <a name="example-1-add-a-single-member-to-a-chat-and-specify-the-timespan-for-the-conversation-history"></a>Exemplo 1: adicionar um único membro a um chat e especificar o tempo de tempo para o histórico da conversa

#### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_specific_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5",
    "visibleHistoryStartDateTime": "2019-04-18T23:51:43.255Z",
    "roles": ["owner"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-specific-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-specific-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-specific-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-specific-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-conversation-member-with-specific-visiblehistorystartdatetime-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_with_specific_visibleHistoryStartDateTime"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```

### <a name="example-2-adding-a-single-member-to-a-microsoft-teams-chat-sharing-no-chat-history"></a>Exemplo 2: adicionar um único membro a um Microsoft Teams chat, sem compartilhar nenhum histórico de chat

#### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_no_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5",
    "roles": ["owner"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-no-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-no-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-no-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-no-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-conversation-member-with-no-visiblehistorystartdatetime-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_with_no_visibleHistoryStartDateTime"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```

### <a name="example-3-adding-a-single-member-to-a-microsoft-teams-chat-sharing-the-whole-history-of-the-chat"></a>Exemplo 3: Adicionar um único membro a um Microsoft Teams chat, compartilhando todo o histórico do chat

#### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member_with_all_visibleHistoryStartDateTime"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5",
    "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z",
    "roles": ["owner"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-with-all-visiblehistorystartdatetime-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-with-all-visiblehistorystartdatetime-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-with-all-visiblehistorystartdatetime-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-with-all-visiblehistorystartdatetime-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-conversation-member-with-all-visiblehistorystartdatetime-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_with_all_visibleHistoryStartDateTime"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```

### <a name="example-4-add-a-single-member-to-a-chat-using-user-principal-name"></a>Exemplo 4: Adicionar um único membro a um chat usando o nome principal do usuário

#### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_conversation_member_upn"
} -->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members
content-type: application/json

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "user@odata.bind": "https://graph.microsoft.com/v1.0/users/jacob@contoso.com",
    "visibleHistoryStartDateTime": "2019-04-18T23:51:43.255Z",
    "roles": ["owner"]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-conversation-member-upn-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-conversation-member-upn-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-conversation-member-upn-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-conversation-member-upn-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-conversation-member-upn-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member_upn"
}
-->
```http
HTTP/1.1 201 Created
Location: /chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```


