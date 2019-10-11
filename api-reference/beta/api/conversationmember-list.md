---
title: Listar conversationMembers
description: Recuperar um membro de um chat ou canal.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 00d3a31d11f354204a64c1957d611a06f5c004be
ms.sourcegitcommit: e4b0211db9b20dfea8be964003661cd99fe064d1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2019
ms.locfileid: "37439803"
---
# <a name="list-conversationmembers"></a><span data-ttu-id="9a846-103">Listar conversationMembers</span><span class="sxs-lookup"><span data-stu-id="9a846-103">List conversationMembers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a846-104">Listar todos os [membros da conversa](../resources/conversationmember.md) de um [chat](../resources/chat.md) ou [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="9a846-104">List all [conversation members](../resources/conversationmember.md) in a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9a846-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="9a846-105">Permissions</span></span>

<span data-ttu-id="9a846-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a846-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a846-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9a846-108">Permission Type</span></span>|<span data-ttu-id="9a846-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9a846-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="9a846-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9a846-110">Delegated (work or school account)</span></span>|<span data-ttu-id="9a846-111">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9a846-111">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="9a846-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9a846-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a846-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="9a846-113">Not supported</span></span>|
|<span data-ttu-id="9a846-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9a846-114">Application</span></span>| <span data-ttu-id="9a846-115">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a846-115">Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="9a846-116">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9a846-116">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="9a846-117">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="9a846-117">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="9a846-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9a846-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members
GET /users/{id}/chats/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9a846-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9a846-119">Optional query parameters</span></span>

<span data-ttu-id="9a846-120">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9a846-120">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9a846-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9a846-121">Request headers</span></span>

| <span data-ttu-id="9a846-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9a846-122">Header</span></span>       | <span data-ttu-id="9a846-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9a846-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9a846-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9a846-124">Authorization</span></span>  | <span data-ttu-id="9a846-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9a846-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9a846-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9a846-127">Request body</span></span>

<span data-ttu-id="9a846-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9a846-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9a846-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a846-129">Response</span></span>

<span data-ttu-id="9a846-130">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma lista de objetos [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a846-130">If successful, this method returns a `200 OK` response code and collection of [Event](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a846-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9a846-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9a846-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9a846-132">Request</span></span>

<span data-ttu-id="9a846-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9a846-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9a846-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9a846-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_conversation_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/chats/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9a846-135">C#</span><span class="sxs-lookup"><span data-stu-id="9a846-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-conversation-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9a846-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9a846-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-conversation-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9a846-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9a846-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-conversation-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9a846-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9a846-138">Response</span></span>

<span data-ttu-id="9a846-139">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9a846-139">Here is an example of the response.</span></span>

><span data-ttu-id="9a846-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9a846-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
