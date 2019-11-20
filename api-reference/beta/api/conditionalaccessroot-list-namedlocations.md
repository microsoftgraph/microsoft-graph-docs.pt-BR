---
title: Listar namedLocations
description: Obtenha uma lista de objetos namedLocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 387e27b30fe9dae92b22855e0f5b6ff721b4019c
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "38747554"
---
# <a name="list-namedlocations"></a><span data-ttu-id="0b2b5-103">Listar namedLocations</span><span class="sxs-lookup"><span data-stu-id="0b2b5-103">List namedLocations</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b2b5-104">Obtenha uma lista de objetos [namedLocation](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="0b2b5-104">Get a list of [namedLocation](../resources/namedlocation.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b2b5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="0b2b5-105">Permissions</span></span>

<span data-ttu-id="0b2b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0b2b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b2b5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0b2b5-108">Permission type</span></span>                        | <span data-ttu-id="0b2b5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0b2b5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0b2b5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0b2b5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b2b5-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b2b5-111">Policy.Read.All</span></span> |
| <span data-ttu-id="0b2b5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0b2b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b2b5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0b2b5-113">Not supported.</span></span> |
| <span data-ttu-id="0b2b5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b2b5-114">Application</span></span>                            | <span data-ttu-id="0b2b5-115">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b2b5-115">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0b2b5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0b2b5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/namedLocations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b2b5-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0b2b5-117">Optional query parameters</span></span>

<span data-ttu-id="0b2b5-118">Este método oferece suporte `$count`aos `$filter`parâmetros `$orderBy`de `$select`consulta `$skip`do, `$top` ,,, e OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="0b2b5-118">This method supports the `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="0b2b5-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0b2b5-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b2b5-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b2b5-120">Request headers</span></span>

| <span data-ttu-id="0b2b5-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0b2b5-121">Name</span></span>      |<span data-ttu-id="0b2b5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b2b5-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0b2b5-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0b2b5-123">Authorization</span></span> | <span data-ttu-id="0b2b5-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0b2b5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0b2b5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0b2b5-126">Request body</span></span>

<span data-ttu-id="0b2b5-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0b2b5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b2b5-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b2b5-128">Response</span></span>

<span data-ttu-id="0b2b5-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [namedLocation](../resources/namedlocation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0b2b5-129">If successful, this method returns a `200 OK` response code and a collection of [namedLocation](../resources/namedlocation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b2b5-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0b2b5-130">Examples</span></span>

### <a name="example-1-list-all-namedlocations"></a><span data-ttu-id="0b2b5-131">Exemplo 1: listar todos os namedLocations</span><span class="sxs-lookup"><span data-stu-id="0b2b5-131">Example 1: List all namedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="0b2b5-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b2b5-132">Request</span></span>

<span data-ttu-id="0b2b5-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b2b5-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0b2b5-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b2b5-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b2b5-135">C#</span><span class="sxs-lookup"><span data-stu-id="0b2b5-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b2b5-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b2b5-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b2b5-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b2b5-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b2b5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b2b5-138">Response</span></span>

<span data-ttu-id="0b2b5-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0b2b5-139">The following is an example of the response.</span></span>

> <span data-ttu-id="0b2b5-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b2b5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/namedLocations",
    "value": [
        {
            "@odata.type": "#microsoft.graph.ipNamedLocation",
            "id": "06e4ff15-ca6b-4843-9c34-3fdd1ce8f739",
            "displayName": "IPv4 named location",
            "modifiedDateTime": "2019-07-26T18:00:43.5796446Z",
            "createdDateTime": "2018-06-22T11:56:12Z",
            "isTrusted": false,
            "ipRanges": [
                {
                    "@odata.type": "#microsoft.graph.iPv4CidrRange",
                    "cidrAddress": "6.5.4.3/32"
                },
                {
                    "@odata.type": "#microsoft.graph.iPv4CidrRange",
                    "cidrAddress": "127.126.125.0/24"
                }
            ]
        },
        {
            "@odata.type": "#microsoft.graph.countryNamedLocation",
            "id": "1b7f0916-7677-40d8-97a1-d606f4ed8fcf",
            "displayName": "Country named location",
            "modifiedDateTime": "2018-09-10T16:54:53.7238848Z",
            "createdDateTime": "2018-09-10T16:54:53.7238848Z",
            "countriesAndRegions": [
                "US",
                "CA"
            ],
            "includeUnknownCountriesAndRegions": false
        },
        {
            "@odata.type": "#microsoft.graph.ipNamedLocation",
            "id": "05239353-9117-4d29-a6a1-89724cb61b8c",
            "displayName": "Trusted IPv6 named location",
            "modifiedDateTime": "2019-09-16T00:47:36.4967092Z",
            "createdDateTime": "2019-09-15T21:53:34.5001162Z",
            "isTrusted": true,
            "ipRanges": [
                {
                    "@odata.type": "#microsoft.graph.iPv6CidrRange",
                    "cidrAddress": "2001:4898:80e8:7:d92a:7695:fda1:9d62/48"
                },
                {
                    "@odata.type": "#microsoft.graph.iPv6CidrRange",
                    "cidrAddress": "2001:4898:80d8:7:d92a:7695:fda1:9d62/48"
                }
            ]
        }
    ]
}
```
### <a name="example-2-list-all-ipnamedlocations"></a><span data-ttu-id="0b2b5-142">Exemplo 2: listar todos os ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="0b2b5-142">Example 2: List all ipNamedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="0b2b5-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b2b5-143">Request</span></span>

