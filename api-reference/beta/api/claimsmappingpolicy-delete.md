---
title: Excluir claimsMappingPolicy
description: Exclua claimsMappingPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0cf08fd80528bf521ee0951a61d1d6e9caf28805
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476277"
---
# <a name="delete-claimsmappingpolicy"></a><span data-ttu-id="ba790-103">Excluir claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="ba790-103">Delete claimsMappingPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba790-104">Excluir um objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="ba790-104">Delete a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba790-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ba790-105">Permissions</span></span>

<span data-ttu-id="ba790-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba790-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ba790-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba790-108">Permission type</span></span>                        | <span data-ttu-id="ba790-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ba790-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ba790-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba790-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ba790-111">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba790-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="ba790-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba790-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba790-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba790-113">Not supported.</span></span> |
| <span data-ttu-id="ba790-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba790-114">Application</span></span>                            | <span data-ttu-id="ba790-115">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="ba790-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba790-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba790-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/claimsMappingPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ba790-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba790-117">Request headers</span></span>

| <span data-ttu-id="ba790-118">Nome</span><span class="sxs-lookup"><span data-stu-id="ba790-118">Name</span></span>          | <span data-ttu-id="ba790-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba790-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ba790-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba790-120">Authorization</span></span> | <span data-ttu-id="ba790-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="ba790-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba790-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba790-122">Request body</span></span>

<span data-ttu-id="ba790-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ba790-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba790-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba790-124">Response</span></span>

<span data-ttu-id="ba790-125">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ba790-125">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ba790-126">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ba790-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ba790-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba790-127">Request</span></span>

<span data-ttu-id="ba790-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba790-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ba790-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba790-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_claimsmappingpolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/claimsMappingPolicies/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ba790-130">C#</span><span class="sxs-lookup"><span data-stu-id="ba790-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-claimsmappingpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ba790-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ba790-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-claimsmappingpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ba790-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ba790-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-claimsmappingpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ba790-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba790-133">Response</span></span>

<span data-ttu-id="ba790-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ba790-134">The following is an example of the response.</span></span>

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
