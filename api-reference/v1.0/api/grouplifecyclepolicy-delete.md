---
title: Excluir groupLifecyclePolicy
description: Exclui um objeto groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 8d243fe1e3b61f114b4a06af354922a0f49c44ed
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263550"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="4d2fd-103">Excluir groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="4d2fd-103">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="4d2fd-104">Exclui um objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="4d2fd-104">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4d2fd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4d2fd-105">Permissions</span></span>

<span data-ttu-id="4d2fd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4d2fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4d2fd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4d2fd-108">Permission type</span></span>      | <span data-ttu-id="4d2fd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4d2fd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d2fd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4d2fd-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4d2fd-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d2fd-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="4d2fd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4d2fd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d2fd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4d2fd-113">Not supported.</span></span>    |
|<span data-ttu-id="4d2fd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4d2fd-114">Application</span></span> | <span data-ttu-id="4d2fd-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d2fd-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d2fd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4d2fd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="4d2fd-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4d2fd-117">Request headers</span></span>

| <span data-ttu-id="4d2fd-118">Nome</span><span class="sxs-lookup"><span data-stu-id="4d2fd-118">Name</span></span> | <span data-ttu-id="4d2fd-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d2fd-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="4d2fd-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="4d2fd-120">Authorization</span></span> | <span data-ttu-id="4d2fd-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4d2fd-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d2fd-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4d2fd-123">Content-Type</span></span>  | <span data-ttu-id="4d2fd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4d2fd-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d2fd-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4d2fd-125">Request body</span></span>
<span data-ttu-id="4d2fd-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4d2fd-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="4d2fd-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d2fd-127">Response</span></span>

<span data-ttu-id="4d2fd-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4d2fd-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4d2fd-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4d2fd-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4d2fd-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4d2fd-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="4d2fd-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="4d2fd-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="4d2fd-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="4d2fd-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="4d2fd-134">C#</span><span class="sxs-lookup"><span data-stu-id="4d2fd-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_grouplifecyclepolicy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4d2fd-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="4d2fd-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_grouplifecyclepolicy-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="4d2fd-136">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="4d2fd-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_grouplifecyclepolicy-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
