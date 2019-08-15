---
title: Obter bookingBusiness
description: Obtenha as propriedades e os relacionamentos de um objeto bookingBusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: ebf41f24bee2016b51f4d9403988014c9e00683b
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415621"
---
# <a name="get-bookingbusiness"></a><span data-ttu-id="68436-103">Obter bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="68436-103">Get bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68436-104">Obtenha as propriedades e os relacionamentos de um objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="68436-104">Get the properties and relationships of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="68436-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="68436-105">Permissions</span></span>
<span data-ttu-id="68436-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68436-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68436-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68436-108">Permission type</span></span>      | <span data-ttu-id="68436-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="68436-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68436-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68436-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="68436-111">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="68436-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="68436-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68436-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68436-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68436-113">Not supported.</span></span>   |
|<span data-ttu-id="68436-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68436-114">Application</span></span> | <span data-ttu-id="68436-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="68436-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="68436-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68436-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="68436-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="68436-117">Optional query parameters</span></span>
<span data-ttu-id="68436-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="68436-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="68436-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68436-119">Request headers</span></span>
| <span data-ttu-id="68436-120">Nome</span><span class="sxs-lookup"><span data-stu-id="68436-120">Name</span></span>      |<span data-ttu-id="68436-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="68436-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="68436-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="68436-122">Authorization</span></span>  | <span data-ttu-id="68436-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="68436-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="68436-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68436-124">Request body</span></span>
<span data-ttu-id="68436-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="68436-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="68436-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="68436-126">Response</span></span>
<span data-ttu-id="68436-127">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [bookingBusiness](../resources/bookingbusiness.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68436-127">If successful, this method returns a `200 OK` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="68436-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68436-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68436-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68436-129">Request</span></span>
<span data-ttu-id="68436-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="68436-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="68436-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="68436-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingbusiness"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Fabrikam@M365B489948.onmicrosoft.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="68436-132">C#</span><span class="sxs-lookup"><span data-stu-id="68436-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="68436-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68436-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="68436-134">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="68436-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="68436-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="68436-135">Response</span></span>
<span data-ttu-id="68436-136">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="68436-136">The following is an example of the response.</span></span> <span data-ttu-id="68436-137">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="68436-137">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="68436-138">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68436-138">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingBusiness"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses/$entity",
    "id":"Fabrikam@M365B489948.onmicrosoft.com",
    "displayName":"Fabrikam",
    "businessType":"",
    "phone":"206-555-0100",
    "email":"manager@fabrikam.com",
    "webSiteUrl":"https://www.fabrikam.com/",
    "defaultCurrencyIso":"USD",
    "isPublished":false,
    "publicUrl":null,
    "address":{
        "type":"home",
        "postOfficeBox":"",
        "street":"4567 Main Street",
        "city":"Buffalo",
        "state":"NY",
        "countryOrRegion":"USA",
        "postalCode":"98052"
    },
    "businessHours":[
        {
            "day":"monday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"tuesday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"wednesday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"thursday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"friday",
            "timeSlots":[
                {
                    "start":"08:00:00.0000000",
                    "end":"17:00:00.0000000"
                }
            ]
        },
        {
            "day":"saturday",
            "timeSlots":[

            ]
        },
        {
            "day":"sunday",
            "timeSlots":[

            ]
        }
    ],
    "schedulingPolicy":{
        "timeSlotInterval":"PT30M",
        "minimumLeadTime":"P1D",
        "maximumAdvance":"P365D",
        "sendConfirmationsToOwner":true,
        "allowStaffSelection":true
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
