---
title: Criar claimsMappingPolicy
description: Criar um novo claimsMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7d4e96ab4f746d24ad436f1c63568533e9c38790
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846195"
---
# <a name="create-claimsmappingpolicy"></a><span data-ttu-id="4eea9-103">Criar claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="4eea9-103">Create claimsMappingPolicy</span></span>

<span data-ttu-id="4eea9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4eea9-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4eea9-105">Criar um novo objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="4eea9-105">Create a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4eea9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4eea9-106">Permissions</span></span>

<span data-ttu-id="4eea9-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="4eea9-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="4eea9-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4eea9-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4eea9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4eea9-109">Permission type</span></span>                        | <span data-ttu-id="4eea9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4eea9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4eea9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4eea9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4eea9-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="4eea9-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="4eea9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4eea9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4eea9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4eea9-114">Not supported.</span></span> |
| <span data-ttu-id="4eea9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4eea9-115">Application</span></span>                            | <span data-ttu-id="4eea9-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="4eea9-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="4eea9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4eea9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="4eea9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4eea9-118">Request headers</span></span>

| <span data-ttu-id="4eea9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4eea9-119">Name</span></span>          | <span data-ttu-id="4eea9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="4eea9-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="4eea9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4eea9-121">Authorization</span></span> | <span data-ttu-id="4eea9-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="4eea9-122">Bearer {token}</span></span> |
| <span data-ttu-id="4eea9-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="4eea9-123">Content-type</span></span> | <span data-ttu-id="4eea9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4eea9-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4eea9-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4eea9-125">Request body</span></span>

<span data-ttu-id="4eea9-126">No corpo da solicitação, forneça uma representação JSON do objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="4eea9-126">In the request body, supply a JSON representation of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4eea9-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4eea9-127">Response</span></span>

<span data-ttu-id="4eea9-128">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4eea9-128">If successful, this method returns a `201 Created` response code and a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4eea9-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="4eea9-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4eea9-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4eea9-130">Request</span></span>

<span data-ttu-id="4eea9-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4eea9-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4eea9-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4eea9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_claimsmappingpolicy_from_claimsmappingpolicies"
}-->

```http
POST https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```

### <a name="response"></a><span data-ttu-id="4eea9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="4eea9-133">Response</span></span>

<span data-ttu-id="4eea9-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4eea9-134">The following is an example of the response.</span></span>

> <span data-ttu-id="4eea9-135">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="4eea9-135">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4eea9-136">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="4eea9-136">All the properties will be returned from an actual call.</span></span>

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
