---
title: Listar namedLocations
description: Obtenha uma lista de objetos namedLocation.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f329c79b1c8a092f53daa22f2c1228f77d810278
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384415"
---
# <a name="list-namedlocations"></a><span data-ttu-id="ec823-103">Listar namedLocations</span><span class="sxs-lookup"><span data-stu-id="ec823-103">List namedLocations</span></span>

<span data-ttu-id="ec823-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec823-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ec823-105">Obtenha uma lista de objetos [namedLocation](../resources/namedlocation.md) .</span><span class="sxs-lookup"><span data-stu-id="ec823-105">Get a list of [namedLocation](../resources/namedlocation.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec823-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="ec823-106">Permissions</span></span>

<span data-ttu-id="ec823-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ec823-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ec823-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ec823-109">Permission type</span></span>                        | <span data-ttu-id="ec823-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ec823-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ec823-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ec823-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ec823-112">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec823-112">Policy.Read.All</span></span> |
| <span data-ttu-id="ec823-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ec823-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec823-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ec823-114">Not supported.</span></span> |
| <span data-ttu-id="ec823-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ec823-115">Application</span></span>                            | <span data-ttu-id="ec823-116">Policy.Read.All</span><span class="sxs-lookup"><span data-stu-id="ec823-116">Policy.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec823-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ec823-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/conditionalAccess/namedLocations
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ec823-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ec823-118">Optional query parameters</span></span>

<span data-ttu-id="ec823-119">Este método oferece suporte aos parâmetros de consulta do,,, `$count` `$filter` `$orderBy` `$select` , `$skip` e `$top` OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ec823-119">This method supports the `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="ec823-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ec823-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ec823-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ec823-121">Request headers</span></span>

| <span data-ttu-id="ec823-122">Nome</span><span class="sxs-lookup"><span data-stu-id="ec823-122">Name</span></span>      |<span data-ttu-id="ec823-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec823-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ec823-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="ec823-124">Authorization</span></span> | <span data-ttu-id="ec823-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ec823-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec823-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ec823-127">Request body</span></span>

<span data-ttu-id="ec823-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ec823-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ec823-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec823-129">Response</span></span>

<span data-ttu-id="ec823-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [namedLocation](../resources/namedlocation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ec823-130">If successful, this method returns a `200 OK` response code and a collection of [namedLocation](../resources/namedlocation.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ec823-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="ec823-131">Examples</span></span>

### <a name="example-1-list-all-namedlocations"></a><span data-ttu-id="ec823-132">Exemplo 1: listar todos os namedLocations</span><span class="sxs-lookup"><span data-stu-id="ec823-132">Example 1: List all namedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="ec823-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec823-133">Request</span></span>

<span data-ttu-id="ec823-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec823-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```http
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations
```

#### <a name="response"></a><span data-ttu-id="ec823-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec823-135">Response</span></span>

<span data-ttu-id="ec823-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ec823-136">The following is an example of the response.</span></span>

> <span data-ttu-id="ec823-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec823-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/namedLocations",
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
### <a name="example-2-list-all-ipnamedlocations"></a><span data-ttu-id="ec823-139">Exemplo 2: listar todos os ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="ec823-139">Example 2: List all ipNamedLocations</span></span>

#### <a name="request"></a><span data-ttu-id="ec823-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec823-140">Request</span></span>

<span data-ttu-id="ec823-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec823-141">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```http
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations?$filter=isof('microsoft.graph.ipNamedLocation')
```

#### <a name="response"></a><span data-ttu-id="ec823-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec823-142">Response</span></span>

<span data-ttu-id="ec823-143">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ec823-143">The following is an example of the response.</span></span>

> <span data-ttu-id="ec823-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec823-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/namedLocations",
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
### <a name="example-3-list-all-namedlocations-created-after-a-certain-date"></a><span data-ttu-id="ec823-146">Exemplo 3: listar todos os namedLocations criados após uma determinada data</span><span class="sxs-lookup"><span data-stu-id="ec823-146">Example 3: List all namedLocations created after a certain date</span></span>

#### <a name="request"></a><span data-ttu-id="ec823-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec823-147">Request</span></span>

<span data-ttu-id="ec823-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec823-148">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```http
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations?$filter=createdDateTime ge 2019-09-01T00:00:00Z
```

#### <a name="response"></a><span data-ttu-id="ec823-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec823-149">Response</span></span>

<span data-ttu-id="ec823-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ec823-150">The following is an example of the response.</span></span>

> <span data-ttu-id="ec823-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec823-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/namedLocations",
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
### <a name="example-4-list-all-countrynamedlocations-containing-a-certain-country-or-region"></a><span data-ttu-id="ec823-153">Exemplo 4: listar todos os countryNamedLocations contendo um determinado país ou região</span><span class="sxs-lookup"><span data-stu-id="ec823-153">Example 4: List all countryNamedLocations containing a certain country or region</span></span>

#### <a name="request"></a><span data-ttu-id="ec823-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ec823-154">Request</span></span>

<span data-ttu-id="ec823-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="ec823-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_namedlocations"
}-->

```http
GET https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations?$filter=microsoft.graph.countryNamedLocation/countriesAndRegions/any(c: c eq 'CA')
```

#### <a name="response"></a><span data-ttu-id="ec823-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="ec823-156">Response</span></span>

<span data-ttu-id="ec823-157">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="ec823-157">The following is an example of the response.</span></span>

> <span data-ttu-id="ec823-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ec823-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#conditionalAccess/namedLocations",
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
