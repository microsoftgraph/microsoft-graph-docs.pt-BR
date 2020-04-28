---
title: Criar claimsMappingPolicy
description: Criar um novo claimsMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8fa07178f6c485a98353c7b5718b0b0c9173f84f
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916499"
---
# <a name="create-claimsmappingpolicy"></a><span data-ttu-id="d3c18-103">Criar claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="d3c18-103">Create claimsMappingPolicy</span></span>

<span data-ttu-id="d3c18-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3c18-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3c18-105">Criar um novo objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="d3c18-105">Create a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3c18-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d3c18-106">Permissions</span></span>

<span data-ttu-id="d3c18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3c18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d3c18-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d3c18-109">Permission type</span></span>                        | <span data-ttu-id="d3c18-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d3c18-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d3c18-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d3c18-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d3c18-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="d3c18-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="d3c18-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d3c18-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3c18-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d3c18-114">Not supported.</span></span> |
| <span data-ttu-id="d3c18-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d3c18-115">Application</span></span>                            | <span data-ttu-id="d3c18-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="d3c18-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="d3c18-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d3c18-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="d3c18-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3c18-118">Request headers</span></span>

| <span data-ttu-id="d3c18-119">Nome</span><span class="sxs-lookup"><span data-stu-id="d3c18-119">Name</span></span>          | <span data-ttu-id="d3c18-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3c18-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d3c18-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="d3c18-121">Authorization</span></span> | <span data-ttu-id="d3c18-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="d3c18-122">Bearer {token}</span></span> |
| <span data-ttu-id="d3c18-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="d3c18-123">Content-type</span></span> | <span data-ttu-id="d3c18-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d3c18-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d3c18-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d3c18-125">Request body</span></span>

<span data-ttu-id="d3c18-126">No corpo da solicitação, forneça uma representação JSON do objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="d3c18-126">In the request body, supply a JSON representation of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d3c18-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3c18-127">Response</span></span>

<span data-ttu-id="d3c18-128">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d3c18-128">If successful, this method returns a `201 Created` response code and a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d3c18-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d3c18-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d3c18-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d3c18-130">Request</span></span>

<span data-ttu-id="d3c18-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d3c18-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d3c18-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3c18-132">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="d3c18-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3c18-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-claimsmappingpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d3c18-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3c18-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-claimsmappingpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="d3c18-135">C#</span><span class="sxs-lookup"><span data-stu-id="d3c18-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-claimsmappingpolicy-from-claimsmappingpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d3c18-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d3c18-136">Response</span></span>

<span data-ttu-id="d3c18-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d3c18-137">The following is an example of the response.</span></span>

> <span data-ttu-id="d3c18-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d3c18-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
