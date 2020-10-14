---
title: Excluir delegatedPermissionClassification
description: Excluir uma classificação de permissão delegada da entidade de serviço de uma API.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 42ea2d19c8bdc98fb51bb6bb1978e98f276012fe
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458595"
---
# <a name="delete-delegatedpermissionclassification"></a><span data-ttu-id="eb6a5-103">Excluir delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="eb6a5-103">Delete delegatedPermissionClassification</span></span>

<span data-ttu-id="eb6a5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb6a5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb6a5-105">Exclui um [delegatedPermissionClassification](../resources/delegatedPermissionClassification.md) que tinha sido definido anteriormente para uma permissão delegada.</span><span class="sxs-lookup"><span data-stu-id="eb6a5-105">Deletes a [delegatedPermissionClassification](../resources/delegatedPermissionClassification.md) which had previously been set for a delegated permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb6a5-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb6a5-106">Permissions</span></span>

<span data-ttu-id="eb6a5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb6a5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb6a5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb6a5-109">Permission type</span></span>      | <span data-ttu-id="eb6a5-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb6a5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb6a5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb6a5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eb6a5-112">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="eb6a5-112">PermissionGrantPolicy.ReadWrite.All</span></span> |
|<span data-ttu-id="eb6a5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb6a5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb6a5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb6a5-114">Not supported.</span></span>    |
|<span data-ttu-id="eb6a5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb6a5-115">Application</span></span> | <span data-ttu-id="eb6a5-116">PermissionGrantPolicy. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="eb6a5-116">PermissionGrantPolicy.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb6a5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb6a5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```

## <a name="request-headers"></a><span data-ttu-id="eb6a5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb6a5-118">Request headers</span></span>

| <span data-ttu-id="eb6a5-119">Nome</span><span class="sxs-lookup"><span data-stu-id="eb6a5-119">Name</span></span>       | <span data-ttu-id="eb6a5-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb6a5-120">Type</span></span> | <span data-ttu-id="eb6a5-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb6a5-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eb6a5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb6a5-122">Authorization</span></span>  | <span data-ttu-id="eb6a5-123">string</span><span class="sxs-lookup"><span data-stu-id="eb6a5-123">string</span></span>  | <span data-ttu-id="eb6a5-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb6a5-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eb6a5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb6a5-126">Request body</span></span>

<span data-ttu-id="eb6a5-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb6a5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb6a5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb6a5-128">Response</span></span>

<span data-ttu-id="eb6a5-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb6a5-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="eb6a5-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="eb6a5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="eb6a5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb6a5-132">Request</span></span>

<span data-ttu-id="eb6a5-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb6a5-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="eb6a5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="eb6a5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_delete_delegatedpermissionclassifications"
}-->

```http
DELETE https://graph.microsoft.com/beta/servicePrincipals/{id}/delegatedPermissionClassifications/{id}
```
# <a name="c"></a>[<span data-ttu-id="eb6a5-135">C#</span><span class="sxs-lookup"><span data-stu-id="eb6a5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipal-delete-delegatedpermissionclassifications-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eb6a5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb6a5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipal-delete-delegatedpermissionclassifications-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eb6a5-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eb6a5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipal-delete-delegatedpermissionclassifications-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="eb6a5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb6a5-138">Response</span></span>

<span data-ttu-id="eb6a5-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="eb6a5-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
