---
title: Listar conversationMembers
description: Recuperar um membro de um bate-papo.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 14247f27d1a4a656afebca28608ce0797c491248
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319717"
---
# <a name="list-conversationmembers"></a><span data-ttu-id="e0874-103">Listar conversationMembers</span><span class="sxs-lookup"><span data-stu-id="e0874-103">List conversationMembers</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0874-104">Listar todos os [membros da conversa](../resources/conversationmember.md) em um [bate-papo](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="e0874-104">List all [conversation members](../resources/conversationmember.md) in a [chat](../resources/chat.md)</span></span>

## <a name="permissions"></a><span data-ttu-id="e0874-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e0874-105">Permissions</span></span>

<span data-ttu-id="e0874-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0874-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0874-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0874-108">Permission Type</span></span>|<span data-ttu-id="e0874-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e0874-109">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="e0874-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0874-110">Delegated (work or school account)</span></span>|<span data-ttu-id="e0874-111">Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e0874-111">Chat.Read, Chat.ReadWrite</span></span>|
|<span data-ttu-id="e0874-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0874-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0874-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e0874-113">Not supported</span></span>|
|<span data-ttu-id="e0874-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0874-114">Application</span></span>| <span data-ttu-id="e0874-115">Chat.Read.All, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0874-115">Chat.Read.All, Chat.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0874-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0874-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members
GET /users/{id}/chats/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0874-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e0874-117">Optional query parameters</span></span>

<span data-ttu-id="e0874-118">Esta operação não é compatível com os [parâmetros de consulta OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e0874-118">This operation does not currently support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0874-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0874-119">Request headers</span></span>

| <span data-ttu-id="e0874-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e0874-120">Header</span></span>       | <span data-ttu-id="e0874-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e0874-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e0874-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0874-122">Authorization</span></span>  | <span data-ttu-id="e0874-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0874-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e0874-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0874-125">Request body</span></span>

<span data-ttu-id="e0874-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e0874-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0874-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0874-127">Response</span></span>

<span data-ttu-id="e0874-128">Se bem sucedido, este método retorna um código de resposta `200 OK` e uma lista de objetos [conversationMember](../resources/conversationmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0874-128">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/conversationmember.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0874-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0874-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e0874-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0874-130">Request</span></span>

<span data-ttu-id="e0874-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0874-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e0874-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0874-132">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```http
GET https://graph.microsoft.com/beta/me/chats/{id}/members
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e0874-133">C#</span><span class="sxs-lookup"><span data-stu-id="e0874-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-conversation-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0874-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0874-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-conversation-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e0874-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0874-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-conversation-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e0874-136">Java</span><span class="sxs-lookup"><span data-stu-id="e0874-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-conversation-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e0874-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0874-137">Response</span></span>

<span data-ttu-id="e0874-138">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0874-138">Here is an example of the response.</span></span>

><span data-ttu-id="e0874-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0874-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
