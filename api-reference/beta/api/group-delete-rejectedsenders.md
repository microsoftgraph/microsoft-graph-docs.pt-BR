---
title: Remover rejectedSender
description: Remover um usuário ou grupo da lista de remetentes rejeitados.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: ef3e1dd0e6280200d789c11659cd7d2ecd0f80ce
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263306"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="c73e4-103">Remover rejectedSender</span><span class="sxs-lookup"><span data-stu-id="c73e4-103">Remove rejectedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c73e4-104">Remover um usuário ou grupo da lista de remetentes rejeitados do grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="c73e4-104">Remove a user or group from the rejected-senders list of the specified group.</span></span>

## <a name="permissions"></a><span data-ttu-id="c73e4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c73e4-105">Permissions</span></span>
<span data-ttu-id="c73e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c73e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c73e4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c73e4-108">Permission type</span></span>                        | <span data-ttu-id="c73e4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c73e4-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="c73e4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c73e4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c73e4-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c73e4-111">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="c73e4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c73e4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c73e4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c73e4-113">Not supported.</span></span> |
| <span data-ttu-id="c73e4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c73e4-114">Application</span></span>                            | <span data-ttu-id="c73e4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c73e4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c73e4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c73e4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="c73e4-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c73e4-117">Request headers</span></span>

| <span data-ttu-id="c73e4-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c73e4-118">Header</span></span>         | <span data-ttu-id="c73e4-119">Valor</span><span class="sxs-lookup"><span data-stu-id="c73e4-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="c73e4-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="c73e4-120">Authorization</span></span>  | <span data-ttu-id="c73e4-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c73e4-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="c73e4-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c73e4-123">Request body</span></span>
<span data-ttu-id="c73e4-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c73e4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c73e4-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="c73e4-125">Response</span></span>
<span data-ttu-id="c73e4-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c73e4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c73e4-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c73e4-128">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="c73e4-129">Exemplo 1: remover um usuário da lista de remetentes rejeitados do grupo.</span><span class="sxs-lookup"><span data-stu-id="c73e4-129">Example 1: Remove a user from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="c73e4-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c73e4-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_user_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}
```
#### <a name="response"></a><span data-ttu-id="c73e4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="c73e4-131">Response</span></span>
<span data-ttu-id="c73e4-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c73e4-132">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c73e4-133">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="c73e4-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c73e4-134">C#</span><span class="sxs-lookup"><span data-stu-id="c73e4-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/remove_user_from_rejectedsenderslist_of_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c73e4-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="c73e4-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/remove_user_from_rejectedsenderslist_of_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c73e4-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c73e4-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/remove_user_from_rejectedsenderslist_of_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-remove-a-group-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="c73e4-137">Exemplo 2: remover um grupo da lista de remetentes rejeitados do grupo.</span><span class="sxs-lookup"><span data-stu-id="c73e4-137">Example 2: Remove a group from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="c73e4-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c73e4-138">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "remove_group_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```

#### <a name="response"></a><span data-ttu-id="c73e4-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="c73e4-139">Response</span></span>
<span data-ttu-id="c73e4-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c73e4-140">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c73e4-141">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="c73e4-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c73e4-142">C#</span><span class="sxs-lookup"><span data-stu-id="c73e4-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/remove_group_from_rejectedsenderslist_of_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c73e4-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="c73e4-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/remove_group_from_rejectedsenderslist_of_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c73e4-144">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="c73e4-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/remove_group_from_rejectedsenderslist_of_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
