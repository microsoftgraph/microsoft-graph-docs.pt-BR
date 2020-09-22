---
title: Criar claimsMappingPolicy
description: Criar um novo claimsMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 24ac7bd004e22e080509c6ac594800efa4a8913c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982511"
---
# <a name="create-claimsmappingpolicy"></a><span data-ttu-id="77c0e-103">Criar claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="77c0e-103">Create claimsMappingPolicy</span></span>

<span data-ttu-id="77c0e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77c0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77c0e-105">Criar um novo objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="77c0e-105">Create a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="77c0e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="77c0e-106">Permissions</span></span>

<span data-ttu-id="77c0e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77c0e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="77c0e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77c0e-109">Permission type</span></span>                        | <span data-ttu-id="77c0e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77c0e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="77c0e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77c0e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="77c0e-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="77c0e-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="77c0e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77c0e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77c0e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77c0e-114">Not supported.</span></span> |
| <span data-ttu-id="77c0e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77c0e-115">Application</span></span>                            | <span data-ttu-id="77c0e-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="77c0e-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="77c0e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77c0e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="77c0e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77c0e-118">Request headers</span></span>

| <span data-ttu-id="77c0e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="77c0e-119">Name</span></span>          | <span data-ttu-id="77c0e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="77c0e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="77c0e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="77c0e-121">Authorization</span></span> | <span data-ttu-id="77c0e-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="77c0e-122">Bearer {token}</span></span> |
| <span data-ttu-id="77c0e-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="77c0e-123">Content-type</span></span> | <span data-ttu-id="77c0e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="77c0e-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="77c0e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77c0e-125">Request body</span></span>

<span data-ttu-id="77c0e-126">No corpo da solicitação, forneça uma representação JSON do objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="77c0e-126">In the request body, supply a JSON representation of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="77c0e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="77c0e-127">Response</span></span>

<span data-ttu-id="77c0e-128">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77c0e-128">If successful, this method returns a `201 Created` response code and a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="77c0e-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="77c0e-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="77c0e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77c0e-130">Request</span></span>

<span data-ttu-id="77c0e-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="77c0e-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="77c0e-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="77c0e-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_claimsmappingpolicy_from_claimsmappingpolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/claimsMappingPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="77c0e-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77c0e-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-claimsmappingpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="77c0e-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="77c0e-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-claimsmappingpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="77c0e-135">C#</span><span class="sxs-lookup"><span data-stu-id="77c0e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-claimsmappingpolicy-from-claimsmappingpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="77c0e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="77c0e-136">Response</span></span>

<span data-ttu-id="77c0e-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="77c0e-137">The following is an example of the response.</span></span>

> <span data-ttu-id="77c0e-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77c0e-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create claimsMappingPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


