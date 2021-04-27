---
title: Listar homeRealmDiscoveryPolicies
description: Obter uma lista de objetos homeRealmDiscoveryPolicy.
localization_priority: Normal
author: hpsin
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e11c38f977562e76eb2b4805603a548730bf0ed1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040935"
---
# <a name="list-homerealmdiscoverypolicies"></a><span data-ttu-id="1ab70-103">Listar homeRealmDiscoveryPolicies</span><span class="sxs-lookup"><span data-stu-id="1ab70-103">List homeRealmDiscoveryPolicies</span></span>

<span data-ttu-id="1ab70-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ab70-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ab70-105">Obter uma lista de [objetos homeRealmDiscoveryPolicy.](../resources/homerealmdiscoverypolicy.md)</span><span class="sxs-lookup"><span data-stu-id="1ab70-105">Get a list of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ab70-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1ab70-106">Permissions</span></span>

<span data-ttu-id="1ab70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ab70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ab70-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ab70-109">Permission type</span></span>                        | <span data-ttu-id="1ab70-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1ab70-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="1ab70-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ab70-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ab70-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ab70-112">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="1ab70-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ab70-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ab70-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ab70-114">Not supported.</span></span> |
| <span data-ttu-id="1ab70-115">Application</span><span class="sxs-lookup"><span data-stu-id="1ab70-115">Application</span></span>                            | <span data-ttu-id="1ab70-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ab70-116">Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ab70-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ab70-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET policies/homeRealmDiscoveryPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1ab70-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1ab70-118">Optional query parameters</span></span>

<span data-ttu-id="1ab70-119">Este método dá suporte `$expand` aos `$filter` parâmetros de consulta , e OData para ajudar a personalizar `$select` a `$top` resposta.</span><span class="sxs-lookup"><span data-stu-id="1ab70-119">This method supports the `$expand`, `$filter`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="1ab70-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="1ab70-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="1ab70-121">Ao `$expand` usar, certifique-se de que seu aplicativo solicita permissões para ler os objetos expandidos.</span><span class="sxs-lookup"><span data-stu-id="1ab70-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ab70-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ab70-122">Request headers</span></span>

| <span data-ttu-id="1ab70-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1ab70-123">Name</span></span>      |<span data-ttu-id="1ab70-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ab70-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1ab70-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ab70-125">Authorization</span></span> | <span data-ttu-id="1ab70-126">Portador {token}</span><span class="sxs-lookup"><span data-stu-id="1ab70-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ab70-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ab70-127">Request body</span></span>

<span data-ttu-id="1ab70-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1ab70-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ab70-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ab70-129">Response</span></span>

<span data-ttu-id="1ab70-130">Se tiver êxito, este método retornará um código de resposta e uma coleção de `200 OK` [objetos homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ab70-130">If successful, this method returns a `200 OK` response code and a collection of [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1ab70-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1ab70-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1ab70-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ab70-132">Request</span></span>

<span data-ttu-id="1ab70-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ab70-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1ab70-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="1ab70-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_homerealmdiscoverypolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies
```
# <a name="c"></a>[<span data-ttu-id="1ab70-135">C#</span><span class="sxs-lookup"><span data-stu-id="1ab70-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-homerealmdiscoverypolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1ab70-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1ab70-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-homerealmdiscoverypolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1ab70-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1ab70-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-homerealmdiscoverypolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1ab70-138">Java</span><span class="sxs-lookup"><span data-stu-id="1ab70-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-homerealmdiscoverypolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1ab70-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ab70-139">Response</span></span>

<span data-ttu-id="1ab70-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="1ab70-140">The following is an example of the response.</span></span>

> <span data-ttu-id="1ab70-141">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="1ab70-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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


