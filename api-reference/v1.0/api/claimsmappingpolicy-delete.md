---
title: Excluir claimsMappingPolicy
description: Exclua claimsMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4ff68292b6140f3c0175f28adecacb68e18a0cc2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966251"
---
# <a name="delete-claimsmappingpolicy"></a><span data-ttu-id="ed44e-103">Excluir claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="ed44e-103">Delete claimsMappingPolicy</span></span>

<span data-ttu-id="ed44e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed44e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed44e-105">Excluir um objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ed44e-105">Delete a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed44e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ed44e-106">Permissions</span></span>

<span data-ttu-id="ed44e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ed44e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ed44e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ed44e-109">Permission type</span></span>                        | <span data-ttu-id="ed44e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ed44e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ed44e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ed44e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ed44e-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ed44e-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="ed44e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ed44e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed44e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ed44e-114">Not supported.</span></span> |
| <span data-ttu-id="ed44e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ed44e-115">Application</span></span>                            | <span data-ttu-id="ed44e-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ed44e-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed44e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ed44e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ed44e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ed44e-118">Request headers</span></span>

| <span data-ttu-id="ed44e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ed44e-119">Name</span></span>          | <span data-ttu-id="ed44e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed44e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ed44e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ed44e-121">Authorization</span></span> | <span data-ttu-id="ed44e-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ed44e-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed44e-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ed44e-123">Request body</span></span>

<span data-ttu-id="ed44e-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ed44e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed44e-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed44e-125">Response</span></span>

<span data-ttu-id="ed44e-126">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ed44e-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ed44e-127">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ed44e-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed44e-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ed44e-128">Request</span></span>

<span data-ttu-id="ed44e-129">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ed44e-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ed44e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed44e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="ed44e-131">C#</span><span class="sxs-lookup"><span data-stu-id="ed44e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed44e-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed44e-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed44e-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed44e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed44e-134">Java</span><span class="sxs-lookup"><span data-stu-id="ed44e-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-claimsmappingpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ed44e-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ed44e-135">Response</span></span>

<span data-ttu-id="ed44e-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ed44e-136">The following is an example of the response.</span></span>

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
  "description": "Delete claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

