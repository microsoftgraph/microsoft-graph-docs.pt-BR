---
title: Criar claimsMappingPolicy
description: Criar um novo claimsMappingPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b59d8682c72058eb63be4dd71fd519b48a6f3703
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42438103"
---
# <a name="create-claimsmappingpolicy"></a><span data-ttu-id="8782f-103">Criar claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="8782f-103">Create claimsMappingPolicy</span></span>

<span data-ttu-id="8782f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8782f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8782f-105">Criar um novo objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8782f-105">Create a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8782f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8782f-106">Permissions</span></span>

<span data-ttu-id="8782f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8782f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8782f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8782f-109">Permission type</span></span>                        | <span data-ttu-id="8782f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8782f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8782f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8782f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8782f-112">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8782f-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="8782f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8782f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8782f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8782f-114">Not supported.</span></span> |
| <span data-ttu-id="8782f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8782f-115">Application</span></span>                            | <span data-ttu-id="8782f-116">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8782f-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="8782f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8782f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="8782f-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8782f-118">Request headers</span></span>

| <span data-ttu-id="8782f-119">Nome</span><span class="sxs-lookup"><span data-stu-id="8782f-119">Name</span></span>          | <span data-ttu-id="8782f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="8782f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8782f-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="8782f-121">Authorization</span></span> | <span data-ttu-id="8782f-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="8782f-122">Bearer {token}</span></span> |
| <span data-ttu-id="8782f-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="8782f-123">Content-type</span></span> | <span data-ttu-id="8782f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8782f-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8782f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8782f-125">Request body</span></span>

<span data-ttu-id="8782f-126">No corpo da solicitação, forneça uma representação JSON do objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="8782f-126">In the request body, supply a JSON representation of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8782f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8782f-127">Response</span></span>

<span data-ttu-id="8782f-128">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8782f-128">If successful, this method returns a `201 Created` response code and a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8782f-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8782f-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8782f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8782f-130">Request</span></span>

<span data-ttu-id="8782f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8782f-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8782f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8782f-132">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="8782f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8782f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-claimsmappingpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8782f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8782f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-claimsmappingpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8782f-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8782f-135">Response</span></span>

<span data-ttu-id="8782f-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8782f-136">The following is an example of the response.</span></span>

> <span data-ttu-id="8782f-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8782f-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
