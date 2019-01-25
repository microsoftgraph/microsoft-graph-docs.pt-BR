---
title: Criar bookingService
description: Crie um novo bookingService para o bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 50501ac1dd79b41b9e970f870964fffaace2f8da
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516109"
---
# <a name="create-bookingservice"></a><span data-ttu-id="3740e-103">Criar bookingService</span><span class="sxs-lookup"><span data-stu-id="3740e-103">Create bookingService</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3740e-104">Crie um novo [bookingService](../resources/bookingservice.md) para o especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="3740e-104">Create a new [bookingService](../resources/bookingservice.md) for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="3740e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3740e-105">Permissions</span></span>
<span data-ttu-id="3740e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3740e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3740e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3740e-108">Permission type</span></span>      | <span data-ttu-id="3740e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3740e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3740e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3740e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="3740e-111">Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="3740e-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="3740e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3740e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3740e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3740e-113">Not supported.</span></span>   |
|<span data-ttu-id="3740e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3740e-114">Application</span></span> | <span data-ttu-id="3740e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3740e-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3740e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3740e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/services

```
## <a name="request-headers"></a><span data-ttu-id="3740e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3740e-117">Request headers</span></span>
| <span data-ttu-id="3740e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="3740e-118">Name</span></span>       | <span data-ttu-id="3740e-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="3740e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3740e-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="3740e-120">Authorization</span></span>  | <span data-ttu-id="3740e-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="3740e-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="3740e-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3740e-122">Request body</span></span>
<span data-ttu-id="3740e-123">No corpo da solicitação, fornece uma representação JSON do objeto [bookingService](../resources/bookingservice.md) .</span><span class="sxs-lookup"><span data-stu-id="3740e-123">In the request body, supply a JSON representation of [bookingService](../resources/bookingservice.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="3740e-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="3740e-124">Response</span></span>
<span data-ttu-id="3740e-125">Se tiver êxito, este método retornará `201, Created` objeto response de código e [bookingService](../resources/bookingservice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3740e-125">If successful, this method returns `201, Created` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3740e-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3740e-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3740e-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3740e-127">Request</span></span>
<span data-ttu-id="3740e-128">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3740e-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingservice_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingService",
    "defaultDuration":"PT1H30M",
    "defaultLocation":{
        "@odata.type":"#microsoft.graph.location",
        "address":{
            "@odata.type":"#microsoft.graph.physicalAddress",
            "city":"Buffalo",
            "countryOrRegion":"USA",
            "postalCode":"98052",
            "postOfficeBox":null,
            "state":"NY",
            "street":"4567 First Street",
            "type@odata.type":"#microsoft.graph.physicalAddressType",
            "type":null
        },
        "coordinates":null,
        "displayName":"Contoso Lunch Delivery",
        "locationEmailAddress":null,
        "locationType@odata.type":"#microsoft.graph.locationType",
        "locationType":null,
        "locationUri":null,
        "uniqueId":null,
        "uniqueIdType@odata.type":"#microsoft.graph.locationUniqueIdType",
        "uniqueIdType":null
    },
    "defaultPrice":10.0,
    "defaultPriceType@odata.type":"#microsoft.graph.bookingPriceType",
    "defaultPriceType":"fixedPrice",
    "defaultReminders@odata.type":"#Collection(microsoft.graph.bookingReminder)",
    "defaultReminders":[
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"Please be reminded that this service is tomorrow.",
            "offset":"P1D",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"allAttendees"
        }
    ],
    "description":"Individual bento box lunch delivery",
    "displayName":"Bento",
    "isHiddenFromCustomers":false,
    "notes":"Home-cooked special",
    "postBuffer":"PT10M",
    "preBuffer":"PT5M",
    "schedulingPolicy":{
        "@odata.type":"#microsoft.graph.bookingSchedulingPolicy",
        "allowStaffSelection":true,
        "maximumAdvance":"P10D",
        "minimumLeadTime":"PT10H",
        "sendConfirmationsToOwner":true,
        "timeSlotInterval":"PT1H"
    },
    "staffMemberIds@odata.type":"#Collection(String)",
    "staffMemberIds":[
        "d90d1e8c-5cfe-48cf-a2d5-966267375b6a",
        "2f5f8794-0b29-45b5-b56a-2eb5ff7aa880"
    ]
}
```
<span data-ttu-id="3740e-129">No corpo da solicitação, fornece uma representação JSON do objeto [bookingService](../resources/bookingservice.md) .</span><span class="sxs-lookup"><span data-stu-id="3740e-129">In the request body, supply a JSON representation of [bookingService](../resources/bookingservice.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3740e-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3740e-130">Response</span></span>
<span data-ttu-id="3740e-131">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3740e-131">The following is an example of the response.</span></span> <span data-ttu-id="3740e-132">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="3740e-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3740e-133">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3740e-133">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingService"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/services/$entity",
    "id": "57da6774-a087-4d69-b0e6-6fb82c339976",
    "displayName": "Bento",
    "defaultDuration": "PT1H30M",
    "defaultPrice": 10,
    "defaultPriceType": "fixedPrice",
    "description": "Individual bento box lunch delivery",
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
    "defaultReminders": [
        {
            "offset": "P1D",
            "recipients": "allAttendees",
            "message": "Please be reminded that this service is tomorrow."
        }
    ],
    "schedulingPolicy": {
        "timeSlotInterval": "PT1H",
        "minimumLeadTime": "PT10H",
        "maximumAdvance": "P10D",
        "sendConfirmationsToOwner": true,
        "allowStaffSelection": true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-post-services.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
