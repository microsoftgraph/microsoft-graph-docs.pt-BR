---
title: Obter featureRolloutPolicy
description: Recupere as propriedades e os relacionamentos de um objeto featurerolloutpolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7ddf2072116cdf7209c2bf24def5edda6aebadcf
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721716"
---
# <a name="get-featurerolloutpolicy"></a><span data-ttu-id="09d07-103">Obter featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="09d07-103">Get featureRolloutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09d07-104">Recupere as propriedades e os relacionamentos de um objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="09d07-104">Retrieve the properties and relationships of a [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="09d07-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="09d07-105">Permissions</span></span>

<span data-ttu-id="09d07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="09d07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="09d07-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09d07-108">Permission type</span></span>                        | <span data-ttu-id="09d07-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09d07-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="09d07-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09d07-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="09d07-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="09d07-111">Policy.Read.All</span></span> |
| <span data-ttu-id="09d07-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09d07-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09d07-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09d07-113">Not supported.</span></span> |
| <span data-ttu-id="09d07-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09d07-114">Application</span></span>                            | <span data-ttu-id="09d07-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09d07-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="09d07-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09d07-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="09d07-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="09d07-117">Optional query parameters</span></span>

<span data-ttu-id="09d07-118">Este método oferece suporte `$select` ao parâmetro de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="09d07-118">This method supports the `$select` OData query parameter to help customize the response.</span></span> <span data-ttu-id="09d07-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="09d07-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="09d07-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09d07-120">Request headers</span></span>

| <span data-ttu-id="09d07-121">Nome</span><span class="sxs-lookup"><span data-stu-id="09d07-121">Name</span></span>      |<span data-ttu-id="09d07-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="09d07-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="09d07-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="09d07-123">Authorization</span></span> | <span data-ttu-id="09d07-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="09d07-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="09d07-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09d07-125">Request body</span></span>

<span data-ttu-id="09d07-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="09d07-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09d07-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="09d07-127">Response</span></span>

<span data-ttu-id="09d07-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [featureRolloutPolicy](../resources/featurerolloutpolicy.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09d07-128">If successful, this method returns a `200 OK` response code and the requested [featureRolloutPolicy](../resources/featurerolloutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="09d07-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="09d07-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="09d07-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09d07-130">Request</span></span>

<span data-ttu-id="09d07-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="09d07-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="09d07-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="09d07-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="09d07-133">C#</span><span class="sxs-lookup"><span data-stu-id="09d07-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="09d07-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09d07-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="09d07-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="09d07-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="09d07-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="09d07-136">Response</span></span>

<span data-ttu-id="09d07-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="09d07-137">The following is an example of the response.</span></span>

> <span data-ttu-id="09d07-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09d07-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
  "displayName": "SeamlessSso rollout policy",
  "description": "SeamlessSso rollout policy",
  "feature": "seamlessSso",
  "isEnabled": true,
  "isAppliedToOrganization": false
}
```

### <a name="request"></a><span data-ttu-id="09d07-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09d07-140">Request</span></span>

<span data-ttu-id="09d07-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="09d07-141">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="09d07-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="09d07-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c?$expand=appliesTo
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="09d07-143">C#</span><span class="sxs-lookup"><span data-stu-id="09d07-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="09d07-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="09d07-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="09d07-145">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="09d07-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="09d07-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="09d07-146">Response</span></span>

<span data-ttu-id="09d07-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="09d07-147">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="09d07-148">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="09d07-148">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="09d07-149">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09d07-149">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
  "displayName": "SeamlessSso rollout policy",
  "description": "SeamlessSso rollout policy",
  "feature": "seamlessSso",
  "isEnabled": true,
  "isAppliedToOrganization": false,
  "appliesTo": [
    {
      "id": "2441b489-4f12-4882-b039-8f6006bd66da",
      "objectType": "group"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
