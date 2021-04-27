---
title: Liste os membros de um bate-papo.
description: Recupere os membros de um bate-papo.
author: bhartono
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e96fdce4e22aa1f83337ca9be938b648394808ac
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047291"
---
# <a name="list-members-of-a-chat"></a><span data-ttu-id="1e36f-103">Liste os membros de um bate-papo.</span><span class="sxs-lookup"><span data-stu-id="1e36f-103">List members of a chat</span></span>

<span data-ttu-id="1e36f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e36f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e36f-105">Listar todos os [membros da conversa](../resources/conversationmember.md) de um [bate-papo](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="1e36f-105">List all [conversation members](../resources/conversationmember.md) in a [chat](../resources/chat.md).</span></span>

> [!NOTE]
> <span data-ttu-id="1e36f-106">As IDs de associação retornadas pelo servidor devem ser tratadas como cadeias de caracteres opacas.</span><span class="sxs-lookup"><span data-stu-id="1e36f-106">The membership IDs returned by the server must be treated as opaque strings.</span></span> <span data-ttu-id="1e36f-107">O cliente não deve tentar analisar ou fazer suposições sobre essas IDs do recursos.</span><span class="sxs-lookup"><span data-stu-id="1e36f-107">The client should not try to parse or make any assumptions about these resource IDs.</span></span>
>
> <span data-ttu-id="1e36f-p102">Os resultados da associação podem ser mapeados para usuários de diferentes locatários, conforme indicado na resposta, no futuro. O cliente não deve presumir que todos os membros sejam apenas do locatário atual.</span><span class="sxs-lookup"><span data-stu-id="1e36f-p102">The membership results could map to users from different tenants, as indicated in the response, in the future. The client should not assume that all members are from the current tenant only.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e36f-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="1e36f-110">Permissions</span></span>

<span data-ttu-id="1e36f-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e36f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e36f-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e36f-113">Permission Type</span></span>|<span data-ttu-id="1e36f-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1e36f-114">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="1e36f-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e36f-115">Delegated (work or school account)</span></span>| <span data-ttu-id="1e36f-116">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1e36f-116">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="1e36f-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e36f-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e36f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e36f-118">Not supported.</span></span>|
|<span data-ttu-id="1e36f-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e36f-119">Application</span></span>| <span data-ttu-id="1e36f-120">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="1e36f-120">ChatMember.Read.All, ChatMember.ReadWrite.All, Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All.</span></span> |

> [!NOTE]
> <span data-ttu-id="1e36f-121">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1e36f-121">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="1e36f-122">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="1e36f-122">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="1e36f-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e36f-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/members
GET /users/{user-id}/chats/{chat-id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1e36f-124">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1e36f-124">Optional query parameters</span></span>

<span data-ttu-id="1e36f-125">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1e36f-125">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e36f-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e36f-126">Request headers</span></span>

| <span data-ttu-id="1e36f-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e36f-127">Header</span></span>       | <span data-ttu-id="1e36f-128">Valor</span><span class="sxs-lookup"><span data-stu-id="1e36f-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="1e36f-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e36f-129">Authorization</span></span>  | <span data-ttu-id="1e36f-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e36f-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1e36f-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e36f-132">Request body</span></span>

<span data-ttu-id="1e36f-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1e36f-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e36f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e36f-134">Response</span></span>

<span data-ttu-id="1e36f-135">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma lista de objetos [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e36f-135">If successful, this method returns a `200 OK` response code and a list of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e36f-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e36f-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e36f-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e36f-137">Request</span></span>

<span data-ttu-id="1e36f-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e36f-138">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1e36f-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e36f-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_conversation_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/chats/19:8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d@unq.gbl.spaces/members
```
# <a name="c"></a>[<span data-ttu-id="1e36f-140">C#</span><span class="sxs-lookup"><span data-stu-id="1e36f-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-conversation-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1e36f-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e36f-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-conversation-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1e36f-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1e36f-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-conversation-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1e36f-143">Java</span><span class="sxs-lookup"><span data-stu-id="1e36f-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-conversation-members-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1e36f-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e36f-144">Response</span></span>

<span data-ttu-id="1e36f-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e36f-145">Here is an example of the response.</span></span>

><span data-ttu-id="1e36f-146">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1e36f-146">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')/chats('19%3A8b081ef6-4792-4def-b2c9-c363a1bf41d5_5031bb31-22c0-4f6f-9f73-91d34ab2b32d%40unq.gbl.spaces')/members",
    "@odata.count": 3,
    "value": [
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "roles": [
                "owner"
            ],
            "displayName": "John Doe",
            "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
            "email": null,
            "tenantId": "6e5147da-6a35-4275-b3f3-fc069456b6eb",
            "visibleHistoryStartDateTime": "2019-04-18T23:51:43.255Z"
        },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "2de87aaf-844d-4def-9dee-2c317f0be1b3",
            "roles": [
                "owner"
            ],
            "displayName": "Bart Hogan",
            "userId": "2de87aaf-844d-4def-9dee-2c317f0be1b3",
            "email": null,
            "tenantId": "6e5147da-6a35-4275-b3f3-fc069456b6eb",
            "visibleHistoryStartDateTime": "0001-01-01T00:00:00Z"
    },
        {
            "@odata.type": "#microsoft.graph.aadUserConversationMember",
            "id": "07ad17ad-ada5-4f1f-a650-7a963886a8a7",
            "roles": [
                "owner"
            ],
            "displayName": "Minna Pham",
            "userId": "07ad17ad-ada5-4f1f-a650-7a963886a8a7",
            "email": null,
            "tenantId": "6e5147da-6a35-4275-b3f3-fc069456b6eb",
            "visibleHistoryStartDateTime": "2019-04-18T23:51:43.255Z"
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


