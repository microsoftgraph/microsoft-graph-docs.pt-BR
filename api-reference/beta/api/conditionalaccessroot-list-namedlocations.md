---
title: Listar namedLocations
description: Obter uma lista de objetos namedLocation.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4a99ea9698154ff6c89c7832d0ad083e71541ac1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947400"
---
# <a name="list-namedlocations"></a><span data-ttu-id="58bd2-103">Listar namedLocations</span><span class="sxs-lookup"><span data-stu-id="58bd2-103">List namedLocations</span></span>

<span data-ttu-id="58bd2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58bd2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58bd2-105">Obter uma lista de [objetos namedLocation.](../resources/namedlocation.md)</span><span class="sxs-lookup"><span data-stu-id="58bd2-105">Get a list of [namedLocation](../resources/namedlocation.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="58bd2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="58bd2-106">Permissions</span></span>

<span data-ttu-id="58bd2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58bd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="58bd2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58bd2-109">Permission type</span></span>                        | <span data-ttu-id="58bd2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58bd2-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="58bd2-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58bd2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="58bd2-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="58bd2-112">Policy.Read.All</span></span> |
| <span data-ttu-id="58bd2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58bd2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58bd2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58bd2-114">Not supported.</span></span> |
| <span data-ttu-id="58bd2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58bd2-115">Application</span></span>                            | <span data-ttu-id="58bd2-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="58bd2-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58bd2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58bd2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/namedLocations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="58bd2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="58bd2-118">Optional query parameters</span></span>

<span data-ttu-id="58bd2-119">Este método dá suporte aos parâmetros de consulta , , , , e OData para `$count` ajudar a personalizar a `$filter` `$orderBy` `$select` `$skip` `$top` resposta.</span><span class="sxs-lookup"><span data-stu-id="58bd2-119">This method supports the `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="58bd2-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="58bd2-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="58bd2-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58bd2-121">Request headers</span></span>

| <span data-ttu-id="58bd2-122">Nome</span><span class="sxs-lookup"><span data-stu-id="58bd2-122">Name</span></span>      |<span data-ttu-id="58bd2-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="58bd2-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="58bd2-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="58bd2-124">Authorization</span></span> | <span data-ttu-id="58bd2-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58bd2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58bd2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58bd2-127">Request body</span></span>

<span data-ttu-id="58bd2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="58bd2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="58bd2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="58bd2-129">Response</span></span>

<span data-ttu-id="58bd2-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos namedLocation](../resources/namedlocation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58bd2-130">If successful, this method returns a `200 OK` response code and a collection of [namedLocation](../resources/namedlocation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="58bd2-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="58bd2-131">Examples</span></span>

### <a name="example-1-list-all-namedlocations"></a><span data-ttu-id="58bd2-132">Exemplo 1: Listar todos os namedLocations</span><span class="sxs-lookup"><span data-stu-id="58bd2-132">Example 1: List all namedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="58bd2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58bd2-133">Request</span></span>

<span data-ttu-id="58bd2-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="58bd2-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="58bd2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="58bd2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations
```
# <a name="c"></a>[<span data-ttu-id="58bd2-136">C#</span><span class="sxs-lookup"><span data-stu-id="58bd2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58bd2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58bd2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58bd2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58bd2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58bd2-139">Java</span><span class="sxs-lookup"><span data-stu-id="58bd2-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-namedlocations-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="58bd2-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="58bd2-140">Response</span></span>

<span data-ttu-id="58bd2-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="58bd2-141">The following is an example of the response.</span></span>

> <span data-ttu-id="58bd2-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58bd2-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-list-all-ipnamedlocations"></a><span data-ttu-id="58bd2-144">Exemplo 2: Listar todos os ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="58bd2-144">Example 2: List all ipNamedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="58bd2-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58bd2-145">Request</span></span>

<span data-ttu-id="58bd2-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="58bd2-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="58bd2-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="58bd2-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations?$filter=isof('microsoft.graph.ipNamedLocation')
```
# <a name="c"></a>[<span data-ttu-id="58bd2-148">C#</span><span class="sxs-lookup"><span data-stu-id="58bd2-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58bd2-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58bd2-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58bd2-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58bd2-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58bd2-151">Java</span><span class="sxs-lookup"><span data-stu-id="58bd2-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-namedlocations-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="58bd2-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="58bd2-152">Response</span></span>

<span data-ttu-id="58bd2-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="58bd2-153">The following is an example of the response.</span></span>

> <span data-ttu-id="58bd2-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58bd2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-3-list-all-namedlocations-created-after-a-certain-date"></a><span data-ttu-id="58bd2-156">Exemplo 3: Listar todos os namedLocations criados após uma determinada data</span><span class="sxs-lookup"><span data-stu-id="58bd2-156">Example 3: List all namedLocations created after a certain date</span></span>

#### <a name="request"></a><span data-ttu-id="58bd2-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58bd2-157">Request</span></span>

<span data-ttu-id="58bd2-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="58bd2-158">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="58bd2-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="58bd2-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations_3"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations?$filter=createdDateTime ge 2019-09-01T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="58bd2-160">C#</span><span class="sxs-lookup"><span data-stu-id="58bd2-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-3-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58bd2-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58bd2-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-3-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58bd2-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58bd2-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-3-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58bd2-163">Java</span><span class="sxs-lookup"><span data-stu-id="58bd2-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-namedlocations-3-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="58bd2-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="58bd2-164">Response</span></span>

<span data-ttu-id="58bd2-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="58bd2-165">The following is an example of the response.</span></span>

> <span data-ttu-id="58bd2-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58bd2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-4-list-all-countrynamedlocations-containing-a-certain-country-or-region"></a><span data-ttu-id="58bd2-168">Exemplo 4: listar todos os countryNamedLocations que contêm um determinado país ou região</span><span class="sxs-lookup"><span data-stu-id="58bd2-168">Example 4: List all countryNamedLocations containing a certain country or region</span></span>

#### <a name="request"></a><span data-ttu-id="58bd2-169">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58bd2-169">Request</span></span>

<span data-ttu-id="58bd2-170">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="58bd2-170">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="58bd2-171">HTTP</span><span class="sxs-lookup"><span data-stu-id="58bd2-171">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_namedlocations_4"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identity/conditionalAccess/namedLocations?$filter=microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')
```
# <a name="c"></a>[<span data-ttu-id="58bd2-172">C#</span><span class="sxs-lookup"><span data-stu-id="58bd2-172">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-namedlocations-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="58bd2-173">JavaScript</span><span class="sxs-lookup"><span data-stu-id="58bd2-173">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-namedlocations-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="58bd2-174">Objective-C</span><span class="sxs-lookup"><span data-stu-id="58bd2-174">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-namedlocations-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="58bd2-175">Java</span><span class="sxs-lookup"><span data-stu-id="58bd2-175">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-namedlocations-4-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="58bd2-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="58bd2-176">Response</span></span>

<span data-ttu-id="58bd2-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="58bd2-177">The following is an example of the response.</span></span>

> <span data-ttu-id="58bd2-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58bd2-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


