---
title: Excluir groupLifecyclePolicy
description: Exclui um objeto groupLifecyclePolicy.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: ae3d415f04803dd197a8da666612c65eed77be8b
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613494"
---
# <a name="delete-grouplifecyclepolicy"></a><span data-ttu-id="24131-103">Excluir groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="24131-103">Delete groupLifecyclePolicy</span></span>

<span data-ttu-id="24131-104">Exclui um objeto [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span><span class="sxs-lookup"><span data-stu-id="24131-104">Deletes a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="24131-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="24131-105">Permissions</span></span>

<span data-ttu-id="24131-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24131-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24131-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24131-108">Permission type</span></span>      | <span data-ttu-id="24131-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24131-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24131-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24131-110">Delegated (work or school account)</span></span> | <span data-ttu-id="24131-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24131-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="24131-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24131-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24131-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24131-113">Not supported.</span></span>    |
|<span data-ttu-id="24131-114">Application</span><span class="sxs-lookup"><span data-stu-id="24131-114">Application</span></span> | <span data-ttu-id="24131-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24131-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="24131-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24131-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groupLifecyclePolicies/{id}

```

## <a name="request-headers"></a><span data-ttu-id="24131-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24131-117">Request headers</span></span>

| <span data-ttu-id="24131-118">Nome</span><span class="sxs-lookup"><span data-stu-id="24131-118">Name</span></span> | <span data-ttu-id="24131-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="24131-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="24131-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="24131-120">Authorization</span></span> | <span data-ttu-id="24131-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24131-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="24131-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="24131-123">Content-Type</span></span>  | <span data-ttu-id="24131-124">application/json</span><span class="sxs-lookup"><span data-stu-id="24131-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="24131-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24131-125">Request body</span></span>
<span data-ttu-id="24131-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24131-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="24131-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="24131-127">Response</span></span>

<span data-ttu-id="24131-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24131-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24131-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24131-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="24131-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24131-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_grouplifecyclepolicy"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groupLifecyclePolicies/{id}
```
##### <a name="response"></a><span data-ttu-id="24131-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="24131-132">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="24131-133">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="24131-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="24131-134">Basic</span><span class="sxs-lookup"><span data-stu-id="24131-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_grouplifecyclepolicy-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24131-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24131-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_grouplifecyclepolicy-Javascript-snippets.md)]

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
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
