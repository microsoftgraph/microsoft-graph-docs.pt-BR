---
title: Obter bookingBusiness
description: Obtenha as propriedades e os relacionamentos de um objeto bookingBusiness.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 229da03e377f1ff0add73195505c359c9fd68121
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462402"
---
# <a name="get-bookingbusiness"></a><span data-ttu-id="574b3-103">Obter bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="574b3-103">Get bookingBusiness</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="574b3-104">Obtenha as propriedades e os relacionamentos de um objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="574b3-104">Get the properties and relationships of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="574b3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="574b3-105">Permissions</span></span>
<span data-ttu-id="574b3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="574b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="574b3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="574b3-108">Permission type</span></span>      | <span data-ttu-id="574b3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="574b3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="574b3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="574b3-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="574b3-111">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="574b3-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="574b3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="574b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="574b3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="574b3-113">Not supported.</span></span>   |
|<span data-ttu-id="574b3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="574b3-114">Application</span></span> | <span data-ttu-id="574b3-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="574b3-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="574b3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="574b3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="574b3-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="574b3-117">Optional query parameters</span></span>
<span data-ttu-id="574b3-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="574b3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="574b3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="574b3-119">Request headers</span></span>
| <span data-ttu-id="574b3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="574b3-120">Name</span></span>      |<span data-ttu-id="574b3-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="574b3-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="574b3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="574b3-122">Authorization</span></span>  | <span data-ttu-id="574b3-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="574b3-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="574b3-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="574b3-124">Request body</span></span>
<span data-ttu-id="574b3-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="574b3-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="574b3-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="574b3-126">Response</span></span>
<span data-ttu-id="574b3-127">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [bookingBusiness](../resources/bookingbusiness.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="574b3-127">If successful, this method returns a `200 OK` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="574b3-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="574b3-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="574b3-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="574b3-129">Request</span></span>
<span data-ttu-id="574b3-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="574b3-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusiness"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="574b3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="574b3-131">Response</span></span>
<span data-ttu-id="574b3-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="574b3-132">The following is an example of the response.</span></span> <span data-ttu-id="574b3-133">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="574b3-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="574b3-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="574b3-134">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingbusiness-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
