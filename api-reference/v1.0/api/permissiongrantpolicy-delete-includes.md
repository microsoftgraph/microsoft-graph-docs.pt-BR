---
title: Excluir permissionGrantConditionSet de inclui coleção de permissionGrantPolicy
description: Exclui um conjunto de condições incluído da política de concessão de permissão.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 2c19e048428456e88fa0d9ce80879630044e7a71
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441701"
---
# <a name="delete-permissiongrantconditionset-from-includes-collection-of-permissiongrantpolicy"></a><span data-ttu-id="18aaa-103">Excluir permissionGrantConditionSet de inclui coleção de permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="18aaa-103">Delete permissionGrantConditionSet from includes collection of permissionGrantPolicy</span></span>

<span data-ttu-id="18aaa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18aaa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="18aaa-105">Exclui uma [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) da coleção **includes** de [uma permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="18aaa-105">Deletes a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) from the **includes** collection of a [permissionGrantPolicy](../resources/permissiongrantpolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="18aaa-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="18aaa-106">Permissions</span></span>

<span data-ttu-id="18aaa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="18aaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="18aaa-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="18aaa-109">Permission type</span></span>      | <span data-ttu-id="18aaa-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="18aaa-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="18aaa-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="18aaa-111">Delegated (work or school account)</span></span> | <span data-ttu-id="18aaa-112">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18aaa-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
| <span data-ttu-id="18aaa-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="18aaa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18aaa-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="18aaa-114">Not supported.</span></span>    |
| <span data-ttu-id="18aaa-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="18aaa-115">Application</span></span> | <span data-ttu-id="18aaa-116">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18aaa-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18aaa-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="18aaa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{permissiongrantpolicy-id}/includes/{include-id}
```

## <a name="request-headers"></a><span data-ttu-id="18aaa-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="18aaa-118">Request headers</span></span>

| <span data-ttu-id="18aaa-119">Nome</span><span class="sxs-lookup"><span data-stu-id="18aaa-119">Name</span></span>       | <span data-ttu-id="18aaa-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="18aaa-120">Type</span></span> | <span data-ttu-id="18aaa-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="18aaa-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="18aaa-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="18aaa-122">Authorization</span></span>  | <span data-ttu-id="18aaa-123">string</span><span class="sxs-lookup"><span data-stu-id="18aaa-123">string</span></span>  | <span data-ttu-id="18aaa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="18aaa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18aaa-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="18aaa-126">Request body</span></span>

<span data-ttu-id="18aaa-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="18aaa-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18aaa-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="18aaa-128">Response</span></span>

<span data-ttu-id="18aaa-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="18aaa-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="18aaa-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="18aaa-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="18aaa-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="18aaa-132">Request</span></span>

<span data-ttu-id="18aaa-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="18aaa-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="18aaa-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="18aaa-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "permissiongrantpolicy_delete_includes"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/permissionGrantPolicies/my-custom-consent-policy/includes/198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5
```
# <a name="c"></a>[<span data-ttu-id="18aaa-135">C#</span><span class="sxs-lookup"><span data-stu-id="18aaa-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permissiongrantpolicy-delete-includes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18aaa-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18aaa-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permissiongrantpolicy-delete-includes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18aaa-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18aaa-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permissiongrantpolicy-delete-includes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18aaa-138">Java</span><span class="sxs-lookup"><span data-stu-id="18aaa-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permissiongrantpolicy-delete-includes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="18aaa-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="18aaa-139">Response</span></span>

<span data-ttu-id="18aaa-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="18aaa-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
