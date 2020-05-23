---
title: Listar conversationMembers
description: Recuperar um membro de um chat ou canal.
author: clearab
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f5454db8b04fee03c2c5ae27e0842df6aa0781fb
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44288512"
---
# <a name="list-conversationmembers"></a><span data-ttu-id="0e7cc-103">Listar conversationMembers</span><span class="sxs-lookup"><span data-stu-id="0e7cc-103">List conversationMembers</span></span>

<span data-ttu-id="0e7cc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e7cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e7cc-105">Listar todos os [membros da conversa](../resources/conversationmember.md) de um [chat](../resources/chat.md) ou [canal](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="0e7cc-105">List all [conversation members](../resources/conversationmember.md) in a [chat](../resources/chat.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0e7cc-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e7cc-106">Permissions</span></span>

<span data-ttu-id="0e7cc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e7cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e7cc-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e7cc-109">Permission Type</span></span>|<span data-ttu-id="0e7cc-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e7cc-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="0e7cc-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e7cc-111">Delegated (work or school account)</span></span>| <span data-ttu-id="0e7cc-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0e7cc-112">Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="0e7cc-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e7cc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e7cc-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e7cc-114">Not supported.</span></span>|
|<span data-ttu-id="0e7cc-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e7cc-115">Application</span></span>| <span data-ttu-id="0e7cc-116">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e7cc-116">Chat.ReadBasic.All, Chat.Read.All, Chat.ReadWrite.All</span></span> |

> [!NOTE]
> <span data-ttu-id="0e7cc-117">É necessário solicitar acesso antes de chamar essa API com permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0e7cc-117">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="0e7cc-118">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="0e7cc-118">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="0e7cc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e7cc-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members
GET /users/{id}/chats/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e7cc-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0e7cc-120">Optional query parameters</span></span>

<span data-ttu-id="0e7cc-121">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0e7cc-121">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e7cc-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e7cc-122">Request headers</span></span>

| <span data-ttu-id="0e7cc-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0e7cc-123">Header</span></span>       | <span data-ttu-id="0e7cc-124">Valor</span><span class="sxs-lookup"><span data-stu-id="0e7cc-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0e7cc-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e7cc-125">Authorization</span></span>  | <span data-ttu-id="0e7cc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e7cc-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0e7cc-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e7cc-128">Request body</span></span>

<span data-ttu-id="0e7cc-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0e7cc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e7cc-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e7cc-130">Response</span></span>

<span data-ttu-id="0e7cc-131">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma lista de objetos [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e7cc-131">If successful, this method returns a `200 OK` response code and a list of [conversationMember](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e7cc-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e7cc-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0e7cc-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e7cc-133">Request</span></span>

<span data-ttu-id="0e7cc-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e7cc-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0e7cc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e7cc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_conversation_members"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/chats/{id}/members
```
# <a name="c"></a>[<span data-ttu-id="0e7cc-136">C#</span><span class="sxs-lookup"><span data-stu-id="0e7cc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-conversation-members-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e7cc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e7cc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-conversation-members-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e7cc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e7cc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-conversation-members-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0e7cc-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e7cc-139">Response</span></span>

<span data-ttu-id="0e7cc-140">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e7cc-140">Here is an example of the response.</span></span>

><span data-ttu-id="0e7cc-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e7cc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
