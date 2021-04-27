---
title: Obter bookingService
description: Obter as propriedades e as relações de um objeto bookingService no bookingbusiness especificado.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 75b3c4db0bc37dc71acefbf3d551221eac821303
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047802"
---
# <a name="get-bookingservice"></a><span data-ttu-id="5aca2-103">Obter bookingService</span><span class="sxs-lookup"><span data-stu-id="5aca2-103">Get bookingService</span></span>

<span data-ttu-id="5aca2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5aca2-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5aca2-105">Obter as propriedades e as relações de um [objeto bookingService](../resources/bookingservice.md) no [bookingbusiness especificado.](../resources/bookingbusiness.md)</span><span class="sxs-lookup"><span data-stu-id="5aca2-105">Get the properties and relationships of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="5aca2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5aca2-106">Permissions</span></span>
<span data-ttu-id="5aca2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5aca2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5aca2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5aca2-109">Permission type</span></span>      | <span data-ttu-id="5aca2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5aca2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5aca2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5aca2-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="5aca2-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="5aca2-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="5aca2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5aca2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5aca2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5aca2-114">Not supported.</span></span>   |
|<span data-ttu-id="5aca2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5aca2-115">Application</span></span> | <span data-ttu-id="5aca2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5aca2-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="5aca2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5aca2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="5aca2-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5aca2-118">Optional query parameters</span></span>
<span data-ttu-id="5aca2-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="5aca2-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5aca2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5aca2-120">Request headers</span></span>
| <span data-ttu-id="5aca2-121">Nome</span><span class="sxs-lookup"><span data-stu-id="5aca2-121">Name</span></span>      |<span data-ttu-id="5aca2-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="5aca2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5aca2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5aca2-123">Authorization</span></span>  | <span data-ttu-id="5aca2-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="5aca2-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="5aca2-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5aca2-125">Request body</span></span>
<span data-ttu-id="5aca2-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5aca2-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5aca2-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="5aca2-127">Response</span></span>
<span data-ttu-id="5aca2-128">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto bookingService](../resources/bookingservice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5aca2-128">If successful, this method returns a `200 OK` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5aca2-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5aca2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5aca2-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5aca2-130">Request</span></span>
<span data-ttu-id="5aca2-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="5aca2-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5aca2-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5aca2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingservice"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
# <a name="c"></a>[<span data-ttu-id="5aca2-133">C#</span><span class="sxs-lookup"><span data-stu-id="5aca2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5aca2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5aca2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5aca2-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5aca2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5aca2-136">Java</span><span class="sxs-lookup"><span data-stu-id="5aca2-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-bookingservice-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5aca2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="5aca2-137">Response</span></span>
<span data-ttu-id="5aca2-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="5aca2-138">The following is an example of the response.</span></span> <span data-ttu-id="5aca2-139">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5aca2-139">Note: The response object shown here might be shortened for readability.</span></span>
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
  "suppressions": [
  ]
}
-->
