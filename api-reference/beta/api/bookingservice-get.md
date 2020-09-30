---
title: Obter bookingService
description: Obtenha as propriedades e os relacionamentos de um objeto bookingService no bookingbusiness especificado.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 8218365646f7ba4d7401362bf1b5365a47218821
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313212"
---
# <a name="get-bookingservice"></a><span data-ttu-id="8069c-103">Obter bookingService</span><span class="sxs-lookup"><span data-stu-id="8069c-103">Get bookingService</span></span>

<span data-ttu-id="8069c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8069c-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8069c-105">Obtenha as propriedades e os relacionamentos de um objeto [bookingService](../resources/bookingservice.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="8069c-105">Get the properties and relationships of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="8069c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="8069c-106">Permissions</span></span>
<span data-ttu-id="8069c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8069c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8069c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8069c-109">Permission type</span></span>      | <span data-ttu-id="8069c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8069c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8069c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8069c-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="8069c-112">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="8069c-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="8069c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8069c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8069c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8069c-114">Not supported.</span></span>   |
|<span data-ttu-id="8069c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8069c-115">Application</span></span> | <span data-ttu-id="8069c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8069c-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="8069c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8069c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8069c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8069c-118">Optional query parameters</span></span>
<span data-ttu-id="8069c-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8069c-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8069c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8069c-120">Request headers</span></span>
| <span data-ttu-id="8069c-121">Nome</span><span class="sxs-lookup"><span data-stu-id="8069c-121">Name</span></span>      |<span data-ttu-id="8069c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="8069c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8069c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8069c-123">Authorization</span></span>  | <span data-ttu-id="8069c-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="8069c-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="8069c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8069c-125">Request body</span></span>
<span data-ttu-id="8069c-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8069c-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="8069c-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="8069c-127">Response</span></span>
<span data-ttu-id="8069c-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [bookingService](../resources/bookingservice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8069c-128">If successful, this method returns a `200 OK` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8069c-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8069c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8069c-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8069c-130">Request</span></span>
<span data-ttu-id="8069c-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="8069c-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8069c-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8069c-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingservice"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
# <a name="c"></a>[<span data-ttu-id="8069c-133">C#</span><span class="sxs-lookup"><span data-stu-id="8069c-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingservice-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8069c-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8069c-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingservice-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8069c-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8069c-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingservice-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8069c-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="8069c-136">Response</span></span>
<span data-ttu-id="8069c-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="8069c-137">The following is an example of the response.</span></span> <span data-ttu-id="8069c-138">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="8069c-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="8069c-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8069c-139">All of the properties will be returned from an actual call.</span></span>
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