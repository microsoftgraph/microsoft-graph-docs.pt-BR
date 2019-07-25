---
title: Remover rejectedSender
description: Remover um usuário ou grupo da lista de remetentes rejeitados.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f15fce9cb8d3d28e39427d1fa4d4a185b3ebde10
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35890741"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="ef5b4-103">Remover rejectedSender</span><span class="sxs-lookup"><span data-stu-id="ef5b4-103">Remove rejectedSender</span></span>
<span data-ttu-id="ef5b4-104">Remover um usuário ou grupo da lista de remetentes rejeitados.</span><span class="sxs-lookup"><span data-stu-id="ef5b4-104">Remove a user or group from the rejected-senders list.</span></span>

## <a name="permissions"></a><span data-ttu-id="ef5b4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ef5b4-105">Permissions</span></span>
<span data-ttu-id="ef5b4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef5b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ef5b4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ef5b4-108">Permission type</span></span>                        | <span data-ttu-id="ef5b4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ef5b4-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="ef5b4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ef5b4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef5b4-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef5b4-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="ef5b4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ef5b4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef5b4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef5b4-113">Not supported.</span></span> |
| <span data-ttu-id="ef5b4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ef5b4-114">Application</span></span>                            | <span data-ttu-id="ef5b4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ef5b4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ef5b4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ef5b4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
DELETE /groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/groups/{other-group-id}
```

## <a name="request-headers"></a><span data-ttu-id="ef5b4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ef5b4-117">Request headers</span></span>

| <span data-ttu-id="ef5b4-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ef5b4-118">Header</span></span>         | <span data-ttu-id="ef5b4-119">Valor</span><span class="sxs-lookup"><span data-stu-id="ef5b4-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="ef5b4-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ef5b4-120">Authorization</span></span>  | <span data-ttu-id="ef5b4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ef5b4-p102">Bearer {token}. Required.</span></span> 

## <a name="request-body"></a><span data-ttu-id="ef5b4-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ef5b4-123">Request body</span></span>
<span data-ttu-id="ef5b4-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ef5b4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ef5b4-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef5b4-125">Response</span></span>
<span data-ttu-id="ef5b4-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ef5b4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef5b4-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ef5b4-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="ef5b4-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ef5b4-129">Request</span></span>
<span data-ttu-id="ef5b4-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ef5b4-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ef5b4-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef5b4-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "remove_rejectedSender_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ef5b4-132">C#</span><span class="sxs-lookup"><span data-stu-id="ef5b4-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-rejectedsender-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ef5b4-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="ef5b4-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-rejectedsender-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ef5b4-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ef5b4-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-rejectedsender-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ef5b4-135">Java</span><span class="sxs-lookup"><span data-stu-id="ef5b4-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-rejectedsender-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ef5b4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="ef5b4-136">Response</span></span>
<span data-ttu-id="ef5b4-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ef5b4-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Remove rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
