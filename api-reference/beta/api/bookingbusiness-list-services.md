---
title: Listar serviços
description: Obter uma lista de objetos bookingService no bookingbusiness especificado.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: cfef3c9e942591822760d103aac46a86e6cccfbb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047893"
---
# <a name="list-services"></a><span data-ttu-id="4241f-103">Listar serviços</span><span class="sxs-lookup"><span data-stu-id="4241f-103">List services</span></span>

<span data-ttu-id="4241f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4241f-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4241f-105">Obter uma lista de [objetos bookingService](../resources/bookingservice.md) no [bookingbusiness especificado.](../resources/bookingbusiness.md)</span><span class="sxs-lookup"><span data-stu-id="4241f-105">Get a list of [bookingService](../resources/bookingservice.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="4241f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="4241f-106">Permissions</span></span>
<span data-ttu-id="4241f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4241f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4241f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4241f-109">Permission type</span></span>      | <span data-ttu-id="4241f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4241f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4241f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4241f-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="4241f-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="4241f-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="4241f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4241f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4241f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4241f-114">Not supported.</span></span>   |
|<span data-ttu-id="4241f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4241f-115">Application</span></span> | <span data-ttu-id="4241f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4241f-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="4241f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4241f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4241f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4241f-118">Optional query parameters</span></span>
<span data-ttu-id="4241f-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4241f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4241f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4241f-120">Request headers</span></span>
| <span data-ttu-id="4241f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="4241f-121">Name</span></span>      |<span data-ttu-id="4241f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4241f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4241f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4241f-123">Authorization</span></span>  | <span data-ttu-id="4241f-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="4241f-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="4241f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4241f-125">Request body</span></span>
<span data-ttu-id="4241f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4241f-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="4241f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="4241f-127">Response</span></span>
<span data-ttu-id="4241f-128">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção de objetos [bookingService](../resources/bookingservice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4241f-128">If successful, this method returns a `200 OK` response code and collection of [bookingService](../resources/bookingservice.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4241f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4241f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4241f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4241f-130">Request</span></span>
<span data-ttu-id="4241f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="4241f-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4241f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="4241f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_services_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services
```
# <a name="c"></a>[<span data-ttu-id="4241f-133">C#</span><span class="sxs-lookup"><span data-stu-id="4241f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-services-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4241f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4241f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-services-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4241f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4241f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-services-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4241f-136">Java</span><span class="sxs-lookup"><span data-stu-id="4241f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-services-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4241f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="4241f-137">Response</span></span>
<span data-ttu-id="4241f-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="4241f-138">The following is an example of the response.</span></span> <span data-ttu-id="4241f-139">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4241f-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingService",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/services",
    "value": [
        {
            "id": "f9b9121f-aed7-4c8c-bb3a-a1796a0b0b2d",
            "displayName": "Initial service",
            "defaultDuration": "PT10M",
            "defaultPrice": 0,
            "defaultPriceType": "notSet",
            "description": "Not sure how to choose? Let us introduce you to our traditional family recipes.",
            "isHiddenFromCustomers": false,
            "notes": "This is where you can add notes about this service that only you and your staff see.",
            "preBuffer": "PT0S",
            "postBuffer": "PT0S",
            "staffMemberIds": [],
            "schedulingPolicy": null,
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
            "defaultReminders": []
        },
        {
            "id": "57da6774-a087-4d69-b0e6-6fb82c339976",
            "displayName": "Catered bento",
            "defaultDuration": "PT30M",
            "defaultPrice": 10,
            "defaultPriceType": "fixedPrice",
            "description": "Catered individual bento box lunch",
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
            "defaultReminders": [],
            "schedulingPolicy": {
                "timeSlotInterval": "PT1H",
                "minimumLeadTime": "PT10H",
                "maximumAdvance": "P10D",
                "sendConfirmationsToOwner": true,
                "allowStaffSelection": true
            }
        },
        {
            "id": "635a7b7c-4230-4d3b-a42b-698e89927528",
            "displayName": "Kaiseki",
            "defaultDuration": "PT1H30M",
            "defaultPrice": 30,
            "defaultPriceType": "fixedPrice",
            "description": "Individual kaiseki lunch delivery",
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
            "defaultReminders": [],
            "schedulingPolicy": {
                "timeSlotInterval": "PT1H",
                "minimumLeadTime": "PT10H",
                "maximumAdvance": "P10D",
                "sendConfirmationsToOwner": true,
                "allowStaffSelection": true
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
  "description": "List services",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
