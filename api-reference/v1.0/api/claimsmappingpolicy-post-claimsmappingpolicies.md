---
title: Criar claimsMappingPolicy
description: Crie uma nova claimsMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: f0f22d941c5d7f5ed1e3691e461d6cda25d5b31f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52051547"
---
# <a name="create-claimsmappingpolicy"></a><span data-ttu-id="24506-103">Criar claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="24506-103">Create claimsMappingPolicy</span></span>

<span data-ttu-id="24506-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24506-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="24506-105">Crie um novo [objeto claimsMappingPolicy.](../resources/claimsmappingpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="24506-105">Create a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="24506-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="24506-106">Permissions</span></span>

<span data-ttu-id="24506-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="24506-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24506-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="24506-109">Permission type</span></span>                        | <span data-ttu-id="24506-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="24506-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="24506-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="24506-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="24506-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="24506-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="24506-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="24506-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24506-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="24506-114">Not supported.</span></span> |
| <span data-ttu-id="24506-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="24506-115">Application</span></span>                            | <span data-ttu-id="24506-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="24506-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="24506-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24506-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="24506-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24506-118">Request headers</span></span>

| <span data-ttu-id="24506-119">Nome</span><span class="sxs-lookup"><span data-stu-id="24506-119">Name</span></span>          | <span data-ttu-id="24506-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="24506-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="24506-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="24506-121">Authorization</span></span> | <span data-ttu-id="24506-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="24506-122">Bearer {token}</span></span> |
| <span data-ttu-id="24506-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="24506-123">Content-type</span></span> | <span data-ttu-id="24506-124">application/json</span><span class="sxs-lookup"><span data-stu-id="24506-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="24506-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24506-125">Request body</span></span>

<span data-ttu-id="24506-126">No corpo da solicitação, fornece uma representação JSON do [objeto claimsMappingPolicy.](../resources/claimsmappingpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="24506-126">In the request body, supply a JSON representation of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="24506-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="24506-127">Response</span></span>

<span data-ttu-id="24506-128">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto claimsMappingPolicy](../resources/claimsmappingpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24506-128">If successful, this method returns a `201 Created` response code and a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="24506-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="24506-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="24506-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24506-130">Request</span></span>

<span data-ttu-id="24506-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="24506-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="24506-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="24506-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="24506-133">C#</span><span class="sxs-lookup"><span data-stu-id="24506-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-claimsmappingpolicy-from-claimsmappingpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="24506-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24506-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-claimsmappingpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="24506-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24506-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-claimsmappingpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="24506-136">Java</span><span class="sxs-lookup"><span data-stu-id="24506-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-claimsmappingpolicy-from-claimsmappingpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="24506-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="24506-137">Response</span></span>

<span data-ttu-id="24506-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="24506-138">The following is an example of the response.</span></span>

> <span data-ttu-id="24506-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="24506-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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

