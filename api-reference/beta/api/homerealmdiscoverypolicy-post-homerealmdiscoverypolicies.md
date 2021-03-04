---
title: Criar homeRealmDiscoveryPolicy
description: Crie uma nova homeRealmDiscoveryPolicy.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ae8899bf66e8c46bd593c88fe456d43a85ad7760
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435669"
---
# <a name="create-homerealmdiscoverypolicy"></a><span data-ttu-id="2c5c7-103">Criar homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="2c5c7-103">Create homeRealmDiscoveryPolicy</span></span>

<span data-ttu-id="2c5c7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c5c7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c5c7-105">Crie um novo [objeto homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2c5c7-105">Create a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2c5c7-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c5c7-106">Permissions</span></span>

<span data-ttu-id="2c5c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2c5c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2c5c7-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c5c7-109">Permission type</span></span>                        | <span data-ttu-id="2c5c7-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c5c7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2c5c7-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c5c7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2c5c7-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="2c5c7-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="2c5c7-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c5c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c5c7-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c5c7-114">Not supported.</span></span> |
| <span data-ttu-id="2c5c7-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c5c7-115">Application</span></span>                            | <span data-ttu-id="2c5c7-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="2c5c7-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c5c7-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c5c7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="2c5c7-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c5c7-118">Request headers</span></span>

| <span data-ttu-id="2c5c7-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2c5c7-119">Name</span></span>          | <span data-ttu-id="2c5c7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c5c7-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2c5c7-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c5c7-121">Authorization</span></span> | <span data-ttu-id="2c5c7-122">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="2c5c7-122">Bearer {token}</span></span> |
| <span data-ttu-id="2c5c7-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="2c5c7-123">Content-type</span></span> | <span data-ttu-id="2c5c7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2c5c7-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2c5c7-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c5c7-125">Request body</span></span>

<span data-ttu-id="2c5c7-126">No corpo da solicitação, fornece uma representação JSON do [objeto homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="2c5c7-126">In the request body, supply a JSON representation of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2c5c7-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c5c7-127">Response</span></span>

<span data-ttu-id="2c5c7-128">Se tiver êxito, este método retornará um código de resposta e um `201 Created` novo [objeto homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c5c7-128">If successful, this method returns a `201 Created` response code and a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2c5c7-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2c5c7-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2c5c7-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c5c7-130">Request</span></span>

<span data-ttu-id="2c5c7-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c5c7-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2c5c7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c5c7-132">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="2c5c7-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c5c7-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c5c7-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c5c7-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="2c5c7-135">C#</span><span class="sxs-lookup"><span data-stu-id="2c5c7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c5c7-136">Java</span><span class="sxs-lookup"><span data-stu-id="2c5c7-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2c5c7-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c5c7-137">Response</span></span>

<span data-ttu-id="2c5c7-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2c5c7-138">The following is an example of the response.</span></span>

> <span data-ttu-id="2c5c7-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2c5c7-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


