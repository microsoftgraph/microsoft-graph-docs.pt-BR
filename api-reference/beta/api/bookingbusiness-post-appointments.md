---
title: Criar bookingAppointment
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 1efde8ef8678afcee97939130e23b52312b03d83
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27936799"
---
# <a name="create-bookingappointment"></a><span data-ttu-id="0cdf2-104">Criar bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="0cdf2-104">Create bookingAppointment</span></span>

 > <span data-ttu-id="0cdf2-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0cdf2-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="0cdf2-107">Crie um novo [bookingAppointment](../resources/bookingappointment.md) para o especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="0cdf2-107">Create a new [bookingAppointment](../resources/bookingappointment.md) for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="0cdf2-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="0cdf2-108">Permissions</span></span>
<span data-ttu-id="0cdf2-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0cdf2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cdf2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0cdf2-111">Permission type</span></span>      | <span data-ttu-id="0cdf2-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0cdf2-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cdf2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0cdf2-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="0cdf2-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="0cdf2-114">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="0cdf2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0cdf2-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cdf2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-116">Not supported.</span></span>   |
|<span data-ttu-id="0cdf2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0cdf2-117">Application</span></span> | <span data-ttu-id="0cdf2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-118">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="0cdf2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0cdf2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/appointments

```
## <a name="request-headers"></a><span data-ttu-id="0cdf2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0cdf2-120">Request headers</span></span>
| <span data-ttu-id="0cdf2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="0cdf2-121">Name</span></span>       | <span data-ttu-id="0cdf2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cdf2-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0cdf2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0cdf2-123">Authorization</span></span>  | <span data-ttu-id="0cdf2-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="0cdf2-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cdf2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0cdf2-125">Request body</span></span>
<span data-ttu-id="0cdf2-126">No corpo da solicitação, fornece uma representação JSON do objeto [bookingAppointment](../resources/bookingappointment.md) .</span><span class="sxs-lookup"><span data-stu-id="0cdf2-126">In the request body, supply a JSON representation of [bookingAppointment](../resources/bookingappointment.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="0cdf2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cdf2-127">Response</span></span>
<span data-ttu-id="0cdf2-128">Se tiver êxito, este método retornará `201, Created` objeto response de código e [bookingAppointment](../resources/bookingappointment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-128">If successful, this method returns `201, Created` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cdf2-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0cdf2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0cdf2-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0cdf2-130">Request</span></span>
<span data-ttu-id="0cdf2-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-131">The following is an example of the request.</span></span> <span data-ttu-id="0cdf2-132">Este compromisso não envolve membros de equipe específico de reserva.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-132">This appointment does not involve booking specific staff members.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_bookingappointment_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments
Content-type: application/json

{
    "@odata.type":"#microsoft.graph.bookingAppointment",
    "customerEmailAddress":"jordanm@contoso.com",
    "customerLocation":{
        "@odata.type":"#microsoft.graph.location",
        "address":{
            "@odata.type":"#microsoft.graph.physicalAddress",
            "city":"Buffalo",
            "countryOrRegion":"USA",
            "postalCode":"98052",
            "postOfficeBox":null,
            "state":"NY",
            "street":"123 First Avenue",
            "type@odata.type":"#microsoft.graph.physicalAddressType",
            "type":null
        },
        "coordinates":null,
        "displayName":"Customer",
        "locationEmailAddress":null,
        "locationType@odata.type":"#microsoft.graph.locationType",
        "locationType":null,
        "locationUri":null,
        "uniqueId":null,
        "uniqueIdType@odata.type":"#microsoft.graph.locationUniqueIdType",
        "uniqueIdType":null
    },
    "customerName":"Jordan Miller",
    "customerNotes":"Please be on time.",
    "customerPhone":"213-555-0199",
    "end":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-01T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceAmount":10.0,
    "invoiceDate":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-01T12:30:00.0000000+00:00",
        "timeZone":"UTC"
    },
    "invoiceId":"1001",
    "invoiceStatus@odata.type":"#microsoft.graph.bookingInvoiceStatus",
    "invoiceStatus":"open",
    "invoiceUrl":"theInvoiceUrl",
    "optOutOfCustomerEmail":false,
    "postBuffer":"PT10M",
    "preBuffer":"PT5M",
    "price":10.0,
    "priceType@odata.type":"#microsoft.graph.bookingPriceType",
    "priceType":"fixedPrice",
    "reminders@odata.type":"#Collection(microsoft.graph.bookingReminder)",
    "reminders":[
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"This service is tomorrow",
            "offset":"P1D",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"allAttendees"
        },
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"Please be available to enjoy your lunch service.",
            "offset":"PT1H",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"customer"
        },
        {
            "@odata.type":"#microsoft.graph.bookingReminder",
            "message":"Please check traffic for next cater.",
            "offset":"PT2H",
            "recipients@odata.type":"#microsoft.graph.bookingReminderRecipients",
            "recipients":"staff"
        }
    ],
    "serviceId":"57da6774-a087-4d69-b0e6-6fb82c339976",
    "serviceLocation":{
        "@odata.type":"#microsoft.graph.location",
        "address":{
            "@odata.type":"#microsoft.graph.physicalAddress",
            "city":"Buffalo",
            "countryOrRegion":"USA",
            "postalCode":"98052",
            "postOfficeBox":null,
            "state":"NY",
            "street":"123 First Avenue",
            "type@odata.type":"#microsoft.graph.physicalAddressType",
            "type":null
        },
        "coordinates":null,
        "displayName":"Customer location",
        "locationEmailAddress":null,
        "locationType@odata.type":"#microsoft.graph.locationType",
        "locationType":null,
        "locationUri":null,
        "uniqueId":null,
        "uniqueIdType@odata.type":"#microsoft.graph.locationUniqueIdType",
        "uniqueIdType":null
    },
    "serviceName":"Catered bento",
    "serviceNotes":"Customer requires punctual service.",
    "start":{
        "@odata.type":"#microsoft.graph.dateTimeTimeZone",
        "dateTime":"2018-05-01T12:00:00.0000000+00:00",
        "timeZone":"UTC"
    }
}
```
<span data-ttu-id="0cdf2-133">No corpo da solicitação, fornece uma representação JSON do objeto [bookingAppointment](../resources/bookingappointment.md) .</span><span class="sxs-lookup"><span data-stu-id="0cdf2-133">In the request body, supply a JSON representation of [bookingAppointment](../resources/bookingappointment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0cdf2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0cdf2-134">Response</span></span>
<span data-ttu-id="0cdf2-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-135">The following is an example of the response.</span></span> <span data-ttu-id="0cdf2-136">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0cdf2-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0cdf2-137">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/appointments/$entity",
    "id": "AAMkADc7zF4J0AAA8v_KnAAA=",
    "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
    "customerId": "7ed53fa5-9ef2-4f2f-975b-27447440bc09",
    "customerName": "Jordan Miller",
    "customerEmailAddress": "jordanm@contoso.com",
    "customerPhone": "213-555-0199",
    "customerNotes": null,
    "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976",
    "serviceName": "Catered bento",
    "duration": "PT30M",
    "preBuffer": "PT5M",
    "postBuffer": "PT10M",
    "priceType": "fixedPrice",
    "price": 10,
    "serviceNotes": "Customer requires punctual service.",
    "optOutOfCustomerEmail": false,
    "staffMemberIds": [],
    "invoiceAmount": 10,
    "invoiceId": "1001",
    "invoiceStatus": "open",
    "invoiceUrl": "theInvoiceUrl",
    "customerLocation": {
        "displayName": "Customer",
        "locationEmailAddress": null,
        "locationUri": "",
        "locationType": null,
        "uniqueId": null,
        "uniqueIdType": null,
        "address": {
            "type": "home",
            "postOfficeBox": "",
            "street": "",
            "city": "",
            "state": "",
            "countryOrRegion": "",
            "postalCode": ""
        },
        "coordinates": {
            "altitude": null,
            "latitude": null,
            "longitude": null,
            "accuracy": null,
            "altitudeAccuracy": null
        }
    },
    "start": {
        "dateTime": "2018-05-01T12:00:00.0000000Z",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2018-05-01T12:30:00.0000000Z",
        "timeZone": "UTC"
    },
    "serviceLocation": {
        "displayName": "Customer location (123 First Avenue, Buffalo, NY 98052, USA)",
        "locationEmailAddress": null,
        "locationUri": "",
        "locationType": null,
        "uniqueId": null,
        "uniqueIdType": null,
        "address": {
            "type": "home",
            "postOfficeBox": "",
            "street": "",
            "city": "",
            "state": "",
            "countryOrRegion": "",
            "postalCode": ""
        },
        "coordinates": {
            "altitude": null,
            "latitude": null,
            "longitude": null,
            "accuracy": null,
            "altitudeAccuracy": null
        }
    },
    "reminders": [
        {
            "offset": "P1D",
            "recipients": "allAttendees",
            "message": "This service is tomorrow"
        },
        {
            "offset": "PT1H",
            "recipients": "customer",
            "message": "Please be available to enjoy your lunch service."
        },
        {
            "offset": "PT2H",
            "recipients": "staff",
            "message": "Please check traffic for next cater."
        }
    ],
    "invoiceDate": {
        "dateTime": "2018-05-01T12:30:00.0000000Z",
        "timeZone": "UTC"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
