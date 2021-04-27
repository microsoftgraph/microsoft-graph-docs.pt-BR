---
title: Listar o calendarView do Bookings
description: Obter a coleção de objetos bookingAppointment para um bookingBusiness, que ocorre no intervalo de datas especificado.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: d96e5b2f2c7f435a0ea8dcd39a4b58ae7657c222
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047907"
---
# <a name="list-bookings-calendarview"></a><span data-ttu-id="e2522-103">Listar o calendarView do Bookings</span><span class="sxs-lookup"><span data-stu-id="e2522-103">List Bookings calendarView</span></span>

<span data-ttu-id="e2522-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2522-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2522-105">Obter a coleção [de objetos bookingAppointment](../resources/bookingappointment.md) para [um bookingBusiness](../resources/bookingbusiness.md), que ocorre no intervalo de datas especificado.</span><span class="sxs-lookup"><span data-stu-id="e2522-105">Get the collection of [bookingAppointment](../resources/bookingappointment.md) objects for a [bookingBusiness](../resources/bookingbusiness.md), that occurs in the specified date range.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2522-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e2522-106">Permissions</span></span>
<span data-ttu-id="e2522-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2522-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2522-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2522-109">Permission type</span></span>      | <span data-ttu-id="e2522-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e2522-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e2522-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2522-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="e2522-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="e2522-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="e2522-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2522-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2522-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2522-114">Not supported.</span></span>   |
|<span data-ttu-id="e2522-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e2522-115">Application</span></span> | <span data-ttu-id="e2522-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2522-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="e2522-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2522-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/calendarView?start={start-value}&end={end-value}
```

## <a name="query-parameters"></a><span data-ttu-id="e2522-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="e2522-118">Query parameters</span></span>

<span data-ttu-id="e2522-119">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="e2522-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="e2522-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="e2522-120">Parameter</span></span>    | <span data-ttu-id="e2522-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2522-121">Type</span></span>   |<span data-ttu-id="e2522-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2522-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e2522-123">iniciar</span><span class="sxs-lookup"><span data-stu-id="e2522-123">start</span></span>|<span data-ttu-id="e2522-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2522-124">DateTimeOffset</span></span>|<span data-ttu-id="e2522-125">A data e a hora de início de um intervalo de tempo, representados no formato ISO 8601, como UTC ou um deslocamento do UTC.</span><span class="sxs-lookup"><span data-stu-id="e2522-125">The start date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="e2522-126">Por exemplo, meia-noite UTC em 1º de janeiro de 2018 teria esta aparência: '2018-01-01T00:00:00Z', e o mesmo horário no PST teria esta aparência: '2017-12-31T16:00:00-08:00'.</span><span class="sxs-lookup"><span data-stu-id="e2522-126">For example, midnight UTC on Jan 1, 2018 would look like this: '2018-01-01T00:00:00Z', and the same time in PST would look like this: '2017-12-31T16:00:00-08:00'.</span></span>|
|<span data-ttu-id="e2522-127">end</span><span class="sxs-lookup"><span data-stu-id="e2522-127">end</span></span>|<span data-ttu-id="e2522-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e2522-128">DateTimeOffset</span></span>|<span data-ttu-id="e2522-129">A data e a hora de término de um intervalo de tempo, representado no formato ISO 8601, como UTC ou um deslocamento do UTC.</span><span class="sxs-lookup"><span data-stu-id="e2522-129">The end date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="e2522-130">Por exemplo, 3am UTC em 1º de janeiro de 2018 teria esta aparência: '2018-01-01T03:00:00Z', e o mesmo horário no PST teria esta aparência: '2017-12-31T19:00:00-08:00'.</span><span class="sxs-lookup"><span data-stu-id="e2522-130">For example, 3am UTC on Jan 1, 2018 would look like this: '2018-01-01T03:00:00Z', and the same time in PST would look like this: '2017-12-31T19:00:00-08:00'.</span></span>|

<span data-ttu-id="e2522-131">Os valores de e são interpretados usando o deslocamento de zona de tempo especificado em seus valores correspondentes e não são afetados pelo valor do `start` `end` `Prefer: outlook.timezone` header, se presente.</span><span class="sxs-lookup"><span data-stu-id="e2522-131">The values of `start` and `end` are interpreted using the timezone offset specified in their corresponding values and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span>

<span data-ttu-id="e2522-132">Este método também dá suporte a alguns [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e2522-132">This method also supports some of the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e2522-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2522-133">Request headers</span></span>
| <span data-ttu-id="e2522-134">Nome</span><span class="sxs-lookup"><span data-stu-id="e2522-134">Name</span></span>       | <span data-ttu-id="e2522-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2522-135">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e2522-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2522-136">Authorization</span></span>  | <span data-ttu-id="e2522-137">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="e2522-137">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2522-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2522-138">Request body</span></span>
<span data-ttu-id="e2522-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e2522-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2522-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2522-140">Response</span></span>
<span data-ttu-id="e2522-141">Se tiver êxito, este método retornará o código de resposta e o objeto da coleção `200, OK` [bookingAppointment](../resources/bookingappointment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2522-141">If successful, this method returns `200, OK` response code and [bookingAppointment](../resources/bookingappointment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2522-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2522-142">Example</span></span>
<span data-ttu-id="e2522-143">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="e2522-143">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e2522-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2522-144">Request</span></span>
<span data-ttu-id="e2522-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2522-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e2522-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2522-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getcalendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/calendarView?start=2018-04-30T00:00:00Z&end=2018-05-10T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="e2522-147">C#</span><span class="sxs-lookup"><span data-stu-id="e2522-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-getcalendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2522-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2522-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-getcalendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2522-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2522-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-getcalendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2522-150">Java</span><span class="sxs-lookup"><span data-stu-id="e2522-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/bookingbusiness-getcalendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e2522-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2522-151">Response</span></span>
<span data-ttu-id="e2522-152">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e2522-152">The following is an example of the response.</span></span> <span data-ttu-id="e2522-153">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e2522-153">Note: The response object shown here might be shortened for readability.</span></span>
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
  ]
}
-->
