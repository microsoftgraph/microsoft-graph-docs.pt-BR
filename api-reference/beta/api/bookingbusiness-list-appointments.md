---
title: Listar compromissos
description: Obter uma lista de objetos bookingAppointment para o bookingbusiness especificado.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: b2543c08dd94109174d9945afec5b6687159db7e
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047914"
---
# <a name="list-appointments"></a><span data-ttu-id="d9c1c-103">Listar compromissos</span><span class="sxs-lookup"><span data-stu-id="d9c1c-103">List appointments</span></span>

<span data-ttu-id="d9c1c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9c1c-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9c1c-105">Obter uma lista de [objetos bookingAppointment](../resources/bookingappointment.md) para o [bookingbusiness especificado.](../resources/bookingbusiness.md)</span><span class="sxs-lookup"><span data-stu-id="d9c1c-105">Get a list of [bookingAppointment](../resources/bookingappointment.md) objects for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="d9c1c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9c1c-106">Permissions</span></span>
<span data-ttu-id="d9c1c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9c1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9c1c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9c1c-109">Permission type</span></span>      | <span data-ttu-id="d9c1c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9c1c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d9c1c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9c1c-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="d9c1c-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="d9c1c-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d9c1c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9c1c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9c1c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9c1c-114">Not supported.</span></span>   |
|<span data-ttu-id="d9c1c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9c1c-115">Application</span></span> | <span data-ttu-id="d9c1c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9c1c-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d9c1c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9c1c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d9c1c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d9c1c-118">Optional query parameters</span></span>
<span data-ttu-id="d9c1c-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d9c1c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="d9c1c-120">Para obter o conjunto de compromissos de uma empresa do Bookings dentro de um intervalo de datas, em vez `$filter` de , obter o [calendarView](bookingbusiness-list-calendarview.md) para esse intervalo de datas.</span><span class="sxs-lookup"><span data-stu-id="d9c1c-120">To get the set of appointments of a Bookings business within a date range, instead of `$filter`, [get the calendarView](bookingbusiness-list-calendarview.md) for that date range.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9c1c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9c1c-121">Request headers</span></span>
| <span data-ttu-id="d9c1c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d9c1c-122">Name</span></span>      |<span data-ttu-id="d9c1c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9c1c-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d9c1c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9c1c-124">Authorization</span></span>  | <span data-ttu-id="d9c1c-125">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d9c1c-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9c1c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9c1c-126">Request body</span></span>
<span data-ttu-id="d9c1c-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9c1c-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d9c1c-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9c1c-128">Response</span></span>
<span data-ttu-id="d9c1c-129">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [bookingAppointment](../resources/bookingappointment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9c1c-129">If successful, this method returns a `200 OK` response code and collection of [bookingAppointment](../resources/bookingappointment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d9c1c-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9c1c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d9c1c-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9c1c-131">Request</span></span>
<span data-ttu-id="d9c1c-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9c1c-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d9c1c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d9c1c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appointments"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments
```
# <a name="c"></a>[<span data-ttu-id="d9c1c-134">C#</span><span class="sxs-lookup"><span data-stu-id="d9c1c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appointments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d9c1c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d9c1c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appointments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d9c1c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d9c1c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appointments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d9c1c-137">Java</span><span class="sxs-lookup"><span data-stu-id="d9c1c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-appointments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d9c1c-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9c1c-138">Response</span></span>
<span data-ttu-id="d9c1c-139">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d9c1c-139">The following is an example of the response.</span></span> <span data-ttu-id="d9c1c-140">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d9c1c-140">Note: The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/appointments",
    "value": [
        {
            "id": "AAMkADKoAAA=",
            "selfServiceAppointmentId": "00000000-0000-0000-0000-000000000000",
            "customerId": "829e3cb5-3d4d-4319-a8de-1953aedaa166",
            "customerName": "Bob Kelly",
            "customerEmailAddress": "bobk@tailspintoys.com",
            "customerPhone": "213-555-0108",
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
            "invoiceId": "1002",
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
                "dateTime": "2018-04-30T13:00:00.0000000Z",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2018-04-30T13:30:00.0000000Z",
                "timeZone": "UTC"
            },
            "serviceLocation": {
                "displayName": "Customer location (987 Third Avenue, Buffalo, NY 98052, USA)",
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
                "dateTime": "2018-04-30T13:30:00.0000000Z",
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
            "reminders": [],
            "invoiceDate": {
                "dateTime": "2018-05-01T12:30:00.0000000Z",
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
  "description": "List appointments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
