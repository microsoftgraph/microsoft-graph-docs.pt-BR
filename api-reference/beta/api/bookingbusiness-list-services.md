---
title: Listar serviços
description: Obtenha uma lista de objetos bookingService no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 0137e4c2d598baa21fe2b382c41636b84cfeb6ab
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718860"
---
# <a name="list-services"></a><span data-ttu-id="a5cdd-103">Listar serviços</span><span class="sxs-lookup"><span data-stu-id="a5cdd-103">List services</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5cdd-104">Obtenha uma lista de objetos [bookingService](../resources/bookingservice.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="a5cdd-104">Get a list of [bookingService](../resources/bookingservice.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a5cdd-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a5cdd-105">Permissions</span></span>
<span data-ttu-id="a5cdd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a5cdd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a5cdd-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5cdd-108">Permission type</span></span>      | <span data-ttu-id="a5cdd-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5cdd-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5cdd-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5cdd-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a5cdd-111">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="a5cdd-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="a5cdd-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5cdd-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5cdd-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5cdd-113">Not supported.</span></span>   |
|<span data-ttu-id="a5cdd-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5cdd-114">Application</span></span> | <span data-ttu-id="a5cdd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a5cdd-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="a5cdd-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5cdd-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a5cdd-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a5cdd-117">Optional query parameters</span></span>
<span data-ttu-id="a5cdd-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a5cdd-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5cdd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5cdd-119">Request headers</span></span>
| <span data-ttu-id="a5cdd-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a5cdd-120">Name</span></span>      |<span data-ttu-id="a5cdd-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5cdd-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a5cdd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5cdd-122">Authorization</span></span>  | <span data-ttu-id="a5cdd-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a5cdd-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5cdd-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5cdd-124">Request body</span></span>
<span data-ttu-id="a5cdd-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a5cdd-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a5cdd-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5cdd-126">Response</span></span>
<span data-ttu-id="a5cdd-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [bookingService](../resources/bookingservice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5cdd-127">If successful, this method returns a `200 OK` response code and collection of [bookingService](../resources/bookingservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a5cdd-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a5cdd-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a5cdd-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5cdd-129">Request</span></span>
<span data-ttu-id="a5cdd-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5cdd-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a5cdd-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5cdd-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_services"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a5cdd-132">C#</span><span class="sxs-lookup"><span data-stu-id="a5cdd-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-services-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a5cdd-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5cdd-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-services-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a5cdd-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="a5cdd-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-services-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a5cdd-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5cdd-135">Response</span></span>
<span data-ttu-id="a5cdd-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a5cdd-136">The following is an example of the response.</span></span> <span data-ttu-id="a5cdd-137">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="a5cdd-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="a5cdd-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a5cdd-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingService",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/services",
    "value": [
        {
            "id": "f9b9121f-aed7-4c8c-bb3a-a1796a0b0b2d",
            "displayName": "Initial service",
            "defaultDuration": "PT10M",
            "defaultPrice": 0,
            "defaultPriceType": "notSet",
            "description": "Not sure how to choose? Let us introduce you to our traditional family recipes.",
            "isHiddenFromCustomers": false,
            "notes": "This is where you can add notes about this service that only you and your staff see.",
            "preBuffer": "PT0S",
            "postBuffer": "PT0S",
            "staffMemberIds": [],
            "schedulingPolicy": null,
            "defaultLocation": {
                "displayName": "Contoso Lunch Delivery",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "type": "home",
                    "postOfficeBox": "",
                    "street": "4567 First Street",
                    "city": "Buffalo",
                    "state": "NY",
                    "countryOrRegion": "USA",
                    "postalCode": "98052"
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "defaultReminders": []
        },
        {
            "id": "57da6774-a087-4d69-b0e6-6fb82c339976",
            "displayName": "Catered bento",
            "defaultDuration": "PT30M",
            "defaultPrice": 10,
            "defaultPriceType": "fixedPrice",
            "description": "Catered individual bento box lunch",
            "isHiddenFromCustomers": false,
            "notes": "Home-cooked special",
            "preBuffer": "PT5M",
            "postBuffer": "PT10M",
            "staffMemberIds": [],
            "defaultLocation": {
                "displayName": "Contoso Lunch Delivery",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "type": "home",
                    "postOfficeBox": "",
                    "street": "4567 First Street",
                    "city": "Buffalo",
                    "state": "NY",
                    "countryOrRegion": "USA",
                    "postalCode": "98052"
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "defaultReminders": [],
            "schedulingPolicy": {
                "timeSlotInterval": "PT1H",
                "minimumLeadTime": "PT10H",
                "maximumAdvance": "P10D",
                "sendConfirmationsToOwner": true,
                "allowStaffSelection": true
            }
        },
        {
            "id": "635a7b7c-4230-4d3b-a42b-698e89927528",
            "displayName": "Kaiseki",
            "defaultDuration": "PT1H30M",
            "defaultPrice": 30,
            "defaultPriceType": "fixedPrice",
            "description": "Individual kaiseki lunch delivery",
            "isHiddenFromCustomers": false,
            "notes": "Home-cooked special",
            "preBuffer": "PT5M",
            "postBuffer": "PT10M",
            "staffMemberIds": [],
            "defaultLocation": {
                "displayName": "Contoso Lunch Delivery",
                "locationEmailAddress": null,
                "locationUri": "",
                "locationType": null,
                "uniqueId": null,
                "uniqueIdType": null,
                "address": {
                    "type": "home",
                    "postOfficeBox": "",
                    "street": "4567 First Street",
                    "city": "Buffalo",
                    "state": "NY",
                    "countryOrRegion": "USA",
                    "postalCode": "98052"
                },
                "coordinates": {
                    "altitude": null,
                    "latitude": null,
                    "longitude": null,
                    "accuracy": null,
                    "altitudeAccuracy": null
                }
            },
            "defaultReminders": [],
            "schedulingPolicy": {
                "timeSlotInterval": "PT1H",
                "minimumLeadTime": "PT10H",
                "maximumAdvance": "P10D",
                "sendConfirmationsToOwner": true,
                "allowStaffSelection": true
            }
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List services",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
