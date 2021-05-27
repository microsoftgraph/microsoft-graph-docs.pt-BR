---
title: Remover rejectedSender
description: Remova um usuário ou grupo da lista de envios rejeitados.
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 14bdcef8d41d204e3c3ae6f3de08a3d1cc53a5ff
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681824"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="c6e4a-103">Remover rejectedSender</span><span class="sxs-lookup"><span data-stu-id="c6e4a-103">Remove rejectedSender</span></span>

<span data-ttu-id="c6e4a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6e4a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6e4a-105">Remova um usuário ou grupo da lista de envios rejeitados do grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="c6e4a-105">Remove a user or group from the rejected-senders list of the specified group.</span></span>

## <a name="permissions"></a><span data-ttu-id="c6e4a-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c6e4a-106">Permissions</span></span>
<span data-ttu-id="c6e4a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6e4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c6e4a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c6e4a-109">Permission type</span></span>                        | <span data-ttu-id="c6e4a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c6e4a-110">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="c6e4a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c6e4a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c6e4a-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6e4a-112">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="c6e4a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c6e4a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c6e4a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6e4a-114">Not supported.</span></span> |
| <span data-ttu-id="c6e4a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c6e4a-115">Application</span></span>                            | <span data-ttu-id="c6e4a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c6e4a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6e4a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c6e4a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="c6e4a-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c6e4a-118">Request headers</span></span>

| <span data-ttu-id="c6e4a-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c6e4a-119">Header</span></span>         | <span data-ttu-id="c6e4a-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c6e4a-120">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="c6e4a-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c6e4a-121">Authorization</span></span>  | <span data-ttu-id="c6e4a-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c6e4a-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="c6e4a-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c6e4a-124">Request body</span></span>
<span data-ttu-id="c6e4a-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c6e4a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c6e4a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6e4a-126">Response</span></span>
<span data-ttu-id="c6e4a-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c6e4a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c6e4a-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c6e4a-129">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="c6e4a-130">Exemplo 1: Remover um usuário da lista rejeitado-senders do grupo.</span><span class="sxs-lookup"><span data-stu-id="c6e4a-130">Example 1: Remove a user from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="c6e4a-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6e4a-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c6e4a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6e4a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_user_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}
```
# <a name="c"></a>[<span data-ttu-id="c6e4a-133">C#</span><span class="sxs-lookup"><span data-stu-id="c6e4a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-user-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6e4a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6e4a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-user-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6e4a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6e4a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-user-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c6e4a-136">Java</span><span class="sxs-lookup"><span data-stu-id="c6e4a-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-user-from-rejectedsenderslist-of-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="c6e4a-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6e4a-137">Response</span></span>
<span data-ttu-id="c6e4a-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c6e4a-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="c6e4a-139">Exemplo 2: Remover um grupo da lista rejeitado-senders do grupo.</span><span class="sxs-lookup"><span data-stu-id="c6e4a-139">Example 2: Remove a group from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="c6e4a-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c6e4a-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="c6e4a-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6e4a-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_group_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```
# <a name="c"></a>[<span data-ttu-id="c6e4a-142">C#</span><span class="sxs-lookup"><span data-stu-id="c6e4a-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-group-from-rejectedsenderslist-of-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6e4a-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6e4a-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-group-from-rejectedsenderslist-of-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6e4a-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6e4a-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-group-from-rejectedsenderslist-of-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c6e4a-145">Java</span><span class="sxs-lookup"><span data-stu-id="c6e4a-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-group-from-rejectedsenderslist-of-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c6e4a-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="c6e4a-146">Response</span></span>
<span data-ttu-id="c6e4a-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c6e4a-147">The following is an example of the response.</span></span> 
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


