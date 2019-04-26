---
title: Obter bookingService
description: Obtenha as propriedades e os relacionamentos de um objeto bookingService no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 450b98dcd4e454fd4f51b45c7fc2f2a82ba2745d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322299"
---
# <a name="get-bookingservice"></a><span data-ttu-id="d7a64-103">Obter bookingService</span><span class="sxs-lookup"><span data-stu-id="d7a64-103">Get bookingService</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7a64-104">Obtenha as propriedades e os relacionamentos de um objeto [bookingService](../resources/bookingservice.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="d7a64-104">Get the properties and relationships of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="d7a64-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d7a64-105">Permissions</span></span>
<span data-ttu-id="d7a64-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7a64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7a64-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d7a64-108">Permission type</span></span>      | <span data-ttu-id="d7a64-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d7a64-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7a64-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d7a64-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="d7a64-111">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="d7a64-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="d7a64-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d7a64-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7a64-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7a64-113">Not supported.</span></span>   |
|<span data-ttu-id="d7a64-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d7a64-114">Application</span></span> | <span data-ttu-id="d7a64-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d7a64-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="d7a64-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d7a64-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d7a64-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d7a64-117">Optional query parameters</span></span>
<span data-ttu-id="d7a64-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d7a64-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7a64-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d7a64-119">Request headers</span></span>
| <span data-ttu-id="d7a64-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d7a64-120">Name</span></span>      |<span data-ttu-id="d7a64-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7a64-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d7a64-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7a64-122">Authorization</span></span>  | <span data-ttu-id="d7a64-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="d7a64-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7a64-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d7a64-124">Request body</span></span>
<span data-ttu-id="d7a64-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d7a64-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="d7a64-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7a64-126">Response</span></span>
<span data-ttu-id="d7a64-127">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [bookingService](../resources/bookingservice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d7a64-127">If successful, this method returns a `200 OK` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d7a64-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7a64-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7a64-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d7a64-129">Request</span></span>
<span data-ttu-id="d7a64-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7a64-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingservice"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
##### <a name="response"></a><span data-ttu-id="d7a64-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d7a64-131">Response</span></span>
<span data-ttu-id="d7a64-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="d7a64-132">The following is an example of the response.</span></span> <span data-ttu-id="d7a64-133">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="d7a64-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d7a64-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d7a64-134">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingService"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/services/$entity",
    "id": "57da6774-a087-4d69-b0e6-6fb82c339976",
    "displayName": "Bento",
    "defaultDuration": "PT30M",
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
  "description": "Get bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
