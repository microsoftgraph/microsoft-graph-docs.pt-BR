---
title: Listar featureRolloutPolicies
description: Recupere uma lista de objetos featureRolloutPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7d9cfd0261cd00e41c47cba312c2fbd42db944b9
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417505"
---
# <a name="list-featurerolloutpolicies"></a><span data-ttu-id="f530b-103">Listar featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="f530b-103">List featureRolloutPolicies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f530b-104">Recupere uma lista de objetos [featureRolloutPolicy](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="f530b-104">Retrieve a list of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f530b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="f530b-105">Permissions</span></span>

<span data-ttu-id="f530b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f530b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f530b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f530b-108">Permission type</span></span>                        | <span data-ttu-id="f530b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f530b-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f530b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f530b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f530b-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="f530b-111">Policy.Read.All</span></span> |
| <span data-ttu-id="f530b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f530b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f530b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f530b-113">Not supported.</span></span> |
| <span data-ttu-id="f530b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f530b-114">Application</span></span>                            | <span data-ttu-id="f530b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f530b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f530b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f530b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f530b-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f530b-117">Optional query parameters</span></span>

<span data-ttu-id="f530b-118">Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a Personalizar `$count`a `$expand`resposta `$filter`: `$orderby`, `$select`, `$skip`, `$top`,,,.</span><span class="sxs-lookup"><span data-stu-id="f530b-118">This method supports the following OData query parameters to help customize the response: `$count`, `$expand`, `$filter`, `$orderby`, `$select`, `$skip`, `$top`.</span></span> <span data-ttu-id="f530b-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f530b-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f530b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f530b-120">Request headers</span></span>

| <span data-ttu-id="f530b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f530b-121">Name</span></span>      |<span data-ttu-id="f530b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f530b-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f530b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f530b-123">Authorization</span></span> | <span data-ttu-id="f530b-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="f530b-124">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f530b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f530b-125">Request body</span></span>

<span data-ttu-id="f530b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f530b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f530b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f530b-127">Response</span></span>

<span data-ttu-id="f530b-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [featureRolloutPolicy](../resources/featurerolloutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f530b-128">If successful, this method returns a `200 OK` response code and a collection of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f530b-129">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f530b-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f530b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f530b-130">Request</span></span>

<span data-ttu-id="f530b-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f530b-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="f530b-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f530b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicies"
}-->

```http
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="f530b-133">C#</span><span class="sxs-lookup"><span data-stu-id="f530b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f530b-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f530b-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="f530b-135">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f530b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f530b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f530b-136">Response</span></span>

<span data-ttu-id="f530b-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f530b-137">The following is an example of the response.</span></span>

> <span data-ttu-id="f530b-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f530b-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "e3c2f23a-edd2-43a8-849f-154e70794ac5",
      "displayName": "PassthroughAuthentication rollout policy",
      "description": "PassthroughAuthentication rollout policy",
      "feature": "passthroughAuthentication",
      "isEnabled": true,
      "isAppliedToOrganization": false
    },
    {
      "id": "df85e4d9-e8c4-4033-a41c-73419a95c29c",
      "displayName": "SeamlessSso rollout policy",
      "description": "SeamlessSso rollout policy",
      "feature": "seamlessSso",
      "isEnabled": true,
      "isAppliedToOrganization": false
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List featureRolloutPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
