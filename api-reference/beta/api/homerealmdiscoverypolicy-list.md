---
title: Listar homeRealmDiscoveryPolicies
description: Obtenha uma lista de objetos homeRealmDiscoveryPolicy.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 34fc65cecaaef50be3eccf129f3a9e86fa0f4694
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234094"
---
# <a name="list-homerealmdiscoverypolicies"></a><span data-ttu-id="c36b9-103">Listar homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="c36b9-103">List homeRealmDiscoveryPolicies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c36b9-104">Obtenha uma lista de objetos [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="c36b9-104">Get a list of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c36b9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="c36b9-105">Permissions</span></span>

<span data-ttu-id="c36b9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c36b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c36b9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c36b9-108">Permission type</span></span>                        | <span data-ttu-id="c36b9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c36b9-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c36b9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c36b9-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c36b9-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="c36b9-111">Policy.Read.All</span></span> |
| <span data-ttu-id="c36b9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c36b9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c36b9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c36b9-113">Not supported.</span></span> |
| <span data-ttu-id="c36b9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c36b9-114">Application</span></span>                            | <span data-ttu-id="c36b9-115">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="c36b9-115">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c36b9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c36b9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/homeRealmDiscoveryPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c36b9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c36b9-117">Optional query parameters</span></span>

<span data-ttu-id="c36b9-118">Este método oferece suporte `$expand`a `$filter`, `$select` e `$top` a parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c36b9-118">This method supports the `$expand`, `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="c36b9-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="c36b9-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="c36b9-120">Ao usar `$expand` certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="c36b9-120">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c36b9-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c36b9-121">Request headers</span></span>

| <span data-ttu-id="c36b9-122">Nome</span><span class="sxs-lookup"><span data-stu-id="c36b9-122">Name</span></span>      |<span data-ttu-id="c36b9-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c36b9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c36b9-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="c36b9-124">Authorization</span></span> | <span data-ttu-id="c36b9-125">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="c36b9-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c36b9-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c36b9-126">Request body</span></span>

<span data-ttu-id="c36b9-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c36b9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c36b9-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="c36b9-128">Response</span></span>

<span data-ttu-id="c36b9-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c36b9-129">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c36b9-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c36b9-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c36b9-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c36b9-131">Request</span></span>

<span data-ttu-id="c36b9-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c36b9-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_homerealmdiscoverypolicies"
}-->

```http
GET https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies
```

### <a name="response"></a><span data-ttu-id="c36b9-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="c36b9-133">Response</span></span>

<span data-ttu-id="c36b9-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c36b9-134">The following is an example of the response.</span></span>

> <span data-ttu-id="c36b9-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c36b9-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List homeRealmDiscoveryPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->