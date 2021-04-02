---
title: Excluir featureRolloutPolicy
description: Exclua um objeto featureRolloutPolicy.
localization_priority: Normal
author: madhavpatel6
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: fc776712a60dd4beaafb2e9ca38391fdf73a0c10
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508894"
---
# <a name="delete-featurerolloutpolicy"></a><span data-ttu-id="42aff-103">Excluir featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="42aff-103">Delete featureRolloutPolicy</span></span>

<span data-ttu-id="42aff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42aff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42aff-105">[Exclua um objeto featureRolloutPolicy.](../resources/featurerolloutpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="42aff-105">Delete a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="42aff-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="42aff-106">Permissions</span></span>

<span data-ttu-id="42aff-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="42aff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="42aff-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="42aff-109">Permission type</span></span>                        | <span data-ttu-id="42aff-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="42aff-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="42aff-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="42aff-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="42aff-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="42aff-112">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="42aff-113">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="42aff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="42aff-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42aff-114">Not supported.</span></span> |
| <span data-ttu-id="42aff-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="42aff-115">Application</span></span>                            | <span data-ttu-id="42aff-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="42aff-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="42aff-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="42aff-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="42aff-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="42aff-118">Request headers</span></span>

| <span data-ttu-id="42aff-119">Nome</span><span class="sxs-lookup"><span data-stu-id="42aff-119">Name</span></span>          | <span data-ttu-id="42aff-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="42aff-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="42aff-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="42aff-121">Authorization</span></span> | <span data-ttu-id="42aff-122">Portador {token}.</span><span class="sxs-lookup"><span data-stu-id="42aff-122">Bearer {token}.</span></span> <span data-ttu-id="42aff-123">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="42aff-123">Required</span></span> |

## <a name="request-body"></a><span data-ttu-id="42aff-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="42aff-124">Request body</span></span>

<span data-ttu-id="42aff-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="42aff-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="42aff-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="42aff-126">Response</span></span>

<span data-ttu-id="42aff-p103">Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="42aff-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="42aff-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="42aff-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="42aff-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="42aff-130">Request</span></span>

<span data-ttu-id="42aff-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="42aff-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="42aff-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="42aff-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy_policies"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="c"></a>[<span data-ttu-id="42aff-133">C#</span><span class="sxs-lookup"><span data-stu-id="42aff-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-featurerolloutpolicy-policies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="42aff-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="42aff-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-featurerolloutpolicy-policies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="42aff-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="42aff-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-featurerolloutpolicy-policies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="42aff-136">Java</span><span class="sxs-lookup"><span data-stu-id="42aff-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-featurerolloutpolicy-policies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="42aff-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="42aff-137">Response</span></span>

<span data-ttu-id="42aff-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="42aff-138">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


