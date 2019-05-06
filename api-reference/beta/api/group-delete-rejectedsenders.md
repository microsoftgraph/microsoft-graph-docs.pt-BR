---
title: Remover rejectedSender
description: Remover um usuário ou grupo da lista de remetentes rejeitados.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 309a859fd45152fc4cd5e29e3d84db7e8c07664e
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593298"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="dfb37-103">Remover rejectedSender</span><span class="sxs-lookup"><span data-stu-id="dfb37-103">Remove rejectedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfb37-104">Remover um usuário ou grupo da lista de remetentes rejeitados do grupo especificado.</span><span class="sxs-lookup"><span data-stu-id="dfb37-104">Remove a user or group from the rejected-senders list of the specified group.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfb37-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dfb37-105">Permissions</span></span>
<span data-ttu-id="dfb37-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfb37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dfb37-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfb37-108">Permission type</span></span>                        | <span data-ttu-id="dfb37-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dfb37-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="dfb37-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfb37-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="dfb37-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfb37-111">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="dfb37-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfb37-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfb37-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfb37-113">Not supported.</span></span> |
| <span data-ttu-id="dfb37-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dfb37-114">Application</span></span>                            | <span data-ttu-id="dfb37-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfb37-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfb37-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfb37-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="dfb37-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfb37-117">Request headers</span></span>

| <span data-ttu-id="dfb37-118">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dfb37-118">Header</span></span>         | <span data-ttu-id="dfb37-119">Valor</span><span class="sxs-lookup"><span data-stu-id="dfb37-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="dfb37-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfb37-120">Authorization</span></span>  | <span data-ttu-id="dfb37-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfb37-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="dfb37-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfb37-123">Request body</span></span>
<span data-ttu-id="dfb37-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dfb37-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfb37-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfb37-125">Response</span></span>
<span data-ttu-id="dfb37-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfb37-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dfb37-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dfb37-128">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="dfb37-129">Exemplo 1: remover um usuário da lista de remetentes rejeitados do grupo.</span><span class="sxs-lookup"><span data-stu-id="dfb37-129">Example 1: Remove a user from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="dfb37-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfb37-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_user_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}
```
#### <a name="response"></a><span data-ttu-id="dfb37-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfb37-131">Response</span></span>
<span data-ttu-id="dfb37-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dfb37-132">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dfb37-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="dfb37-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dfb37-134">Basic</span><span class="sxs-lookup"><span data-stu-id="dfb37-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/remove_user_from_rejectedsenderslist_of_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfb37-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfb37-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/remove_user_from_rejectedsenderslist_of_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="example-2-remove-a-group-from-the-rejected-senders-list-of-the-group"></a><span data-ttu-id="dfb37-136">Exemplo 2: remover um grupo da lista de remetentes rejeitados do grupo.</span><span class="sxs-lookup"><span data-stu-id="dfb37-136">Example 2: Remove a group from the rejected-senders list of the group.</span></span>
#### <a name="request"></a><span data-ttu-id="dfb37-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfb37-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "remove_group_from_rejectedsenderslist_of_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```

#### <a name="response"></a><span data-ttu-id="dfb37-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfb37-138">Response</span></span>
<span data-ttu-id="dfb37-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dfb37-139">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="dfb37-140">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="dfb37-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="dfb37-141">Basic</span><span class="sxs-lookup"><span data-stu-id="dfb37-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/remove_group_from_rejectedsenderslist_of_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfb37-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfb37-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/remove_group_from_rejectedsenderslist_of_group-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-delete-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
