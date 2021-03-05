---
title: Criar claimsMappingPolicy
description: Crie uma nova claimsMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 20aa2b84085fde1b2a68b8d6781313e60b448e74
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434794"
---
# <a name="create-claimsmappingpolicy"></a><span data-ttu-id="6c5f4-103">Criar claimsMappingPolicy</span><span class="sxs-lookup"><span data-stu-id="6c5f4-103">Create claimsMappingPolicy</span></span>

<span data-ttu-id="6c5f4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c5f4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c5f4-105">Crie um novo [objeto claimsMappingPolicy.](../resources/claimsmappingpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c5f4-105">Create a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c5f4-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6c5f4-106">Permissions</span></span>

<span data-ttu-id="6c5f4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c5f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c5f4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c5f4-109">Permission type</span></span>                        | <span data-ttu-id="6c5f4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c5f4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6c5f4-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c5f4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c5f4-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c5f4-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="6c5f4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c5f4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c5f4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c5f4-114">Not supported.</span></span> |
| <span data-ttu-id="6c5f4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c5f4-115">Application</span></span>                            | <span data-ttu-id="6c5f4-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6c5f4-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c5f4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c5f4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/claimsMappingPolicies
```

## <a name="request-headers"></a><span data-ttu-id="6c5f4-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6c5f4-118">Request headers</span></span>

| <span data-ttu-id="6c5f4-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6c5f4-119">Name</span></span>          | <span data-ttu-id="6c5f4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c5f4-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6c5f4-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6c5f4-121">Authorization</span></span> | <span data-ttu-id="6c5f4-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="6c5f4-122">Bearer {token}</span></span> |
| <span data-ttu-id="6c5f4-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="6c5f4-123">Content-type</span></span> | <span data-ttu-id="6c5f4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6c5f4-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c5f4-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c5f4-125">Request body</span></span>

<span data-ttu-id="6c5f4-126">No corpo da solicitação, fornece uma representação JSON do [objeto claimsMappingPolicy.](../resources/claimsmappingpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="6c5f4-126">In the request body, supply a JSON representation of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6c5f4-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c5f4-127">Response</span></span>

<span data-ttu-id="6c5f4-128">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto claimsMappingPolicy](../resources/claimsmappingpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6c5f4-128">If successful, this method returns a `201 Created` response code and a new [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c5f4-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6c5f4-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c5f4-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6c5f4-130">Request</span></span>

<span data-ttu-id="6c5f4-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6c5f4-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6c5f4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c5f4-132">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6c5f4-133">C#</span><span class="sxs-lookup"><span data-stu-id="6c5f4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-claimsmappingpolicy-from-claimsmappingpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c5f4-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c5f4-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-claimsmappingpolicy-from-claimsmappingpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c5f4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c5f4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-claimsmappingpolicy-from-claimsmappingpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6c5f4-136">Java</span><span class="sxs-lookup"><span data-stu-id="6c5f4-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-claimsmappingpolicy-from-claimsmappingpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6c5f4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c5f4-137">Response</span></span>

<span data-ttu-id="6c5f4-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6c5f4-138">The following is an example of the response.</span></span>

> <span data-ttu-id="6c5f4-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6c5f4-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

