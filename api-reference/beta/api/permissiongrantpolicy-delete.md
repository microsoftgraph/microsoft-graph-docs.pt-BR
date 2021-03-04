---
title: Excluir permissionGrantPolicy
description: Exclua um objeto permissionGrantPolicy.
localization_priority: Normal
doc_type: apiPageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: a2e6791392330b8b2d2b59a61e2e5d84098dc9d8
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447681"
---
# <a name="delete-permissiongrantpolicy"></a><span data-ttu-id="3abf6-103">Excluir permissionGrantPolicy</span><span class="sxs-lookup"><span data-stu-id="3abf6-103">Delete permissionGrantPolicy</span></span>

<span data-ttu-id="3abf6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3abf6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3abf6-105">[Exclua um objeto permissionGrantPolicy.](../resources/permissiongrantpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3abf6-105">Delete a [permissionGrantPolicy](../resources/permissiongrantpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3abf6-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="3abf6-106">Permissions</span></span>

<span data-ttu-id="3abf6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3abf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3abf6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3abf6-109">Permission type</span></span>                        | <span data-ttu-id="3abf6-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3abf6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3abf6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3abf6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3abf6-112">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="3abf6-112">Policy.ReadWrite.PermissionGrant</span></span> |
| <span data-ttu-id="3abf6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3abf6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3abf6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3abf6-114">Not supported.</span></span> |
| <span data-ttu-id="3abf6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3abf6-115">Application</span></span>                            | <span data-ttu-id="3abf6-116">Policy.ReadWrite.PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="3abf6-116">Policy.ReadWrite.PermissionGrant</span></span> |

## <a name="http-request"></a><span data-ttu-id="3abf6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3abf6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/permissionGrantPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3abf6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3abf6-118">Request headers</span></span>

| <span data-ttu-id="3abf6-119">Nome</span><span class="sxs-lookup"><span data-stu-id="3abf6-119">Name</span></span>           | <span data-ttu-id="3abf6-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="3abf6-120">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="3abf6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="3abf6-121">Authorization</span></span>  | <span data-ttu-id="3abf6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3abf6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3abf6-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3abf6-124">Request body</span></span>

<span data-ttu-id="3abf6-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3abf6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3abf6-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3abf6-126">Response</span></span>

<span data-ttu-id="3abf6-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3abf6-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3abf6-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3abf6-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3abf6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3abf6-130">Request</span></span>

<span data-ttu-id="3abf6-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3abf6-131">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3abf6-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3abf6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_permissiongrantpolicy"
}-->

```msgraph-interactive
DELETE https://graph.microsoft.com/beta/policies/permissionGrantPolicies/my-custom-consent-policy
```
# <a name="c"></a>[<span data-ttu-id="3abf6-133">C#</span><span class="sxs-lookup"><span data-stu-id="3abf6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-permissiongrantpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3abf6-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3abf6-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-permissiongrantpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3abf6-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3abf6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-permissiongrantpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3abf6-136">Java</span><span class="sxs-lookup"><span data-stu-id="3abf6-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-permissiongrantpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3abf6-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="3abf6-137">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
