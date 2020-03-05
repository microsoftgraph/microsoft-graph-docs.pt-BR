---
title: Listar namedLocations
description: Obtenha uma lista de objetos namedLocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a51aec675f0596eb5232f2f3d6160a22f03d0b7f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437942"
---
# <a name="list-namedlocations"></a><span data-ttu-id="9197c-103">Listar namedLocations</span><span class="sxs-lookup"><span data-stu-id="9197c-103">List namedLocations</span></span>

<span data-ttu-id="9197c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9197c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9197c-105">Obtenha uma lista de objetos [namedLocation](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="9197c-105">Get a list of [namedLocation](../resources/namedlocation.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9197c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9197c-106">Permissions</span></span>

<span data-ttu-id="9197c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9197c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9197c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9197c-109">Permission type</span></span>                        | <span data-ttu-id="9197c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9197c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9197c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9197c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9197c-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="9197c-112">Policy.Read.All</span></span> |
| <span data-ttu-id="9197c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9197c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9197c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9197c-114">Not supported.</span></span> |
| <span data-ttu-id="9197c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9197c-115">Application</span></span>                            | <span data-ttu-id="9197c-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="9197c-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9197c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9197c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/namedLocations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9197c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9197c-118">Optional query parameters</span></span>

<span data-ttu-id="9197c-119">Este método oferece suporte `$count`aos `$filter`parâmetros `$orderBy`de `$select`consulta `$skip`do, `$top` ,,, e OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9197c-119">This method supports the `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="9197c-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="9197c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9197c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9197c-121">Request headers</span></span>

| <span data-ttu-id="9197c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="9197c-122">Name</span></span>      |<span data-ttu-id="9197c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9197c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9197c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9197c-124">Authorization</span></span> | <span data-ttu-id="9197c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9197c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9197c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9197c-127">Request body</span></span>

<span data-ttu-id="9197c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9197c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9197c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9197c-129">Response</span></span>

<span data-ttu-id="9197c-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [namedLocation](../resources/namedlocation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9197c-130">If successful, this method returns a `200 OK` response code and a collection of [namedLocation](../resources/namedlocation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9197c-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9197c-131">Examples</span></span>

### <a name="example-1-list-all-namedlocations"></a><span data-ttu-id="9197c-132">Exemplo 1: listar todos os namedLocations</span><span class="sxs-lookup"><span data-stu-id="9197c-132">Example 1: List all namedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="9197c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9197c-133">Request</span></span>

<span data-ttu-id="9197c-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9197c-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9197c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9197c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations
```
# <a name="c"></a>[<span data-ttu-id="9197c-136">C#</span><span class="sxs-lookup"><span data-stu-id="9197c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9197c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9197c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9197c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9197c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9197c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="9197c-139">Response</span></span>

<span data-ttu-id="9197c-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9197c-140">The following is an example of the response.</span></span>

> <span data-ttu-id="9197c-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9197c-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-list-all-ipnamedlocations"></a><span data-ttu-id="9197c-143">Exemplo 2: listar todos os ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="9197c-143">Example 2: List all ipNamedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="9197c-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9197c-144">Request</span></span>

<span data-ttu-id="9197c-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9197c-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9197c-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="9197c-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations?$filter=isof('microsoft.graph.ipNamedLocation')
```
# <a name="c"></a>[<span data-ttu-id="9197c-147">C#</span><span class="sxs-lookup"><span data-stu-id="9197c-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9197c-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9197c-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9197c-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9197c-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9197c-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="9197c-150">Response</span></span>

<span data-ttu-id="9197c-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9197c-151">The following is an example of the response.</span></span>

> <span data-ttu-id="9197c-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9197c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-3-list-all-namedlocations-created-after-a-certain-date"></a><span data-ttu-id="9197c-154">Exemplo 3: listar todos os namedLocations criados após uma determinada data</span><span class="sxs-lookup"><span data-stu-id="9197c-154">Example 3: List all namedLocations created after a certain date</span></span>

#### <a name="request"></a><span data-ttu-id="9197c-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9197c-155">Request</span></span>

<span data-ttu-id="9197c-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9197c-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9197c-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="9197c-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations?$filter=createdDateTime ge 2019-09-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="9197c-158">C#</span><span class="sxs-lookup"><span data-stu-id="9197c-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9197c-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9197c-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9197c-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9197c-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9197c-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="9197c-161">Response</span></span>

<span data-ttu-id="9197c-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9197c-162">The following is an example of the response.</span></span>

> <span data-ttu-id="9197c-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9197c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-4-list-all-countrynamedlocations-containing-a-certain-country-or-region"></a><span data-ttu-id="9197c-165">Exemplo 4: listar todos os countryNamedLocations contendo um determinado país ou região</span><span class="sxs-lookup"><span data-stu-id="9197c-165">Example 4: List all countryNamedLocations containing a certain country or region</span></span>

#### <a name="request"></a><span data-ttu-id="9197c-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9197c-166">Request</span></span>

<span data-ttu-id="9197c-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9197c-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9197c-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="9197c-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations?$filter=microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')
```
# <a name="c"></a>[<span data-ttu-id="9197c-169">C#</span><span class="sxs-lookup"><span data-stu-id="9197c-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9197c-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9197c-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9197c-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9197c-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9197c-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="9197c-172">Response</span></span>

<span data-ttu-id="9197c-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9197c-173">The following is an example of the response.</span></span>

> <span data-ttu-id="9197c-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9197c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
