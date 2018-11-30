---
title: Lista de compromissos
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: 5e0846a1671a7a566e5175a331dc7c03e02af537
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034676"
---
# <a name="list-appointments"></a><span data-ttu-id="969c0-104">Lista de compromissos</span><span class="sxs-lookup"><span data-stu-id="969c0-104">List appointments</span></span>

 > <span data-ttu-id="969c0-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="969c0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="969c0-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="969c0-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="969c0-107">Obtenha uma lista de objetos [bookingAppointment](../resources/bookingappointment.md) para o especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="969c0-107">Get a list of [bookingAppointment](../resources/bookingappointment.md) objects for the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="969c0-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="969c0-108">Permissions</span></span>
<span data-ttu-id="969c0-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="969c0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="969c0-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="969c0-111">Permission type</span></span>      | <span data-ttu-id="969c0-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="969c0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="969c0-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="969c0-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="969c0-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="969c0-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="969c0-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="969c0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="969c0-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="969c0-116">Not supported.</span></span>   |
|<span data-ttu-id="969c0-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="969c0-117">Application</span></span> | <span data-ttu-id="969c0-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="969c0-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="969c0-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="969c0-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/appointments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="969c0-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="969c0-120">Optional query parameters</span></span>
<span data-ttu-id="969c0-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="969c0-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="969c0-122">Para obter o conjunto de compromissos de uma empresa reservas dentro de um intervalo de datas, em vez de `$filter`, [Obtenha o calendarView](bookingbusiness-list-calendarview.md) para aquele intervalo de data.</span><span class="sxs-lookup"><span data-stu-id="969c0-122">To get the set of appointments of a Bookings business within a date range, instead of `$filter`, [get the calendarView](bookingbusiness-list-calendarview.md) for that date range.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="969c0-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="969c0-123">Request headers</span></span>
| <span data-ttu-id="969c0-124">Nome</span><span class="sxs-lookup"><span data-stu-id="969c0-124">Name</span></span>      |<span data-ttu-id="969c0-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="969c0-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="969c0-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="969c0-126">Authorization</span></span>  | <span data-ttu-id="969c0-127">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="969c0-127">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="969c0-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="969c0-128">Request body</span></span>
<span data-ttu-id="969c0-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="969c0-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="969c0-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="969c0-130">Response</span></span>
<span data-ttu-id="969c0-131">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [bookingAppointment](../resources/bookingappointment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="969c0-131">If successful, this method returns a `200 OK` response code and collection of [bookingAppointment](../resources/bookingappointment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="969c0-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="969c0-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="969c0-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="969c0-133">Request</span></span>
<span data-ttu-id="969c0-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="969c0-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appointments"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/appointments
```
##### <a name="response"></a><span data-ttu-id="969c0-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="969c0-135">Response</span></span>
<span data-ttu-id="969c0-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="969c0-136">The following is an example of the response.</span></span> <span data-ttu-id="969c0-137">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="969c0-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="969c0-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="969c0-138">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List appointments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->