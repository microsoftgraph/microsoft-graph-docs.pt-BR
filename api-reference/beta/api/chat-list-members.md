---
title: Liste os membros de um bate-papo.
description: Recupere os membros de um bate-papo.
author: anandjo
ms.localizationpriority: high
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fe42a5220550e77e99a2eba3c9848dd63959dc42
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394464"
---
# <a name="list-members-of-a-chat"></a>Liste os membros de um bate-papo.

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Listar todos os [membros da conversa](../resources/conversationmember.md) de um [bate-papo](../resources/chat.md).

> [!NOTE]
> As IDs de associação retornadas pelo servidor devem ser tratadas como cadeias de caracteres opacas. O cliente não deve tentar analisar ou fazer suposições sobre essas IDs do recursos.
>
> Os resultados da associação podem ser mapeados para usuários de diferentes locatários, conforme indicado na resposta, no futuro. O cliente não deve presumir que todos os membros sejam apenas do locatário atual.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|---------|-------------|
|Delegado (conta corporativa ou de estudante)| ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo| ChatMember.Read.Chat *, Chat.Manage.Chat*, ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All |

> **Observação**: Permissões marcadas com * usam [consentimento específico de recurso](/microsoftteams/platform/graph-api/rsc/resource-specific-consent).

> [!NOTE]
> Antes de chamar essa API com permissões de aplicativo, você deve solicitar acesso. Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/members
GET /users/{user-id | user-principal-name}/chats/{chat-id}/members
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

### <a name="request"></a>Solicitação

Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_conversation_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/chats/19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d@unq.gbl.spaces/members
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-conversation-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-conversation-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-conversation-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-conversation-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-conversation-members-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
   "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d%40unq.gbl.spaces')/members",
   "@odata.count":3,
   "value":[
      {
         "@odata.type":"#microsoft.graph.aadUserConversationMember",
         "id":"8b081ef6-4792-4def-b2c9-c363a1bf41d5",
         "roles":[
            "owner"
         ],
         "displayName":"John Doe",
         "userId":"8b081ef6-4792-4def-b2c9-c363a1bf41d5",
         "email":null,
         "tenantId":"6e5147da-6a35-4275-b3f3-fc069456b6eb",
         "visibleHistoryStartDateTime":"2019-04-18T23:51:43.255Z"
      },
      {
         "@odata.type":"#microsoft.graph.aadUserConversationMember",
         "id":"2de87aaf-844d-4def-9dee-2c317f0be1b3",
         "roles":[
            "owner"
         ],
         "displayName":"Bart Hogan",
         "userId":"2de87aaf-844d-4def-9dee-2c317f0be1b3",
         "email":null,
         "tenantId":"6e5147da-6a35-4275-b3f3-fc069456b6eb",
         "visibleHistoryStartDateTime":"0001-01-01T00:00:00Z"
      },
      {
         "@odata.type":"#microsoft.graph.aadUserConversationMember",
         "id":"07ad17ad-ada5-4f1f-a650-7a963886a8a7",
         "roles":[
            "owner"
         ],
         "displayName":"Minna Pham",
         "userId":"07ad17ad-ada5-4f1f-a650-7a963886a8a7",
         "email":null,
         "tenantId":"6e5147da-6a35-4275-b3f3-fc069456b6eb",
         "visibleHistoryStartDateTime":"2019-04-18T23:51:43.255Z"
      }
   ]
}
```

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
  ]
}
-->
