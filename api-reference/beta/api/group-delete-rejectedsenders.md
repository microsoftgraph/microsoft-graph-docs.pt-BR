---
title: Remover rejectedSender
description: Remover um usuário ou grupo da lista de remetentes rejeitados.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 41ffc56b6b30d8b3e0d6231027c265d6540d462e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42420182"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="7d362-103">Remover rejectedSender</span><span class="sxs-lookup"><span data-stu-id="7d362-103">Remove rejectedSender</span></span>

<span data-ttu-id="7d362-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7d362-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d362-105">Remover um usuário ou grupo da lista de remetentes rejeitados do grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="7d362-105">Remove a user or group from the rejected-senders list of the specified group.</span></span>

## <a name="permissions"></a><span data-ttu-id="7d362-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7d362-106">Permissions</span></span>
<span data-ttu-id="7d362-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7d362-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7d362-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7d362-109">Permission type</span></span>                        | <span data-ttu-id="7d362-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7d362-110">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="7d362-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7d362-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7d362-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d362-112">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="7d362-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7d362-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7d362-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d362-114">Not supported.</span></span> |
| <span data-ttu-id="7d362-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7d362-115">Application</span></span>                            | <span data-ttu-id="7d362-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7d362-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7d362-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7d362-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="7d362-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7d362-118">Request headers</span></span>

| <span data-ttu-id="7d362-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7d362-119">Header</span></span>         | <span data-ttu-id="7d362-120">Valor</span><span class="sxs-lookup"><span data-stu-id="7d362-120">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="7d362-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="7d362-121">Authorization</span></span>  | <span data-ttu-id="7d362-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7d362-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="7d362-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7d362-124">Request body</span></span>
<span data-ttu-id="7d362-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7d362-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7d362-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d362-126">Response</span></span>
<span data-ttu-id="7d362-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7d362-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7d362-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="7d362-129">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="7d362-130">Exemplo 1: remover um usuário da lista de remetentes rejeitados do grupo.</span><span class="sxs-lookup"><span data-stu-id="7d362-130">Example 1: Remove a user from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="7d362-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d362-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="7d362-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d362-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_user_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}
```
# <a name="c"></a>[<span data-ttu-id="7d362-133">C#</span><span class="sxs-lookup"><span data-stu-id="7d362-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-user-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d362-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d362-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-user-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d362-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d362-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-user-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="7d362-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d362-136">Response</span></span>
<span data-ttu-id="7d362-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7d362-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="7d362-138">Exemplo 2: remover um grupo da lista de remetentes rejeitados do grupo.</span><span class="sxs-lookup"><span data-stu-id="7d362-138">Example 2: Remove a group from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="7d362-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7d362-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="7d362-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="7d362-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_group_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```
# <a name="c"></a>[<span data-ttu-id="7d362-141">C#</span><span class="sxs-lookup"><span data-stu-id="7d362-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-group-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7d362-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7d362-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-group-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7d362-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7d362-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-group-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7d362-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7d362-144">Response</span></span>
<span data-ttu-id="7d362-145">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="7d362-145">The following is an example of the response.</span></span> 
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
