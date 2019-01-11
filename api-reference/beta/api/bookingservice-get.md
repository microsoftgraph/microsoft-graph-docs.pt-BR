---
title: Obter bookingService
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 7a309e076f480d051a1da47265dedaf4c32207d9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819688"
---
# <a name="get-bookingservice"></a><span data-ttu-id="28694-104">Obter bookingService</span><span class="sxs-lookup"><span data-stu-id="28694-104">Get bookingService</span></span>

 > <span data-ttu-id="28694-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="28694-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28694-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="28694-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="28694-107">Obtenha as propriedades e relacionamentos de um objeto [bookingService](../resources/bookingservice.md) no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="28694-107">Get the properties and relationships of a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="28694-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="28694-108">Permissions</span></span>
<span data-ttu-id="28694-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28694-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28694-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28694-111">Permission type</span></span>      | <span data-ttu-id="28694-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="28694-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28694-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28694-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="28694-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="28694-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="28694-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28694-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28694-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28694-116">Not supported.</span></span>   |
|<span data-ttu-id="28694-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28694-117">Application</span></span> | <span data-ttu-id="28694-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28694-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="28694-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28694-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/services/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="28694-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="28694-120">Optional query parameters</span></span>
<span data-ttu-id="28694-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="28694-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="28694-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28694-122">Request headers</span></span>
| <span data-ttu-id="28694-123">Nome</span><span class="sxs-lookup"><span data-stu-id="28694-123">Name</span></span>      |<span data-ttu-id="28694-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="28694-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="28694-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="28694-125">Authorization</span></span>  | <span data-ttu-id="28694-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="28694-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="28694-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28694-127">Request body</span></span>
<span data-ttu-id="28694-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28694-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="28694-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="28694-129">Response</span></span>
<span data-ttu-id="28694-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [bookingService](../resources/bookingservice.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28694-130">If successful, this method returns a `200 OK` response code and [bookingService](../resources/bookingservice.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="28694-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28694-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="28694-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28694-132">Request</span></span>
<span data-ttu-id="28694-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="28694-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingservice"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
##### <a name="response"></a><span data-ttu-id="28694-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="28694-134">Response</span></span>
<span data-ttu-id="28694-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="28694-135">The following is an example of the response.</span></span> <span data-ttu-id="28694-136">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="28694-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="28694-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28694-137">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
