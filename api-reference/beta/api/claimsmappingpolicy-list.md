---
title: Listar claimsMappingPolicies
description: Obter uma lista de objetos claimsMappingPolicy.
localization_priority: Normal
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8edf50e39377b7c5205e5f9d23368cf4e9684f89
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437713"
---
# <a name="list-claimsmappingpolicies"></a><span data-ttu-id="b9d75-103">Listar claimsMappingPolicies</span><span class="sxs-lookup"><span data-stu-id="b9d75-103">List claimsMappingPolicies</span></span>

<span data-ttu-id="b9d75-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9d75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9d75-105">Obter uma lista de [objetos claimsMappingPolicy.](../resources/claimsmappingpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="b9d75-105">Get a list of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="b9d75-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="b9d75-106">Permissions</span></span>

<span data-ttu-id="b9d75-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9d75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b9d75-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9d75-109">Permission type</span></span>                        | <span data-ttu-id="b9d75-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b9d75-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b9d75-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9d75-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b9d75-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="b9d75-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="b9d75-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9d75-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9d75-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9d75-114">Not supported.</span></span> |
| <span data-ttu-id="b9d75-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b9d75-115">Application</span></span>                            | <span data-ttu-id="b9d75-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="b9d75-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="b9d75-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9d75-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/claimsMappingPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9d75-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="b9d75-118">Optional query parameters</span></span>

<span data-ttu-id="b9d75-119">Este método dá suporte `$expand` aos `$filter` parâmetros de consulta , e OData para ajudar a personalizar `$select` a `$top` resposta.</span><span class="sxs-lookup"><span data-stu-id="b9d75-119">This method supports the `$expand`, `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="b9d75-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="b9d75-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="b9d75-121">Ao `$expand` usar, certifique-se de que seu aplicativo solicita permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="b9d75-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b9d75-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9d75-122">Request headers</span></span>

| <span data-ttu-id="b9d75-123">Nome</span><span class="sxs-lookup"><span data-stu-id="b9d75-123">Name</span></span>      |<span data-ttu-id="b9d75-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9d75-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b9d75-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9d75-125">Authorization</span></span> | <span data-ttu-id="b9d75-126">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="b9d75-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b9d75-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9d75-127">Request body</span></span>

<span data-ttu-id="b9d75-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9d75-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9d75-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9d75-129">Response</span></span>

<span data-ttu-id="b9d75-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos claimsMappingPolicy](../resources/claimsmappingpolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b9d75-130">If successful, this method returns a `200 OK` response code and a collection of [claimsMappingPolicy](../resources/claimsmappingpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b9d75-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="b9d75-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b9d75-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9d75-132">Request</span></span>

<span data-ttu-id="b9d75-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9d75-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b9d75-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="b9d75-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_claimsmappingpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/claimsMappingPolicies
```
# <a name="c"></a>[<span data-ttu-id="b9d75-135">C#</span><span class="sxs-lookup"><span data-stu-id="b9d75-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-claimsmappingpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b9d75-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b9d75-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-claimsmappingpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b9d75-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b9d75-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-claimsmappingpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b9d75-138">Java</span><span class="sxs-lookup"><span data-stu-id="b9d75-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-claimsmappingpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b9d75-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9d75-139">Response</span></span>

<span data-ttu-id="b9d75-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="b9d75-140">The following is an example of the response.</span></span>

> <span data-ttu-id="b9d75-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9d75-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


