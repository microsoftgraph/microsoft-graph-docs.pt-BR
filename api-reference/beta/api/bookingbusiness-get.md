---
title: Obter bookingBusiness
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 6df16d3c4dbb77c2e97e55fda1881a38c9270c22
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809517"
---
# <a name="get-bookingbusiness"></a><span data-ttu-id="08712-104">Obter bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="08712-104">Get bookingBusiness</span></span>

 > <span data-ttu-id="08712-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="08712-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08712-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="08712-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="08712-107">Obtenha as propriedades e relacionamentos de um objeto [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="08712-107">Get the properties and relationships of a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="08712-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="08712-108">Permissions</span></span>
<span data-ttu-id="08712-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08712-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08712-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="08712-111">Permission type</span></span>      | <span data-ttu-id="08712-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="08712-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08712-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="08712-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="08712-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="08712-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="08712-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="08712-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08712-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08712-116">Not supported.</span></span>   |
|<span data-ttu-id="08712-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="08712-117">Application</span></span> | <span data-ttu-id="08712-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="08712-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="08712-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="08712-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/<id>
```
## <a name="optional-query-parameters"></a><span data-ttu-id="08712-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="08712-120">Optional query parameters</span></span>
<span data-ttu-id="08712-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="08712-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="08712-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="08712-122">Request headers</span></span>
| <span data-ttu-id="08712-123">Nome</span><span class="sxs-lookup"><span data-stu-id="08712-123">Name</span></span>      |<span data-ttu-id="08712-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="08712-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="08712-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="08712-125">Authorization</span></span>  | <span data-ttu-id="08712-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="08712-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="08712-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="08712-127">Request body</span></span>
<span data-ttu-id="08712-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="08712-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="08712-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="08712-129">Response</span></span>
<span data-ttu-id="08712-130">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [bookingBusiness](../resources/bookingbusiness.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="08712-130">If successful, this method returns a `200 OK` response code and [bookingBusiness](../resources/bookingbusiness.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="08712-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="08712-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="08712-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="08712-132">Request</span></span>
<span data-ttu-id="08712-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="08712-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_bookingbusiness"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="08712-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="08712-134">Response</span></span>
<span data-ttu-id="08712-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="08712-135">The following is an example of the response.</span></span> <span data-ttu-id="08712-136">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="08712-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="08712-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="08712-137">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
