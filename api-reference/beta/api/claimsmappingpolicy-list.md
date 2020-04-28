---
title: Listar claimsMappingPolicies
description: Obtenha uma lista de objetos claimsMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4a257d9cdb1466bb28b3b511ce85a2776c288144
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2020
ms.locfileid: "43916624"
---
# <a name="list-claimsmappingpolicies"></a><span data-ttu-id="13189-103">Listar claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="13189-103">List claimsMappingPolicies</span></span>

<span data-ttu-id="13189-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13189-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13189-105">Obtenha uma lista de objetos [claimsMappingPolicy](../resources/claimsmappingpolicy.md) .</span><span class="sxs-lookup"><span data-stu-id="13189-105">Get a list of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="13189-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="13189-106">Permissions</span></span>

<span data-ttu-id="13189-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="13189-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="13189-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="13189-109">Permission type</span></span>                        | <span data-ttu-id="13189-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="13189-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="13189-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="13189-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="13189-112">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="13189-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="13189-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="13189-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="13189-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="13189-114">Not supported.</span></span> |
| <span data-ttu-id="13189-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="13189-115">Application</span></span>                            | <span data-ttu-id="13189-116">Policy. Read. All, Policy. ReadWrite. ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="13189-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="13189-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="13189-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/claimsMappingPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="13189-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="13189-118">Optional query parameters</span></span>

<span data-ttu-id="13189-119">Este método oferece suporte `$expand`a `$filter`, `$select` e `$top` a parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="13189-119">This method supports the `$expand`, `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="13189-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="13189-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="13189-121">Ao usar `$expand` certifique-se de que seu aplicativo solicite permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="13189-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="13189-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13189-122">Request headers</span></span>

| <span data-ttu-id="13189-123">Nome</span><span class="sxs-lookup"><span data-stu-id="13189-123">Name</span></span>      |<span data-ttu-id="13189-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="13189-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="13189-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="13189-125">Authorization</span></span> | <span data-ttu-id="13189-126">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="13189-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="13189-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="13189-127">Request body</span></span>

<span data-ttu-id="13189-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="13189-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="13189-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="13189-129">Response</span></span>

<span data-ttu-id="13189-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [claimsMappingPolicy](../resources/claimsmappingpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="13189-130">If successful, this method returns a `200 OK` response code and a collection of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="13189-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="13189-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="13189-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="13189-132">Request</span></span>

<span data-ttu-id="13189-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="13189-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="13189-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="13189-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_claimsmappingpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/claimsMappingPolicies
```
# <a name="c"></a>[<span data-ttu-id="13189-135">C#</span><span class="sxs-lookup"><span data-stu-id="13189-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-claimsmappingpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="13189-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="13189-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-claimsmappingpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="13189-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="13189-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-claimsmappingpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="13189-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="13189-138">Response</span></span>

<span data-ttu-id="13189-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="13189-139">The following is an example of the response.</span></span>

> <span data-ttu-id="13189-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="13189-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
