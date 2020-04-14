---
title: Obter bookingBusiness
description: Obtenha as propriedades e os relacionamentos de um objeto bookingBusiness.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 3b31f51b2e0c6e963cbef0cc9d3fd7c82c0c5b11
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43367381"
---
# <a name="get-bookingbusiness"></a><span data-ttu-id="f1d84-103">Obter bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="f1d84-103">Get bookingBusiness</span></span>

<span data-ttu-id="f1d84-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1d84-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1d84-105">Obtenha as propriedades e os relacionamentos de um objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="f1d84-105">Get the properties and relationships of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="f1d84-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f1d84-106">Permissions</span></span>
<span data-ttu-id="f1d84-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1d84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1d84-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1d84-109">Permission type</span></span>      | <span data-ttu-id="f1d84-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1d84-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1d84-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1d84-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="f1d84-112">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="f1d84-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="f1d84-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1d84-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1d84-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1d84-114">Not supported.</span></span>   |
|<span data-ttu-id="f1d84-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1d84-115">Application</span></span> | <span data-ttu-id="f1d84-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1d84-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="f1d84-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1d84-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f1d84-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f1d84-118">Optional query parameters</span></span>
<span data-ttu-id="f1d84-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f1d84-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f1d84-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1d84-120">Request headers</span></span>
| <span data-ttu-id="f1d84-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f1d84-121">Name</span></span>      |<span data-ttu-id="f1d84-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1d84-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f1d84-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1d84-123">Authorization</span></span>  | <span data-ttu-id="f1d84-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="f1d84-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1d84-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1d84-125">Request body</span></span>
<span data-ttu-id="f1d84-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f1d84-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="f1d84-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1d84-127">Response</span></span>
<span data-ttu-id="f1d84-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [bookingBusiness](../resources/bookingbusiness.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1d84-128">If successful, this method returns a `200 OK` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f1d84-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1d84-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f1d84-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1d84-130">Request</span></span>
<span data-ttu-id="f1d84-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1d84-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1d84-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1d84-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingbusiness"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Fabrikam@M365B489948.onmicrosoft.com
```
# <a name="c"></a>[<span data-ttu-id="f1d84-133">C#</span><span class="sxs-lookup"><span data-stu-id="f1d84-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1d84-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1d84-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1d84-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1d84-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="f1d84-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1d84-136">Response</span></span>
<span data-ttu-id="f1d84-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f1d84-137">The following is an example of the response.</span></span> <span data-ttu-id="f1d84-138">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="f1d84-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f1d84-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1d84-139">All of the properties will be returned from an actual call.</span></span>
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
