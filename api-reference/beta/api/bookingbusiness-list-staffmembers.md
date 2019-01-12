---
title: Lista staffMembers
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 81f170e101ad2aa600991cb79eaccdc65db8e4be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951380"
---
# <a name="list-staffmembers"></a><span data-ttu-id="9827d-104">Lista staffMembers</span><span class="sxs-lookup"><span data-stu-id="9827d-104">List staffMembers</span></span>

 > <span data-ttu-id="9827d-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9827d-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9827d-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9827d-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="9827d-107">Obtenha uma lista de objetos [bookingStaffMember](../resources/bookingstaffmember.md) no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="9827d-107">Get a list of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="9827d-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="9827d-108">Permissions</span></span>
<span data-ttu-id="9827d-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9827d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9827d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9827d-111">Permission type</span></span>      | <span data-ttu-id="9827d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9827d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9827d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9827d-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="9827d-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="9827d-114">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="9827d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9827d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9827d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9827d-116">Not supported.</span></span>   |
|<span data-ttu-id="9827d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9827d-117">Application</span></span> | <span data-ttu-id="9827d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9827d-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="9827d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9827d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="9827d-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="9827d-120">Optional query parameters</span></span>
<span data-ttu-id="9827d-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="9827d-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9827d-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9827d-122">Request headers</span></span>
| <span data-ttu-id="9827d-123">Nome</span><span class="sxs-lookup"><span data-stu-id="9827d-123">Name</span></span>      |<span data-ttu-id="9827d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="9827d-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9827d-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="9827d-125">Authorization</span></span>  | <span data-ttu-id="9827d-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="9827d-126">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="9827d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9827d-127">Request body</span></span>
<span data-ttu-id="9827d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9827d-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9827d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9827d-129">Response</span></span>
<span data-ttu-id="9827d-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [bookingStaffMember](../resources/bookingstaffmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9827d-130">If successful, this method returns a `200 OK` response code and collection of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9827d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9827d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9827d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9827d-132">Request</span></span>
<span data-ttu-id="9827d-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="9827d-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_staffmembers"
}-->
```http
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffMembers
```
##### <a name="response"></a><span data-ttu-id="9827d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9827d-134">Response</span></span>
<span data-ttu-id="9827d-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="9827d-135">The following is an example of the response.</span></span> <span data-ttu-id="9827d-136">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="9827d-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="9827d-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9827d-137">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List staffMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