<span data-ttu-id="0b2b5-144">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b2b5-144">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0b2b5-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b2b5-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations?$filter=isof('microsoft.graph.ipNamedLocation')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b2b5-146">C#</span><span class="sxs-lookup"><span data-stu-id="0b2b5-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b2b5-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b2b5-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b2b5-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b2b5-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b2b5-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b2b5-149">Response</span></span>

<span data-ttu-id="0b2b5-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0b2b5-150">The following is an example of the response.</span></span>

> <span data-ttu-id="0b2b5-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b2b5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/namedLocations",
    "value": [
        {
            "@odata.type": "#microsoft.graph.ipNamedLocation",
            "id": "06e4ff15-ca6b-4843-9c34-3fdd1ce8f739",
            "displayName": "IPv4 named location",
            "modifiedDateTime": "2019-07-26T18:00:43.5796446Z",
            "createdDateTime": "2018-06-22T11:56:12Z",
            "isTrusted": false,
            "ipRanges": [
                {
                    "@odata.type": "#microsoft.graph.iPv4CidrRange",
                    "cidrAddress": "6.5.4.3/32"
                },
                {
                    "@odata.type": "#microsoft.graph.iPv4CidrRange",
                    "cidrAddress": "127.126.125.0/24"
                }
            ]
        },
        {
            "@odata.type": "#microsoft.graph.ipNamedLocation",
            "id": "05239353-9117-4d29-a6a1-89724cb61b8c",
            "displayName": "Trusted IPv6 named location",
            "modifiedDateTime": "2019-09-16T00:47:36.4967092Z",
            "createdDateTime": "2019-09-15T21:53:34.5001162Z",
            "isTrusted": true,
            "ipRanges": [
                {
                    "@odata.type": "#microsoft.graph.iPv6CidrRange",
                    "cidrAddress": "2001:4898:80e8:7:d92a:7695:fda1:9d62/48"
                },
                {
                    "@odata.type": "#microsoft.graph.iPv6CidrRange",
                    "cidrAddress": "2001:4898:80d8:7:d92a:7695:fda1:9d62/48"
                }
            ]
        }
    ]
}
```
### <a name="example-3-list-all-namedlocations-created-after-a-certain-date"></a><span data-ttu-id="0b2b5-153">Exemplo 3: listar todos os namedLocations criados após uma determinada data</span><span class="sxs-lookup"><span data-stu-id="0b2b5-153">Example 3: List all namedLocations created after a certain date</span></span>

#### <a name="request"></a><span data-ttu-id="0b2b5-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b2b5-154">Request</span></span>

<span data-ttu-id="0b2b5-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b2b5-155">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0b2b5-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b2b5-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations?$filter=createdDateTime ge 2019-09-01T00:00:00Z
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b2b5-157">C#</span><span class="sxs-lookup"><span data-stu-id="0b2b5-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b2b5-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b2b5-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b2b5-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b2b5-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b2b5-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b2b5-160">Response</span></span>

<span data-ttu-id="0b2b5-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0b2b5-161">The following is an example of the response.</span></span>

> <span data-ttu-id="0b2b5-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b2b5-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/namedLocations",
    "value": [
        {
            "@odata.type": "#microsoft.graph.ipNamedLocation",
            "id": "05239353-9117-4d29-a6a1-89724cb61b8c",
            "displayName": "Trusted IPv6 named location",
            "modifiedDateTime": "2019-09-16T00:47:36.4967092Z",
            "createdDateTime": "2019-09-15T21:53:34.5001162Z",
            "isTrusted": true,
            "ipRanges": [
                {
                    "@odata.type": "#microsoft.graph.iPv6CidrRange",
                    "cidrAddress": "2001:4898:80e8:7:d92a:7695:fda1:9d62/48"
                },
                {
                    "@odata.type": "#microsoft.graph.iPv6CidrRange",
                    "cidrAddress": "2001:4898:80d8:7:d92a:7695:fda1:9d62/48"
                }
            ]
        }
    ]
}
```
### <a name="example-4-list-all-countrynamedlocations-containing-a-certain-country-or-region"></a><span data-ttu-id="0b2b5-164">Exemplo 4: listar todos os countryNamedLocations contendo um determinado país ou região</span><span class="sxs-lookup"><span data-stu-id="0b2b5-164">Example 4: List all countryNamedLocations containing a certain country or region</span></span>

#### <a name="request"></a><span data-ttu-id="0b2b5-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0b2b5-165">Request</span></span>

<span data-ttu-id="0b2b5-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0b2b5-166">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0b2b5-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b2b5-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations?$filter=microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b2b5-168">C#</span><span class="sxs-lookup"><span data-stu-id="0b2b5-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b2b5-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b2b5-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b2b5-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b2b5-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b2b5-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="0b2b5-171">Response</span></span>

<span data-ttu-id="0b2b5-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0b2b5-172">The following is an example of the response.</span></span>

> <span data-ttu-id="0b2b5-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0b2b5-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.namedLocation",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json


{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#conditionalAccess/namedLocations",
    "value": [
        {
            "@odata.type": "#microsoft.graph.countryNamedLocation",
            "id": "1b7f0916-7677-40d8-97a1-d606f4ed8fcf",
            "displayName": "Country named location",
            "modifiedDateTime": "2018-09-10T16:54:53.7238848Z",
            "createdDateTime": "2018-09-10T16:54:53.7238848Z",
            "countriesAndRegions": [
                "US",
                "CA"
            ],
            "includeUnknownCountriesAndRegions": false
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List namedLocations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
