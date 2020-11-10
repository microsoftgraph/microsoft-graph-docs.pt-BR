---
title: Excluir permissionGrantConditionSet da coleção Excludes de permissionGrantPolicy
description: Exclui um conjunto de condições excluídas da política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: fa922ebbe4c62e3015acb37a179b6c1d0c6ed6ab
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48977973"
---
# <a name="delete-permissiongrantconditionset-from-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="0477f-103">Excluir permissionGrantConditionSet da coleção Excludes de permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="0477f-103">Delete permissionGrantConditionSet from excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="0477f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0477f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0477f-105">Exclui [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) da coleção **Excludes** de um [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="0477f-105">Deletes a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) from the **excludes** collection of a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0477f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0477f-106">Permissions</span></span>

<span data-ttu-id="0477f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0477f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0477f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0477f-109">Permission type</span></span>      | <span data-ttu-id="0477f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0477f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="0477f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0477f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0477f-112">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0477f-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
| <span data-ttu-id="0477f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0477f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0477f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0477f-114">Not supported.</span></span>    |
| <span data-ttu-id="0477f-115">Application</span><span class="sxs-lookup"><span data-stu-id="0477f-115">Application</span></span> | <span data-ttu-id="0477f-116">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="0477f-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0477f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0477f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/excludes/{exclude-id}
```

## <a name="request-headers"></a><span data-ttu-id="0477f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0477f-118">Request headers</span></span>

| <span data-ttu-id="0477f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0477f-119">Name</span></span>       | <span data-ttu-id="0477f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0477f-120">Type</span></span> | <span data-ttu-id="0477f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0477f-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0477f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="0477f-122">Authorization</span></span>  | <span data-ttu-id="0477f-123">string</span><span class="sxs-lookup"><span data-stu-id="0477f-123">string</span></span>  | <span data-ttu-id="0477f-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0477f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0477f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0477f-126">Request body</span></span>

<span data-ttu-id="0477f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0477f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0477f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0477f-128">Response</span></span>

<span data-ttu-id="0477f-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0477f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0477f-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0477f-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0477f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0477f-132">Request</span></span>

<span data-ttu-id="0477f-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0477f-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0477f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0477f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_excludes"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy/excludes/6a846635-3e70-4a10-821e-512a0db93cbd
```
# <a name="c"></a>[<span data-ttu-id="0477f-135">C#</span><span class="sxs-lookup"><span data-stu-id="0477f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-delete-excludes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0477f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0477f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-delete-excludes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0477f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0477f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-delete-excludes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0477f-138">Java</span><span class="sxs-lookup"><span data-stu-id="0477f-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-delete-excludes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0477f-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="0477f-139">Response</span></span>

<span data-ttu-id="0477f-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0477f-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
