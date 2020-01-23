---
title: Criar claimsMappingPolicy
description: Criar um novo claimsMappingPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: badb0bc304d4fa41a4826e7b166308dd80e148c3
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476333"
---
# <a name="create-claimsmappingpolicy"></a><span data-ttu-id="5edc9-103">Criar claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="5edc9-103">Create claimsMappingPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5edc9-104">Criar um novo objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="5edc9-104">Create a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5edc9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="5edc9-105">Permissions</span></span>

<span data-ttu-id="5edc9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5edc9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5edc9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5edc9-108">Permission type</span></span>                        | <span data-ttu-id="5edc9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5edc9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5edc9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5edc9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5edc9-111">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="5edc9-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="5edc9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5edc9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5edc9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5edc9-113">Not supported.</span></span> |
| <span data-ttu-id="5edc9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5edc9-114">Application</span></span>                            | <span data-ttu-id="5edc9-115">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="5edc9-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="5edc9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5edc9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="5edc9-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5edc9-117">Request headers</span></span>

| <span data-ttu-id="5edc9-118">Nome</span><span class="sxs-lookup"><span data-stu-id="5edc9-118">Name</span></span>          | <span data-ttu-id="5edc9-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="5edc9-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5edc9-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="5edc9-120">Authorization</span></span> | <span data-ttu-id="5edc9-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="5edc9-121">Bearer {token}</span></span> |
| <span data-ttu-id="5edc9-122">Content-type</span><span class="sxs-lookup"><span data-stu-id="5edc9-122">Content-type</span></span> | <span data-ttu-id="5edc9-123">application/json</span><span class="sxs-lookup"><span data-stu-id="5edc9-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5edc9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5edc9-124">Request body</span></span>

<span data-ttu-id="5edc9-125">No corpo da solicitação, forneça uma representação JSON do objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="5edc9-125">In the request body, supply a JSON representation of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5edc9-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="5edc9-126">Response</span></span>

<span data-ttu-id="5edc9-127">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5edc9-127">If successful, this method returns a `201 Created` response code and a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5edc9-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5edc9-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5edc9-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5edc9-129">Request</span></span>

<span data-ttu-id="5edc9-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5edc9-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5edc9-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="5edc9-131">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5edc9-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5edc9-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-claimsmappingpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5edc9-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5edc9-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-claimsmappingpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5edc9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5edc9-134">Response</span></span>

<span data-ttu-id="5edc9-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5edc9-135">The following is an example of the response.</span></span>

> <span data-ttu-id="5edc9-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5edc9-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
