---
title: Excluir permissionGrantConditionSet de exclui coleção de permissionGrantPolicy
description: Exclui um conjunto de condições excluído da política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 9215ee6d935f19581fbe855f50635f5dc0bd5c98
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447677"
---
# <a name="delete-permissiongrantconditionset-from-excludes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="f5714-103">Excluir permissionGrantConditionSet de exclui coleção de permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="f5714-103">Delete permissionGrantConditionSet from excludes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="f5714-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5714-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5714-105">Exclui um [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) da coleção **excludes** de [uma permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="f5714-105">Deletes a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) from the **excludes** collection of a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f5714-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5714-106">Permissions</span></span>

<span data-ttu-id="f5714-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5714-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f5714-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5714-109">Permission type</span></span>      | <span data-ttu-id="f5714-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5714-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="f5714-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5714-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f5714-112">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5714-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
| <span data-ttu-id="f5714-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5714-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5714-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5714-114">Not supported.</span></span>    |
| <span data-ttu-id="f5714-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5714-115">Application</span></span> | <span data-ttu-id="f5714-116">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5714-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5714-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5714-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/excludes/{exclude-id}
```

## <a name="request-headers"></a><span data-ttu-id="f5714-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5714-118">Request headers</span></span>

| <span data-ttu-id="f5714-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f5714-119">Name</span></span>       | <span data-ttu-id="f5714-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5714-120">Type</span></span> | <span data-ttu-id="f5714-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5714-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f5714-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5714-122">Authorization</span></span>  | <span data-ttu-id="f5714-123">string</span><span class="sxs-lookup"><span data-stu-id="f5714-123">string</span></span>  | <span data-ttu-id="f5714-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5714-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5714-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5714-126">Request body</span></span>

<span data-ttu-id="f5714-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f5714-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5714-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5714-128">Response</span></span>

<span data-ttu-id="f5714-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5714-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f5714-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f5714-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f5714-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5714-132">Request</span></span>

<span data-ttu-id="f5714-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5714-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f5714-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="f5714-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_excludes"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy/excludes/6a846635-3e70-4a10-821e-512a0db93cbd
```
# <a name="c"></a>[<span data-ttu-id="f5714-135">C#</span><span class="sxs-lookup"><span data-stu-id="f5714-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-delete-excludes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f5714-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f5714-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-delete-excludes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f5714-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f5714-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-delete-excludes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f5714-138">Java</span><span class="sxs-lookup"><span data-stu-id="f5714-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-delete-excludes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f5714-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5714-139">Response</span></span>

<span data-ttu-id="f5714-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f5714-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
