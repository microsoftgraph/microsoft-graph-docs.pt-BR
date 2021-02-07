---
title: Excluir delegatedPermissionClassification
description: Exclua uma classificação de permissão delegada da entidade de serviço de uma API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: decce0d0a9e3f6915676cb7151da0d43ddff3067
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133095"
---
# <a name="delete-delegatedpermissionclassification"></a><span data-ttu-id="14ccf-103">Excluir delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="14ccf-103">Delete delegatedPermissionClassification</span></span>

<span data-ttu-id="14ccf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14ccf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="14ccf-105">Exclui um [delegatedPermissionClassification](../resources/delegatedPermissionClassification.md) que foi definido anteriormente para uma permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="14ccf-105">Deletes a [delegatedPermissionClassification](../resources/delegatedPermissionClassification.md) which had previously been set for a delegated permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="14ccf-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="14ccf-106">Permissions</span></span>

<span data-ttu-id="14ccf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14ccf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14ccf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="14ccf-109">Permission type</span></span>      | <span data-ttu-id="14ccf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="14ccf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="14ccf-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="14ccf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="14ccf-112">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14ccf-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="14ccf-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="14ccf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14ccf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="14ccf-114">Not supported.</span></span>    |
|<span data-ttu-id="14ccf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="14ccf-115">Application</span></span> | <span data-ttu-id="14ccf-116">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14ccf-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="14ccf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="14ccf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="14ccf-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="14ccf-118">Request headers</span></span>

| <span data-ttu-id="14ccf-119">Nome</span><span class="sxs-lookup"><span data-stu-id="14ccf-119">Name</span></span>       | <span data-ttu-id="14ccf-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="14ccf-120">Type</span></span> | <span data-ttu-id="14ccf-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="14ccf-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="14ccf-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="14ccf-122">Authorization</span></span>  | <span data-ttu-id="14ccf-123">string</span><span class="sxs-lookup"><span data-stu-id="14ccf-123">string</span></span>  | <span data-ttu-id="14ccf-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="14ccf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14ccf-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="14ccf-126">Request body</span></span>

<span data-ttu-id="14ccf-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="14ccf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="14ccf-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="14ccf-128">Response</span></span>

<span data-ttu-id="14ccf-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="14ccf-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="14ccf-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="14ccf-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="14ccf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="14ccf-132">Request</span></span>

<span data-ttu-id="14ccf-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="14ccf-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="14ccf-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="14ccf-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_delegatedpermissionclassifications"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```
# <a name="c"></a>[<span data-ttu-id="14ccf-135">C#</span><span class="sxs-lookup"><span data-stu-id="14ccf-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-delegatedpermissionclassifications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14ccf-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14ccf-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-delegatedpermissionclassifications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14ccf-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14ccf-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-delegatedpermissionclassifications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14ccf-138">Java</span><span class="sxs-lookup"><span data-stu-id="14ccf-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delete-delegatedpermissionclassifications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="14ccf-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="14ccf-139">Response</span></span>

<span data-ttu-id="14ccf-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="14ccf-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
