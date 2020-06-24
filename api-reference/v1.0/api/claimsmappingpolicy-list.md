---
title: Listar claimsMappingPolicies
description: Obtenha uma lista de objetos claimsMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c29332a35e9112207f3033b4e63f2b9f73ca2f9e
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846196"
---
# <a name="list-claimsmappingpolicies"></a><span data-ttu-id="55134-103">Listar claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="55134-103">List claimsMappingPolicies</span></span>

<span data-ttu-id="55134-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55134-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="55134-105">Obtenha uma lista de objetos [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="55134-105">Get a list of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="55134-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="55134-106">Permissions</span></span>

<span data-ttu-id="55134-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="55134-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="55134-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55134-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="55134-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55134-109">Permission type</span></span>                        | <span data-ttu-id="55134-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="55134-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="55134-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55134-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="55134-112">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="55134-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="55134-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55134-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55134-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55134-114">Not supported.</span></span> |
| <span data-ttu-id="55134-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55134-115">Application</span></span>                            | <span data-ttu-id="55134-116">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="55134-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="55134-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55134-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/claimsMappingPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="55134-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="55134-118">Optional query parameters</span></span>

<span data-ttu-id="55134-119">Este método oferece suporte a `$expand` , `$filter` e a parâmetros de `$select` `$top` consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="55134-119">This method supports the `$expand`, `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="55134-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="55134-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="55134-121">Ao usar `$expand` certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="55134-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="55134-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55134-122">Request headers</span></span>

| <span data-ttu-id="55134-123">Nome</span><span class="sxs-lookup"><span data-stu-id="55134-123">Name</span></span>      |<span data-ttu-id="55134-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="55134-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="55134-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="55134-125">Authorization</span></span> | <span data-ttu-id="55134-126">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="55134-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="55134-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55134-127">Request body</span></span>

<span data-ttu-id="55134-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="55134-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="55134-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="55134-129">Response</span></span>

<span data-ttu-id="55134-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [claimsMappingPolicy](../resources/claimsmappingpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55134-130">If successful, this method returns a `200 OK` response code and a collection of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="55134-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="55134-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="55134-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55134-132">Request</span></span>

<span data-ttu-id="55134-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="55134-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="55134-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="55134-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_claimsmappingpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies
```

### <a name="response"></a><span data-ttu-id="55134-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="55134-135">Response</span></span>

<span data-ttu-id="55134-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="55134-136">The following is an example of the response.</span></span>

> <span data-ttu-id="55134-137">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="55134-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="55134-138">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="55134-138">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy",
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
  "description": "List claimsMappingPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
