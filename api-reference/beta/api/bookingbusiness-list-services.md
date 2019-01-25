---
title: Lista de serviços
description: Obtenha uma lista de objetos bookingService no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 0571f7c57d2ee37b3095de3e3568cf906c17a987
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511608"
---
# <a name="list-services"></a><span data-ttu-id="67bd9-103">Lista de serviços</span><span class="sxs-lookup"><span data-stu-id="67bd9-103">List services</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67bd9-104">Obtenha uma lista de objetos [bookingService](../resources/bookingservice.md) no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="67bd9-104">Get a list of [bookingService](../resources/bookingservice.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="67bd9-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="67bd9-105">Permissions</span></span>
<span data-ttu-id="67bd9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67bd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67bd9-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67bd9-108">Permission type</span></span>      | <span data-ttu-id="67bd9-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67bd9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67bd9-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67bd9-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="67bd9-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="67bd9-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="67bd9-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67bd9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67bd9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67bd9-113">Not supported.</span></span>   |
|<span data-ttu-id="67bd9-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67bd9-114">Application</span></span> | <span data-ttu-id="67bd9-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67bd9-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="67bd9-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67bd9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services
```
## <a name="optional-query-parameters"></a><span data-ttu-id="67bd9-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="67bd9-117">Optional query parameters</span></span>
<span data-ttu-id="67bd9-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="67bd9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67bd9-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67bd9-119">Request headers</span></span>
| <span data-ttu-id="67bd9-120">Nome</span><span class="sxs-lookup"><span data-stu-id="67bd9-120">Name</span></span>      |<span data-ttu-id="67bd9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="67bd9-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="67bd9-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="67bd9-122">Authorization</span></span>  | <span data-ttu-id="67bd9-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="67bd9-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="67bd9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67bd9-124">Request body</span></span>
<span data-ttu-id="67bd9-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="67bd9-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="67bd9-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="67bd9-126">Response</span></span>
<span data-ttu-id="67bd9-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [bookingService](../resources/bookingservice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67bd9-127">If successful, this method returns a `200 OK` response code and collection of [bookingService](../resources/bookingservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="67bd9-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67bd9-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67bd9-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67bd9-129">Request</span></span>
<span data-ttu-id="67bd9-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="67bd9-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_services"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services
```
##### <a name="response"></a><span data-ttu-id="67bd9-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="67bd9-131">Response</span></span>
<span data-ttu-id="67bd9-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="67bd9-132">The following is an example of the response.</span></span> <span data-ttu-id="67bd9-133">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="67bd9-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="67bd9-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67bd9-134">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingbusiness-list-services.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
