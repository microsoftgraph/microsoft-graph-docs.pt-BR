---
title: Listar staffMembers
description: Obtenha uma lista de objetos bookingStaffMember no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 317fa38932bb5dc813b9b676bef26f73a6020daf
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322583"
---
# <a name="list-staffmembers"></a><span data-ttu-id="dc50e-103">Listar staffMembers</span><span class="sxs-lookup"><span data-stu-id="dc50e-103">List staffMembers</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc50e-104">Obtenha uma lista de objetos [bookingStaffMember](../resources/bookingstaffmember.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="dc50e-104">Get a list of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="dc50e-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="dc50e-105">Permissions</span></span>
<span data-ttu-id="dc50e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc50e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc50e-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc50e-108">Permission type</span></span>      | <span data-ttu-id="dc50e-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="dc50e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc50e-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc50e-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="dc50e-111">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="dc50e-111">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="dc50e-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc50e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc50e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc50e-113">Not supported.</span></span>   |
|<span data-ttu-id="dc50e-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc50e-114">Application</span></span> | <span data-ttu-id="dc50e-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc50e-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="dc50e-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc50e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dc50e-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dc50e-117">Optional query parameters</span></span>
<span data-ttu-id="dc50e-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dc50e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc50e-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc50e-119">Request headers</span></span>
| <span data-ttu-id="dc50e-120">Nome</span><span class="sxs-lookup"><span data-stu-id="dc50e-120">Name</span></span>      |<span data-ttu-id="dc50e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc50e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dc50e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc50e-122">Authorization</span></span>  | <span data-ttu-id="dc50e-123">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="dc50e-123">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc50e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc50e-124">Request body</span></span>
<span data-ttu-id="dc50e-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc50e-125">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="dc50e-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc50e-126">Response</span></span>
<span data-ttu-id="dc50e-127">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [bookingStaffMember](../resources/bookingstaffmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dc50e-127">If successful, this method returns a `200 OK` response code and collection of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dc50e-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc50e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc50e-129">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc50e-129">Request</span></span>
<span data-ttu-id="dc50e-130">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc50e-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_staffmembers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffMembers
```
##### <a name="response"></a><span data-ttu-id="dc50e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc50e-131">Response</span></span>
<span data-ttu-id="dc50e-132">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="dc50e-132">The following is an example of the response.</span></span> <span data-ttu-id="dc50e-133">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="dc50e-133">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="dc50e-134">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc50e-134">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingStaffMember",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/staffMembers",
    "value":[
        {
            "id":"8ee1c803-a1fa-406d-8259-7ab53233f148",
            "displayName":"Dana Swope",
            "emailAddress":"danas@contoso.com",
            "availabilityIsAffectedByPersonalCalendar":false,
            "colorIndex":1,
            "role":"externalGuest",
            "useBusinessHours":true,
            "workingHours":[
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
                }
            ]
        },
        {
            "id":"71d64d0e-7225-49b6-b0b1-070d476cda51",
            "displayName":"Samantha Booth",
            "emailAddress":"samanthab@M365B489948.OnMicrosoft.com",
            "availabilityIsAffectedByPersonalCalendar":true,
            "colorIndex":0,
            "role":"administrator",
            "useBusinessHours":true,
            "workingHours":[
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
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List staffMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
