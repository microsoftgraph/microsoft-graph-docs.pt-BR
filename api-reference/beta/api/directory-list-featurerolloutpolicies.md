---
title: Listar featureRolloutPolicies
description: Recupere uma lista de objetos featureRolloutPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e24f74abf158f42335f3b218167eb40e4f0930af
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435273"
---
# <a name="list-featurerolloutpolicies"></a><span data-ttu-id="1cc1f-103">Listar featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="1cc1f-103">List featureRolloutPolicies</span></span>

<span data-ttu-id="1cc1f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1cc1f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cc1f-105">Recupere uma lista de objetos [featureRolloutPolicy](../resources/featurerolloutpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="1cc1f-105">Retrieve a list of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1cc1f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1cc1f-106">Permissions</span></span>

<span data-ttu-id="1cc1f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cc1f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1cc1f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cc1f-109">Permission type</span></span>                        | <span data-ttu-id="1cc1f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cc1f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1cc1f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cc1f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1cc1f-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="1cc1f-112">Policy.Read.All</span></span> |
| <span data-ttu-id="1cc1f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cc1f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cc1f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cc1f-114">Not supported.</span></span> |
| <span data-ttu-id="1cc1f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cc1f-115">Application</span></span>                            | <span data-ttu-id="1cc1f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cc1f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1cc1f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cc1f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /directory/featureRolloutPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1cc1f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1cc1f-118">Optional query parameters</span></span>

<span data-ttu-id="1cc1f-119">Este método dá suporte aos seguintes parâmetros de consulta OData para ajudar a Personalizar `$count`a `$expand`resposta `$filter`: `$orderby`, `$select`, `$skip`, `$top`,,,.</span><span class="sxs-lookup"><span data-stu-id="1cc1f-119">This method supports the following OData query parameters to help customize the response: `$count`, `$expand`, `$filter`, `$orderby`, `$select`, `$skip`, `$top`.</span></span> <span data-ttu-id="1cc1f-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1cc1f-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1cc1f-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc1f-121">Request headers</span></span>

| <span data-ttu-id="1cc1f-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1cc1f-122">Name</span></span>      |<span data-ttu-id="1cc1f-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cc1f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1cc1f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1cc1f-124">Authorization</span></span> | <span data-ttu-id="1cc1f-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="1cc1f-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1cc1f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc1f-126">Request body</span></span>

<span data-ttu-id="1cc1f-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1cc1f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1cc1f-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cc1f-128">Response</span></span>

<span data-ttu-id="1cc1f-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [featureRolloutPolicy](../resources/featurerolloutpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1cc1f-129">If successful, this method returns a `200 OK` response code and a collection of [featureRolloutPolicy](../resources/featurerolloutpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1cc1f-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1cc1f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1cc1f-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc1f-131">Request</span></span>

<span data-ttu-id="1cc1f-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1cc1f-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1cc1f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1cc1f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_featurerolloutpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/directory/featureRolloutPolicies
```
# <a name="c"></a>[<span data-ttu-id="1cc1f-134">C#</span><span class="sxs-lookup"><span data-stu-id="1cc1f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-featurerolloutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1cc1f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1cc1f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-featurerolloutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1cc1f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1cc1f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-featurerolloutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1cc1f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cc1f-137">Response</span></span>

<span data-ttu-id="1cc1f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1cc1f-138">The following is an example of the response.</span></span>

> <span data-ttu-id="1cc1f-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1cc1f-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
