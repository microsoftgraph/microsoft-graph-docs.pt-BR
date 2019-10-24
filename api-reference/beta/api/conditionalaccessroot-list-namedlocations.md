---
title: Listar namedLocations
description: Obtenha uma lista de objetos namedLocation.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4f5f7d52efa504df499e50cd3ebaa37359255493
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653808"
---
# <a name="list-namedlocations"></a><span data-ttu-id="72ddc-103">Listar namedLocations</span><span class="sxs-lookup"><span data-stu-id="72ddc-103">List namedLocations</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72ddc-104">Obtenha uma lista de objetos [namedLocation](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="72ddc-104">Get a list of [namedLocation](../resources/namedlocation.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="72ddc-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="72ddc-105">Permissions</span></span>

<span data-ttu-id="72ddc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72ddc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="72ddc-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72ddc-108">Permission type</span></span>                        | <span data-ttu-id="72ddc-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72ddc-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="72ddc-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72ddc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="72ddc-111">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="72ddc-111">Policy.Read.All</span></span> |
| <span data-ttu-id="72ddc-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72ddc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72ddc-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72ddc-113">Not supported.</span></span> |
| <span data-ttu-id="72ddc-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72ddc-114">Application</span></span>                            | <span data-ttu-id="72ddc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72ddc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="72ddc-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72ddc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /conditionalAccess/namedLocations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="72ddc-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="72ddc-117">Optional query parameters</span></span>

<span data-ttu-id="72ddc-118">Este método oferece suporte `$count`aos `$filter`parâmetros `$orderBy`de `$select`consulta `$skip`do, `$top` ,,, e OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="72ddc-118">This method supports the `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="72ddc-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="72ddc-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="72ddc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72ddc-120">Request headers</span></span>

| <span data-ttu-id="72ddc-121">Nome</span><span class="sxs-lookup"><span data-stu-id="72ddc-121">Name</span></span>      |<span data-ttu-id="72ddc-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="72ddc-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="72ddc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="72ddc-123">Authorization</span></span> | <span data-ttu-id="72ddc-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72ddc-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="72ddc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72ddc-126">Request body</span></span>

<span data-ttu-id="72ddc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="72ddc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="72ddc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="72ddc-128">Response</span></span>

<span data-ttu-id="72ddc-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [namedLocation](../resources/namedlocation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72ddc-129">If successful, this method returns a `200 OK` response code and a collection of [namedLocation](../resources/namedlocation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="72ddc-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="72ddc-130">Examples</span></span>

### <a name="example-1-list-all-namedlocations"></a><span data-ttu-id="72ddc-131">Exemplo 1: listar todos os namedLocations</span><span class="sxs-lookup"><span data-stu-id="72ddc-131">Example 1: List all namedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="72ddc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72ddc-132">Request</span></span>

<span data-ttu-id="72ddc-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="72ddc-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```http
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations
```

#### <a name="response"></a><span data-ttu-id="72ddc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="72ddc-134">Response</span></span>

<span data-ttu-id="72ddc-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="72ddc-135">The following is an example of the response.</span></span>

> <span data-ttu-id="72ddc-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72ddc-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-2-list-all-ipnamedlocations"></a><span data-ttu-id="72ddc-138">Exemplo 2: listar todos os ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="72ddc-138">Example 2: List all ipNamedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="72ddc-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72ddc-139">Request</span></span>

<span data-ttu-id="72ddc-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="72ddc-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```http
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations?$filter=isof('microsoft.graph.ipNamedLocation')
```

#### <a name="response"></a><span data-ttu-id="72ddc-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="72ddc-141">Response</span></span>

<span data-ttu-id="72ddc-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="72ddc-142">The following is an example of the response.</span></span>

> <span data-ttu-id="72ddc-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72ddc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-3-list-all-namedlocations-created-after-a-certain-date"></a><span data-ttu-id="72ddc-145">Exemplo 3: listar todos os namedLocations criados após uma determinada data</span><span class="sxs-lookup"><span data-stu-id="72ddc-145">Example 3: List all namedLocations created after a certain date</span></span>

#### <a name="request"></a><span data-ttu-id="72ddc-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72ddc-146">Request</span></span>

<span data-ttu-id="72ddc-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="72ddc-147">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```http
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations?$filter=createdDateTime ge 2019-09-01T00:00:00Z
```

#### <a name="response"></a><span data-ttu-id="72ddc-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="72ddc-148">Response</span></span>

<span data-ttu-id="72ddc-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="72ddc-149">The following is an example of the response.</span></span>

> <span data-ttu-id="72ddc-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72ddc-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
### <a name="example-4-list-all-countrynamedlocations-containing-a-certain-country-or-region"></a><span data-ttu-id="72ddc-152">Exemplo 4: listar todos os countryNamedLocations contendo um determinado país ou região</span><span class="sxs-lookup"><span data-stu-id="72ddc-152">Example 4: List all countryNamedLocations containing a certain country or region</span></span>

#### <a name="request"></a><span data-ttu-id="72ddc-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72ddc-153">Request</span></span>

<span data-ttu-id="72ddc-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="72ddc-154">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```http
GET https://graph.microsoft.com/beta/conditionalAccess/namedLocations?$filter=microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')
```

#### <a name="response"></a><span data-ttu-id="72ddc-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="72ddc-155">Response</span></span>

<span data-ttu-id="72ddc-156">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="72ddc-156">The following is an example of the response.</span></span>

> <span data-ttu-id="72ddc-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72ddc-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
