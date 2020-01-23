---
title: Criar homeRealmDiscoveryPolicy
description: Criar um novo homeRealmDiscoveryPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac52450c558b709c74d024d30c843679eda239ea
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475765"
---
# <a name="create-homerealmdiscoverypolicy"></a><span data-ttu-id="11023-103">Criar homeRealmDiscoveryPolicy</span><span class="sxs-lookup"><span data-stu-id="11023-103">Create homeRealmDiscoveryPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11023-104">Criar um novo objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="11023-104">Create a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="11023-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="11023-105">Permissions</span></span>

<span data-ttu-id="11023-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11023-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11023-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="11023-108">Permission type</span></span>                        | <span data-ttu-id="11023-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="11023-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="11023-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="11023-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="11023-111">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="11023-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="11023-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="11023-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11023-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="11023-113">Not supported.</span></span> |
| <span data-ttu-id="11023-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="11023-114">Application</span></span>                            | <span data-ttu-id="11023-115">Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="11023-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="11023-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="11023-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/homeRealmDiscoveryPolicies
```

## <a name="request-headers"></a><span data-ttu-id="11023-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="11023-117">Request headers</span></span>

| <span data-ttu-id="11023-118">Nome</span><span class="sxs-lookup"><span data-stu-id="11023-118">Name</span></span>          | <span data-ttu-id="11023-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="11023-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="11023-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="11023-120">Authorization</span></span> | <span data-ttu-id="11023-121">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="11023-121">Bearer {token}</span></span> |
| <span data-ttu-id="11023-122">Content-type</span><span class="sxs-lookup"><span data-stu-id="11023-122">Content-type</span></span> | <span data-ttu-id="11023-123">application/json</span><span class="sxs-lookup"><span data-stu-id="11023-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="11023-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="11023-124">Request body</span></span>

<span data-ttu-id="11023-125">No corpo da solicitação, forneça uma representação JSON do objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="11023-125">In the request body, supply a JSON representation of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="11023-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="11023-126">Response</span></span>

<span data-ttu-id="11023-127">Se tiver êxito, este método retornará `201 Created` um código de resposta e um novo objeto [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="11023-127">If successful, this method returns a `201 Created` response code and a new [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="11023-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="11023-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="11023-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="11023-129">Request</span></span>

<span data-ttu-id="11023-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="11023-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="11023-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="11023-131">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="11023-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11023-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="11023-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11023-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-homerealmdiscoverypolicy-from-homerealmdiscoverypolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="11023-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="11023-134">Response</span></span>

<span data-ttu-id="11023-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="11023-135">The following is an example of the response.</span></span>

> <span data-ttu-id="11023-p102">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="11023-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
