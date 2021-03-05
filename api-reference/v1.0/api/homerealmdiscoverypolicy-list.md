---
title: Listar homeRealmDiscoveryPolicies
description: Obter uma lista de objetos homeRealmDiscoveryPolicy.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1d39a040d4afcdcbe6ef7ba510b0a89551a2babd
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441890"
---
# <a name="list-homerealmdiscoverypolicies"></a><span data-ttu-id="f877e-103">Listar homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="f877e-103">List homeRealmDiscoveryPolicies</span></span>

<span data-ttu-id="f877e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f877e-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="f877e-105">Obter uma lista de [objetos homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="f877e-105">Get a list of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="f877e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f877e-106">Permissions</span></span>

<span data-ttu-id="f877e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f877e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f877e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f877e-109">Permission type</span></span>                        | <span data-ttu-id="f877e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f877e-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f877e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f877e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f877e-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f877e-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="f877e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f877e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f877e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f877e-114">Not supported.</span></span> |
| <span data-ttu-id="f877e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f877e-115">Application</span></span>                            | <span data-ttu-id="f877e-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="f877e-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="f877e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f877e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/homeRealmDiscoveryPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f877e-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f877e-118">Optional query parameters</span></span>

<span data-ttu-id="f877e-119">Este método dá suporte `$expand` aos `$filter` parâmetros de consulta , , e OData para ajudar a `$select` personalizar a `$top` resposta.</span><span class="sxs-lookup"><span data-stu-id="f877e-119">This method supports the `$expand`, `$filter`, `$select`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="f877e-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="f877e-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="f877e-121">Ao usar `$expand` , certifique-se de que seu aplicativo solicita permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="f877e-121">When using `$expand`, make sure that your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f877e-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f877e-122">Request headers</span></span>

| <span data-ttu-id="f877e-123">Nome</span><span class="sxs-lookup"><span data-stu-id="f877e-123">Name</span></span>      |<span data-ttu-id="f877e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f877e-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f877e-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f877e-125">Authorization</span></span> | <span data-ttu-id="f877e-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f877e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f877e-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f877e-128">Request body</span></span>

<span data-ttu-id="f877e-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f877e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f877e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="f877e-130">Response</span></span>

<span data-ttu-id="f877e-131">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f877e-131">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f877e-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f877e-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f877e-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f877e-133">Request</span></span>

<span data-ttu-id="f877e-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f877e-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f877e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f877e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_homerealmdiscoverypolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies
```
# <a name="c"></a>[<span data-ttu-id="f877e-136">C#</span><span class="sxs-lookup"><span data-stu-id="f877e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-homerealmdiscoverypolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f877e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f877e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-homerealmdiscoverypolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f877e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f877e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-homerealmdiscoverypolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f877e-139">Java</span><span class="sxs-lookup"><span data-stu-id="f877e-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-homerealmdiscoverypolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f877e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="f877e-140">Response</span></span>

<span data-ttu-id="f877e-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f877e-141">The following is an example of the response.</span></span>

> <span data-ttu-id="f877e-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f877e-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

