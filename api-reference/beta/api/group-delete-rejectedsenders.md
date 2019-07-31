---
title: Remover rejectedSender
description: Remover um usuário ou grupo da lista de remetentes rejeitados.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f10877431a1b7931df67697a556f00be4f3cbbab
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954058"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="f7837-103">Remover rejectedSender</span><span class="sxs-lookup"><span data-stu-id="f7837-103">Remove rejectedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7837-104">Remover um usuário ou grupo da lista de remetentes rejeitados do grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="f7837-104">Remove a user or group from the rejected-senders list of the specified group.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7837-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f7837-105">Permissions</span></span>
<span data-ttu-id="f7837-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7837-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f7837-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7837-108">Permission type</span></span>                        | <span data-ttu-id="f7837-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f7837-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="f7837-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7837-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f7837-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7837-111">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="f7837-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7837-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7837-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7837-113">Not supported.</span></span> |
| <span data-ttu-id="f7837-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7837-114">Application</span></span>                            | <span data-ttu-id="f7837-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7837-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7837-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7837-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="f7837-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7837-117">Request headers</span></span>

| <span data-ttu-id="f7837-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7837-118">Header</span></span>         | <span data-ttu-id="f7837-119">Valor</span><span class="sxs-lookup"><span data-stu-id="f7837-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="f7837-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7837-120">Authorization</span></span>  | <span data-ttu-id="f7837-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7837-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="f7837-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7837-123">Request body</span></span>
<span data-ttu-id="f7837-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f7837-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7837-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7837-125">Response</span></span>
<span data-ttu-id="f7837-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7837-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f7837-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f7837-128">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="f7837-129">Exemplo 1: remover um usuário da lista de remetentes rejeitados do grupo.</span><span class="sxs-lookup"><span data-stu-id="f7837-129">Example 1: Remove a user from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="f7837-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7837-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="f7837-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7837-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_user_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f7837-132">C#</span><span class="sxs-lookup"><span data-stu-id="f7837-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-user-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7837-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="f7837-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-user-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f7837-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f7837-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-user-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f7837-135">Java</span><span class="sxs-lookup"><span data-stu-id="f7837-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-user-from-rejectedsenderslist-of-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f7837-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7837-136">Response</span></span>
<span data-ttu-id="f7837-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f7837-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="f7837-138">Exemplo 2: remover um grupo da lista de remetentes rejeitados do grupo.</span><span class="sxs-lookup"><span data-stu-id="f7837-138">Example 2: Remove a group from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="f7837-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7837-139">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f7837-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7837-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_group_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f7837-141">C#</span><span class="sxs-lookup"><span data-stu-id="f7837-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-group-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f7837-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="f7837-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-group-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f7837-143">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f7837-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-group-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="f7837-144">Java</span><span class="sxs-lookup"><span data-stu-id="f7837-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-group-from-rejectedsenderslist-of-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f7837-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7837-145">Response</span></span>
<span data-ttu-id="f7837-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f7837-146">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
