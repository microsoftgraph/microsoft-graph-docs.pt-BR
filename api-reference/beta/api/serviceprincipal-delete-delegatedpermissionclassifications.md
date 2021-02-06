---
title: Excluir delegatedPermissionClassification
description: Exclua uma classificação de permissão delegada da entidade de serviço de uma API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: aa10fbf12e0fef1ef6b8a96ec61cbb0571d47f8b
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137386"
---
# <a name="delete-delegatedpermissionclassification"></a><span data-ttu-id="dfcf1-103">Excluir delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="dfcf1-103">Delete delegatedPermissionClassification</span></span>

<span data-ttu-id="dfcf1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfcf1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfcf1-105">Exclui um [delegatedPermissionClassification](../resources/delegatedPermissionClassification.md) que foi definido anteriormente para uma permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="dfcf1-105">Deletes a [delegatedPermissionClassification](../resources/delegatedPermissionClassification.md) which had previously been set for a delegated permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="dfcf1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="dfcf1-106">Permissions</span></span>

<span data-ttu-id="dfcf1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dfcf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfcf1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dfcf1-109">Permission type</span></span>      | <span data-ttu-id="dfcf1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dfcf1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfcf1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dfcf1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dfcf1-112">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfcf1-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="dfcf1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dfcf1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfcf1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dfcf1-114">Not supported.</span></span>    |
|<span data-ttu-id="dfcf1-115">Application</span><span class="sxs-lookup"><span data-stu-id="dfcf1-115">Application</span></span> | <span data-ttu-id="dfcf1-116">PermissionGrantPolicy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfcf1-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfcf1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dfcf1-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="dfcf1-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dfcf1-118">Request headers</span></span>

| <span data-ttu-id="dfcf1-119">Nome</span><span class="sxs-lookup"><span data-stu-id="dfcf1-119">Name</span></span>       | <span data-ttu-id="dfcf1-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfcf1-120">Type</span></span> | <span data-ttu-id="dfcf1-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfcf1-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dfcf1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="dfcf1-122">Authorization</span></span>  | <span data-ttu-id="dfcf1-123">string</span><span class="sxs-lookup"><span data-stu-id="dfcf1-123">string</span></span>  | <span data-ttu-id="dfcf1-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dfcf1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dfcf1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dfcf1-126">Request body</span></span>

<span data-ttu-id="dfcf1-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dfcf1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfcf1-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfcf1-128">Response</span></span>

<span data-ttu-id="dfcf1-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dfcf1-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dfcf1-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="dfcf1-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dfcf1-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dfcf1-132">Request</span></span>

<span data-ttu-id="dfcf1-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dfcf1-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dfcf1-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfcf1-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_delegatedpermissionclassifications"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```
# <a name="c"></a>[<span data-ttu-id="dfcf1-135">C#</span><span class="sxs-lookup"><span data-stu-id="dfcf1-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-delegatedpermissionclassifications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfcf1-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfcf1-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-delegatedpermissionclassifications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfcf1-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfcf1-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-delegatedpermissionclassifications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dfcf1-138">Java</span><span class="sxs-lookup"><span data-stu-id="dfcf1-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/serviceprincipal-delete-delegatedpermissionclassifications-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dfcf1-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="dfcf1-139">Response</span></span>

<span data-ttu-id="dfcf1-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dfcf1-140">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

