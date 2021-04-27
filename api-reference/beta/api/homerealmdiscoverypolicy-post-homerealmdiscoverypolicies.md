---
title: Criar homeRealmDiscoveryPolicy
description: Crie uma nova homeRealmDiscoveryPolicy.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a46fd261bc29ff3a7fb275f4f8e0f1ab6e2df21f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040907"
---
# <a name="create-homerealmdiscoverypolicy"></a><span data-ttu-id="e2d25-103">Criar homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="e2d25-103">Create homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="e2d25-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2d25-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2d25-105">Crie um novo [objeto homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e2d25-105">Create a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2d25-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2d25-106">Permissions</span></span>

<span data-ttu-id="e2d25-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2d25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e2d25-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2d25-109">Permission type</span></span>                        | <span data-ttu-id="e2d25-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2d25-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e2d25-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2d25-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e2d25-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="e2d25-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="e2d25-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2d25-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2d25-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2d25-114">Not supported.</span></span> |
| <span data-ttu-id="e2d25-115">Application</span><span class="sxs-lookup"><span data-stu-id="e2d25-115">Application</span></span>                            | <span data-ttu-id="e2d25-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="e2d25-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="e2d25-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2d25-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="e2d25-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2d25-118">Request headers</span></span>

| <span data-ttu-id="e2d25-119">Nome</span><span class="sxs-lookup"><span data-stu-id="e2d25-119">Name</span></span>          | <span data-ttu-id="e2d25-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2d25-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="e2d25-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2d25-121">Authorization</span></span> | <span data-ttu-id="e2d25-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="e2d25-122">Bearer {token}</span></span> |
| <span data-ttu-id="e2d25-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="e2d25-123">Content-type</span></span> | <span data-ttu-id="e2d25-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e2d25-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e2d25-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2d25-125">Request body</span></span>

<span data-ttu-id="e2d25-126">No corpo da solicitação, fornece uma representação JSON do [objeto homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="e2d25-126">In the request body, supply a JSON representation of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e2d25-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2d25-127">Response</span></span>

<span data-ttu-id="e2d25-128">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2d25-128">If successful, this method returns a `201 Created` response code and a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e2d25-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e2d25-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e2d25-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2d25-130">Request</span></span>

<span data-ttu-id="e2d25-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2d25-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e2d25-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2d25-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_homerealmdiscoverypolicy_from_homerealmdiscoverypolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="e2d25-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2d25-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2d25-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2d25-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="e2d25-135">C#</span><span class="sxs-lookup"><span data-stu-id="e2d25-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2d25-136">Java</span><span class="sxs-lookup"><span data-stu-id="e2d25-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e2d25-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2d25-137">Response</span></span>

<span data-ttu-id="e2d25-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e2d25-138">The following is an example of the response.</span></span>

> <span data-ttu-id="e2d25-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e2d25-139">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
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
  "description": "Create homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


