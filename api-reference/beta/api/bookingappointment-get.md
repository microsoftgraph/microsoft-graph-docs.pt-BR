---
title: Obter bookingAppointment
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 7b9b04a8104bfe6f4569a31d0e88616af4e97fdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850796"
---
# <a name="get-bookingappointment"></a><span data-ttu-id="32c32-104">Obter bookingAppointment</span><span class="sxs-lookup"><span data-stu-id="32c32-104">Get bookingAppointment</span></span>

 > <span data-ttu-id="32c32-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="32c32-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32c32-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="32c32-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="32c32-107">Obtenha as propriedades e relacionamentos de um objeto [bookingAppointment](../resources/bookingappointment.md) no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="32c32-107">Get the properties and relationships of a [bookingAppointment](../resources/bookingappointment.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>

<span data-ttu-id="32c32-108">As propriedades **start** e **end** sempre são retornadas em UTC.</span><span class="sxs-lookup"><span data-stu-id="32c32-108">The **start** and **end** properties are always returned in UTC.</span></span>
## <a name="permissions"></a><span data-ttu-id="32c32-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="32c32-109">Permissions</span></span>
<span data-ttu-id="32c32-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32c32-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32c32-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="32c32-112">Permission type</span></span>      | <span data-ttu-id="32c32-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="32c32-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32c32-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="32c32-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="32c32-115">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="32c32-115">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="32c32-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="32c32-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32c32-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32c32-117">Not supported.</span></span>   |
|<span data-ttu-id="32c32-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="32c32-118">Application</span></span> | <span data-ttu-id="32c32-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="32c32-119">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="32c32-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="32c32-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="32c32-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="32c32-121">Optional query parameters</span></span>
<span data-ttu-id="32c32-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="32c32-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="32c32-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="32c32-123">Request headers</span></span>
| <span data-ttu-id="32c32-124">Nome</span><span class="sxs-lookup"><span data-stu-id="32c32-124">Name</span></span>      |<span data-ttu-id="32c32-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="32c32-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="32c32-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="32c32-126">Authorization</span></span>  | <span data-ttu-id="32c32-127">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="32c32-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="32c32-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="32c32-128">Request body</span></span>
<span data-ttu-id="32c32-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="32c32-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="32c32-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="32c32-130">Response</span></span>
<span data-ttu-id="32c32-131">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [bookingAppointment](../resources/bookingappointment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="32c32-131">If successful, this method returns a `200 OK` response code and [bookingAppointment](../resources/bookingappointment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="32c32-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="32c32-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="32c32-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="32c32-133">Request</span></span>
<span data-ttu-id="32c32-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="32c32-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingappointment"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments/AAMkADKnAAA=
```
##### <a name="response"></a><span data-ttu-id="32c32-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="32c32-135">Response</span></span>
<span data-ttu-id="32c32-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="32c32-136">The following is an example of the response.</span></span> <span data-ttu-id="32c32-137">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="32c32-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="32c32-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="32c32-138">All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingAppointment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
