---
title: Obter bookingAppointment
description: Obtenha as propriedades e os relacionamentos de um objeto bookingAppointment no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 3f21d9b57f0ef692db80e42f40a152d3bdc29bfa
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33636517"
---
# <a name="get-bookingappointment"></a><span data-ttu-id="638cf-103">Obter bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="638cf-103">Get bookingAppointment</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="638cf-104">Obtenha as propriedades e os relacionamentos de um objeto [bookingAppointment](../resources/bookingappointment.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="638cf-104">Get the properties and relationships of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="638cf-105">As propriedades **Start** e **end** sempre são retornadas em UTC.</span><span class="sxs-lookup"><span data-stu-id="638cf-105">The **start** and **end** properties are always returned in UTC.</span></span>
## <a name="permissions"></a><span data-ttu-id="638cf-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="638cf-106">Permissions</span></span>
<span data-ttu-id="638cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="638cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="638cf-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="638cf-109">Permission type</span></span>      | <span data-ttu-id="638cf-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="638cf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="638cf-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="638cf-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="638cf-112">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="638cf-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="638cf-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="638cf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="638cf-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="638cf-114">Not supported.</span></span>   |
|<span data-ttu-id="638cf-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="638cf-115">Application</span></span> | <span data-ttu-id="638cf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="638cf-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="638cf-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="638cf-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="638cf-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="638cf-118">Optional query parameters</span></span>
<span data-ttu-id="638cf-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="638cf-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="638cf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="638cf-120">Request headers</span></span>
| <span data-ttu-id="638cf-121">Nome</span><span class="sxs-lookup"><span data-stu-id="638cf-121">Name</span></span>      |<span data-ttu-id="638cf-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="638cf-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="638cf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="638cf-123">Authorization</span></span>  | <span data-ttu-id="638cf-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="638cf-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="638cf-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="638cf-125">Request body</span></span>
<span data-ttu-id="638cf-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="638cf-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="638cf-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="638cf-127">Response</span></span>
<span data-ttu-id="638cf-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [bookingAppointment](../resources/bookingappointment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="638cf-128">If successful, this method returns a `200 OK` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="638cf-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="638cf-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="638cf-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="638cf-130">Request</span></span>
<span data-ttu-id="638cf-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="638cf-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingappointment"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
```
##### <a name="response"></a><span data-ttu-id="638cf-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="638cf-132">Response</span></span>
<span data-ttu-id="638cf-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="638cf-133">The following is an example of the response.</span></span> <span data-ttu-id="638cf-134">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="638cf-134">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="638cf-135">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="638cf-135">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/appointments/$entity",
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
        "dateTime": "2018-05-06T12:30:00.0000000Z",
        "timeZone": "UTC"
    }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="638cf-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="638cf-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="638cf-137">Basic</span><span class="sxs-lookup"><span data-stu-id="638cf-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_bookingappointment-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="638cf-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="638cf-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_bookingappointment-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingappointment-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingappointment-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
