---
title: Obter bookingBusiness
description: Obtenha as propriedades e os relacionamentos de um objeto bookingBusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: cb6dcc9fc1b31d9f07fb2bd8ad8d7cffcbc7416f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441285"
---
# <a name="get-bookingbusiness"></a><span data-ttu-id="c715f-103">Obter bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="c715f-103">Get bookingBusiness</span></span>

<span data-ttu-id="c715f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c715f-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c715f-105">Obtenha as propriedades e os relacionamentos de um objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="c715f-105">Get the properties and relationships of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c715f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c715f-106">Permissions</span></span>
<span data-ttu-id="c715f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c715f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c715f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c715f-109">Permission type</span></span>      | <span data-ttu-id="c715f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c715f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c715f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c715f-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="c715f-112">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="c715f-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="c715f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c715f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c715f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c715f-114">Not supported.</span></span>   |
|<span data-ttu-id="c715f-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c715f-115">Application</span></span> | <span data-ttu-id="c715f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c715f-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c715f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c715f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c715f-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c715f-118">Optional query parameters</span></span>
<span data-ttu-id="c715f-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c715f-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c715f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c715f-120">Request headers</span></span>
| <span data-ttu-id="c715f-121">Nome</span><span class="sxs-lookup"><span data-stu-id="c715f-121">Name</span></span>      |<span data-ttu-id="c715f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c715f-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c715f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c715f-123">Authorization</span></span>  | <span data-ttu-id="c715f-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="c715f-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="c715f-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c715f-125">Request body</span></span>
<span data-ttu-id="c715f-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c715f-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c715f-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c715f-127">Response</span></span>
<span data-ttu-id="c715f-128">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [bookingBusiness](../resources/bookingbusiness.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c715f-128">If successful, this method returns a `200 OK` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c715f-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c715f-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c715f-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c715f-130">Request</span></span>
<span data-ttu-id="c715f-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c715f-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c715f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c715f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_bookingbusiness"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Fabrikam@M365B489948.onmicrosoft.com
```
# <a name="c"></a>[<span data-ttu-id="c715f-133">C#</span><span class="sxs-lookup"><span data-stu-id="c715f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c715f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c715f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c715f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c715f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c715f-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c715f-136">Response</span></span>
<span data-ttu-id="c715f-137">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="c715f-137">The following is an example of the response.</span></span> <span data-ttu-id="c715f-138">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="c715f-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c715f-139">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c715f-139">All of the properties will be returned from an actual call.</span></span>
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
