---
title: Lista reservas calendarView
description: Obtenha a coleção de objetos bookingAppointment para um bookingBusiness, o que ocorre no intervalo de datas especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 39b96e089d035ffd21155064252e36fd07a0a6c5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526071"
---
# <a name="list-bookings-calendarview"></a><span data-ttu-id="8cf86-103">Lista reservas calendarView</span><span class="sxs-lookup"><span data-stu-id="8cf86-103">List Bookings calendarView</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cf86-104">Obtenha a coleção de objetos [bookingAppointment](../resources/bookingappointment.md) para um [bookingBusiness](../resources/bookingbusiness.md), que ocorre no intervalo de datas especificado.</span><span class="sxs-lookup"><span data-stu-id="8cf86-104">Get the collection of [bookingAppointment](../resources/bookingappointment.md) objects for a [bookingBusiness](../resources/bookingbusiness.md), that occurs in the specified date range.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cf86-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="8cf86-105">Permissions</span></span>
<span data-ttu-id="8cf86-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cf86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cf86-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8cf86-108">Permission type</span></span>      | <span data-ttu-id="8cf86-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8cf86-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8cf86-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8cf86-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="8cf86-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="8cf86-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="8cf86-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8cf86-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cf86-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cf86-113">Not supported.</span></span>   |
|<span data-ttu-id="8cf86-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8cf86-114">Application</span></span> | <span data-ttu-id="8cf86-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8cf86-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="8cf86-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8cf86-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/calendarView?start={start-value}&end={end-value}

```
## <a name="request-headers"></a><span data-ttu-id="8cf86-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8cf86-117">Request headers</span></span>
| <span data-ttu-id="8cf86-118">Nome</span><span class="sxs-lookup"><span data-stu-id="8cf86-118">Name</span></span>       | <span data-ttu-id="8cf86-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cf86-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8cf86-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="8cf86-120">Authorization</span></span>  | <span data-ttu-id="8cf86-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="8cf86-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cf86-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8cf86-122">Request body</span></span>
<span data-ttu-id="8cf86-123">Forneça os seguintes parâmetros de consulta com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="8cf86-123">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="8cf86-124">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="8cf86-124">Parameter</span></span>    | <span data-ttu-id="8cf86-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cf86-125">Type</span></span>   |<span data-ttu-id="8cf86-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cf86-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cf86-127">start</span><span class="sxs-lookup"><span data-stu-id="8cf86-127">start</span></span>|<span data-ttu-id="8cf86-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cf86-128">DateTimeOffset</span></span>|<span data-ttu-id="8cf86-129">A data de início e a hora de um intervalo de tempo, representados no formato ISO 8601, como UTC ou deslocamento do UTC.</span><span class="sxs-lookup"><span data-stu-id="8cf86-129">The start date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="8cf86-130">Por exemplo, meia-noite UTC em 1 de Jan de 2018, ficaria assim: ' 2018-01-01T00:00:00Z', e o mesmo tempo no PST ficaria assim: ' 2017-12-31T16:00:00-08:00 '.</span><span class="sxs-lookup"><span data-stu-id="8cf86-130">For example, midnight UTC on Jan 1, 2018 would look like this: '2018-01-01T00:00:00Z', and the same time in PST would look like this: '2017-12-31T16:00:00-08:00'.</span></span>|
|<span data-ttu-id="8cf86-131">end</span><span class="sxs-lookup"><span data-stu-id="8cf86-131">end</span></span>|<span data-ttu-id="8cf86-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cf86-132">DateTimeOffset</span></span>|<span data-ttu-id="8cf86-133">A data de término e a hora de um intervalo de tempo, representados no formato ISO 8601, como UTC ou deslocamento do UTC.</span><span class="sxs-lookup"><span data-stu-id="8cf86-133">The end date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="8cf86-134">Por exemplo, 3 am UTC em 1 de Jan de 2018, ficaria assim: ' 2018-01-01T03:00:00Z', e o mesmo tempo no PST ficaria assim: ' 2017-12-31T19:00:00-08:00 '.</span><span class="sxs-lookup"><span data-stu-id="8cf86-134">For example, 3am UTC on Jan 1, 2018 would look like this: '2018-01-01T03:00:00Z', and the same time in PST would look like this: '2017-12-31T19:00:00-08:00'.</span></span>|

## <a name="response"></a><span data-ttu-id="8cf86-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cf86-135">Response</span></span>
<span data-ttu-id="8cf86-136">Se tiver êxito, este método retornará `200, OK` objeto de coleção [bookingAppointment](../resources/bookingappointment.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8cf86-136">If successful, this method returns `200, OK` response code and [bookingAppointment](../resources/bookingappointment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cf86-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8cf86-137">Example</span></span>
<span data-ttu-id="8cf86-138">Este é um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="8cf86-138">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="8cf86-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8cf86-139">Request</span></span>
<span data-ttu-id="8cf86-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8cf86-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getcalendarview"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/calendarView?start=2018-04-30T00:00:00Z&end=2018-05-10T00:00:00Z
```

##### <a name="response"></a><span data-ttu-id="8cf86-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="8cf86-141">Response</span></span>
<span data-ttu-id="8cf86-142">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8cf86-142">The following is an example of the response.</span></span> <span data-ttu-id="8cf86-143">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="8cf86-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8cf86-144">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8cf86-144">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/calendarView",
    "value": [
        {
            "id": "AAMkADKpAAA=",
            "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
            "customerId": "80b5ddda-1e3b-4c9d-abe2-d606cc075e2e",
            "customerName": "Adele Vance",
            "customerEmailAddress": "adelev@proseware.com",
            "customerPhone": "213-555-0156",
            "customerNotes": null,
            "serviceId": "57da6774-a087-4d69-b0e6-6fb82c339976",
            "serviceName": "Catered bento",
            "duration": "PT30M",
            "preBuffer": "PT5M",
            "postBuffer": "PT10M",
            "priceType": "fixedPrice",
            "price": 10,
            "serviceNotes": null,
            "optOutOfCustomerEmail": false,
            "staffMemberIds": [],
            "invoiceAmount": 10,
            "invoiceId": "1003",
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
                "dateTime": "2018-05-05T12:00:00.0000000Z",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2018-05-05T12:30:00.0000000Z",
                "timeZone": "UTC"
            },
            "serviceLocation": {
                "displayName": "Customer location (876 Tenth Avenue, Buffalo, NY 98052, USA)",
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
            "reminders": [],
            "invoiceDate": {
                "dateTime": "2018-05-05T12:30:00.0000000Z",
                "timeZone": "UTC"
            }
        },
        {
            "id": "AAMkADKnAAA=",
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
            "serviceNotes": null,
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
                "dateTime": "2018-05-06T12:00:00.0000000Z",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2018-05-06T12:30:00.0000000Z",
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
            "reminders": [],
            "invoiceDate": {
                "dateTime": "2018-05-06T12:30:00.0000000Z",
                "timeZone": "UTC"
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
  "description": "bookingBusiness: getCalendarView",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-list-calendarview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
