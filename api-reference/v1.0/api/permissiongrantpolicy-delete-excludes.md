---
title: Excluir permissionGrantConditionSet da coleção Excludes de permissionGrantPolicy
description: Exclui um conjunto de condições excluídas da política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 745e42b4d236177febe3486ba1dfcbf427fe27bd
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524377"
---
# <a name="delete-permissiongrantconditionset-from-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="272a7-103">Excluir permissionGrantConditionSet da coleção Excludes de permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="272a7-103">Delete permissionGrantConditionSet from excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="272a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="272a7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="272a7-105">Exclui [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) da coleção **Excludes** de um [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="272a7-105">Deletes a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) from the **excludes** collection of a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="272a7-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="272a7-106">Permissions</span></span>

<span data-ttu-id="272a7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="272a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="272a7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="272a7-109">Permission type</span></span>      | <span data-ttu-id="272a7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="272a7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="272a7-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="272a7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="272a7-112">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="272a7-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
| <span data-ttu-id="272a7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="272a7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="272a7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="272a7-114">Not supported.</span></span>    |
| <span data-ttu-id="272a7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="272a7-115">Application</span></span> | <span data-ttu-id="272a7-116">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="272a7-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="272a7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="272a7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/excludes/{exclude-id}
```

## <a name="request-headers"></a><span data-ttu-id="272a7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="272a7-118">Request headers</span></span>

| <span data-ttu-id="272a7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="272a7-119">Name</span></span>       | <span data-ttu-id="272a7-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="272a7-120">Type</span></span> | <span data-ttu-id="272a7-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="272a7-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="272a7-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="272a7-122">Authorization</span></span>  | <span data-ttu-id="272a7-123">string</span><span class="sxs-lookup"><span data-stu-id="272a7-123">string</span></span>  | <span data-ttu-id="272a7-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="272a7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="272a7-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="272a7-126">Request body</span></span>

<span data-ttu-id="272a7-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="272a7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="272a7-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="272a7-128">Response</span></span>

<span data-ttu-id="272a7-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="272a7-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="272a7-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="272a7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="272a7-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="272a7-132">Request</span></span>

<span data-ttu-id="272a7-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="272a7-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="272a7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="272a7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_excludes"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy/excludes/6a846635-3e70-4a10-821e-512a0db93cbd
```
# <a name="c"></a>[<span data-ttu-id="272a7-135">C#</span><span class="sxs-lookup"><span data-stu-id="272a7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-delete-excludes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="272a7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="272a7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-delete-excludes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="272a7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="272a7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-delete-excludes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="272a7-138">Java</span><span class="sxs-lookup"><span data-stu-id="272a7-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-delete-excludes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="272a7-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="272a7-139">Response</span></span>

<span data-ttu-id="272a7-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="272a7-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
