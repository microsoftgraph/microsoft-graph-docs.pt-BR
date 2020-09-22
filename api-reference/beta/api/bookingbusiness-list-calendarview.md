---
title: Listar o calendarView do Bookings
description: Obter a coleção de objetos bookingAppointment para um bookingBusiness, que ocorre no intervalo de datas especificado.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 8a6a0e70937dbf24d59adcc922944f211e570448
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988062"
---
# <a name="list-bookings-calendarview"></a><span data-ttu-id="9e69e-103">Listar o calendarView do Bookings</span><span class="sxs-lookup"><span data-stu-id="9e69e-103">List Bookings calendarView</span></span>

<span data-ttu-id="9e69e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e69e-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e69e-105">Obter a coleção de objetos [bookingAppointment](../resources/bookingappointment.md) para um [bookingBusiness](../resources/bookingbusiness.md), que ocorre no intervalo de datas especificado.</span><span class="sxs-lookup"><span data-stu-id="9e69e-105">Get the collection of [bookingAppointment](../resources/bookingappointment.md) objects for a [bookingBusiness](../resources/bookingbusiness.md), that occurs in the specified date range.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e69e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9e69e-106">Permissions</span></span>
<span data-ttu-id="9e69e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e69e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e69e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9e69e-109">Permission type</span></span>      | <span data-ttu-id="9e69e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9e69e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e69e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9e69e-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="9e69e-112">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="9e69e-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="9e69e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9e69e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e69e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e69e-114">Not supported.</span></span>   |
|<span data-ttu-id="9e69e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9e69e-115">Application</span></span> | <span data-ttu-id="9e69e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9e69e-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9e69e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9e69e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/calendarView?start={start-value}&end={end-value}
```

## <a name="query-parameters"></a><span data-ttu-id="9e69e-118">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="9e69e-118">Query parameters</span></span>

<span data-ttu-id="9e69e-119">Forneça os seguintes parâmetros de consulta necessários com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="9e69e-119">In the request URL, provide the following required query parameters with values.</span></span>

| <span data-ttu-id="9e69e-120">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="9e69e-120">Parameter</span></span>    | <span data-ttu-id="9e69e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="9e69e-121">Type</span></span>   |<span data-ttu-id="9e69e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e69e-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e69e-123">iniciar</span><span class="sxs-lookup"><span data-stu-id="9e69e-123">start</span></span>|<span data-ttu-id="9e69e-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e69e-124">DateTimeOffset</span></span>|<span data-ttu-id="9e69e-125">A data e a hora de início de um intervalo de tempo, representadas no formato ISO 8601, como UTC ou offset do UTC.</span><span class="sxs-lookup"><span data-stu-id="9e69e-125">The start date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="9e69e-126">Por exemplo, meia-noite UTC em 1º de janeiro de 2018 teria a seguinte aparência: ' 2018-01-01T00:00:00Z ' e o mesmo tempo em PST teria a seguinte aparência: ' 2017-12-31T16:00:00-08:00 '.</span><span class="sxs-lookup"><span data-stu-id="9e69e-126">For example, midnight UTC on Jan 1, 2018 would look like this: '2018-01-01T00:00:00Z', and the same time in PST would look like this: '2017-12-31T16:00:00-08:00'.</span></span>|
|<span data-ttu-id="9e69e-127">end</span><span class="sxs-lookup"><span data-stu-id="9e69e-127">end</span></span>|<span data-ttu-id="9e69e-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e69e-128">DateTimeOffset</span></span>|<span data-ttu-id="9e69e-129">A data e a hora de término de um intervalo de tempo, representadas no formato ISO 8601, como UTC ou offset do UTC.</span><span class="sxs-lookup"><span data-stu-id="9e69e-129">The end date and time of a time range, represented in ISO 8601 format, as UTC or an offset from UTC.</span></span> <span data-ttu-id="9e69e-130">Por exemplo, 3am UTC em 1º de janeiro de 2018 teria a seguinte aparência: ' 2018-01-01T03:00: o 00Z ' e o mesmo momento em PST teria a seguinte aparência: ' 2017-12-31T19:00:00-08:00 '.</span><span class="sxs-lookup"><span data-stu-id="9e69e-130">For example, 3am UTC on Jan 1, 2018 would look like this: '2018-01-01T03:00:00Z', and the same time in PST would look like this: '2017-12-31T19:00:00-08:00'.</span></span>|

<span data-ttu-id="9e69e-131">Os valores de `start` e `end` são interpretados usando o deslocamento de fuso horário especificado em seus valores correspondentes e não são afetados pelo valor do `Prefer: outlook.timezone` cabeçalho, se houver.</span><span class="sxs-lookup"><span data-stu-id="9e69e-131">The values of `start` and `end` are interpreted using the timezone offset specified in their corresponding values and are not impacted by the value of the `Prefer: outlook.timezone` header if present.</span></span>

<span data-ttu-id="9e69e-132">Este método também dá suporte a alguns [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9e69e-132">This method also supports some of the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e69e-133">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9e69e-133">Request headers</span></span>
| <span data-ttu-id="9e69e-134">Nome</span><span class="sxs-lookup"><span data-stu-id="9e69e-134">Name</span></span>       | <span data-ttu-id="9e69e-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e69e-135">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9e69e-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e69e-136">Authorization</span></span>  | <span data-ttu-id="9e69e-137">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9e69e-137">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e69e-138">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9e69e-138">Request body</span></span>
<span data-ttu-id="9e69e-139">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9e69e-139">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e69e-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e69e-140">Response</span></span>
<span data-ttu-id="9e69e-141">Se bem-sucedido, este método retorna `200, OK` o código de resposta e o objeto da coleção [bookingAppointment](../resources/bookingappointment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9e69e-141">If successful, this method returns `200, OK` response code and [bookingAppointment](../resources/bookingappointment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e69e-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9e69e-142">Example</span></span>
<span data-ttu-id="9e69e-143">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="9e69e-143">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9e69e-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9e69e-144">Request</span></span>
<span data-ttu-id="9e69e-145">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9e69e-145">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9e69e-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e69e-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_getcalendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/calendarView?start=2018-04-30T00:00:00Z&end=2018-05-10T00:00:00Z
```
# <a name="c"></a>[<span data-ttu-id="9e69e-147">C#</span><span class="sxs-lookup"><span data-stu-id="9e69e-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/bookingbusiness-getcalendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e69e-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e69e-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/bookingbusiness-getcalendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e69e-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e69e-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/bookingbusiness-getcalendarview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9e69e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="9e69e-150">Response</span></span>
<span data-ttu-id="9e69e-151">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9e69e-151">The following is an example of the response.</span></span> <span data-ttu-id="9e69e-152">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="9e69e-152">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9e69e-153">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9e69e-153">All of the properties will be returned from an actual call.</span></span>
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


