---
title: Criar claimsMappingPolicy
description: Criar um novo claimsMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1a1570e237c57f565c66afd0c921c31b6b8765f1
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863225"
---
# <a name="create-claimsmappingpolicy"></a><span data-ttu-id="0e966-103">Criar claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="0e966-103">Create claimsMappingPolicy</span></span>

<span data-ttu-id="0e966-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e966-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0e966-105">Criar um novo objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="0e966-105">Create a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e966-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="0e966-106">Permissions</span></span>

<span data-ttu-id="0e966-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="0e966-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="0e966-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e966-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0e966-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e966-109">Permission type</span></span>                        | <span data-ttu-id="0e966-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0e966-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0e966-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e966-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0e966-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e966-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="0e966-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e966-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e966-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e966-114">Not supported.</span></span> |
| <span data-ttu-id="0e966-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e966-115">Application</span></span>                            | <span data-ttu-id="0e966-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0e966-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e966-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e966-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="0e966-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e966-118">Request headers</span></span>

| <span data-ttu-id="0e966-119">Nome</span><span class="sxs-lookup"><span data-stu-id="0e966-119">Name</span></span>          | <span data-ttu-id="0e966-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e966-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0e966-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e966-121">Authorization</span></span> | <span data-ttu-id="0e966-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="0e966-122">Bearer {token}</span></span> |
| <span data-ttu-id="0e966-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="0e966-123">Content-type</span></span> | <span data-ttu-id="0e966-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0e966-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e966-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e966-125">Request body</span></span>

<span data-ttu-id="0e966-126">No corpo da solicitação, forneça uma representação JSON do objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="0e966-126">In the request body, supply a JSON representation of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0e966-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e966-127">Response</span></span>

<span data-ttu-id="0e966-128">Se tiver êxito, este método retornará um `201 Created` código de resposta e um novo objeto [claimsMappingPolicy](../resources/claimsmappingpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e966-128">If successful, this method returns a `201 Created` response code and a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0e966-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0e966-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0e966-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e966-130">Request</span></span>

<span data-ttu-id="0e966-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e966-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0e966-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="0e966-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="0e966-133">C#</span><span class="sxs-lookup"><span data-stu-id="0e966-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-claimsmappingpolicy-from-claimsmappingpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0e966-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0e966-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-claimsmappingpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0e966-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0e966-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-claimsmappingpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0e966-136">Java</span><span class="sxs-lookup"><span data-stu-id="0e966-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-claimsmappingpolicy-from-claimsmappingpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0e966-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e966-137">Response</span></span>

<span data-ttu-id="0e966-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0e966-138">The following is an example of the response.</span></span>

> <span data-ttu-id="0e966-139">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="0e966-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0e966-140">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="0e966-140">All the properties will be returned from an actual call.</span></span>

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
