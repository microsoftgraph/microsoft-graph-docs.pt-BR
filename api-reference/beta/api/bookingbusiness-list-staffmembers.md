---
title: Listar staffMembers
description: Obtenha uma lista de objetos bookingStaffMember no bookingbusiness especificado.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 4d60a2cf9e0ef5fca999522ad9136e1a4178dabe
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960730"
---
# <a name="list-staffmembers"></a><span data-ttu-id="25bc1-103">Listar staffMembers</span><span class="sxs-lookup"><span data-stu-id="25bc1-103">List staffMembers</span></span>

<span data-ttu-id="25bc1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25bc1-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25bc1-105">Obtenha uma lista de objetos [bookingStaffMember](../resources/bookingstaffmember.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="25bc1-105">Get a list of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="25bc1-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="25bc1-106">Permissions</span></span>
<span data-ttu-id="25bc1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25bc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25bc1-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25bc1-109">Permission type</span></span>      | <span data-ttu-id="25bc1-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25bc1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25bc1-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25bc1-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="25bc1-112">Bookings. Read. All, BookingsAppointment. ReadWrite. All, bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="25bc1-112">Bookings.Read.All, BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="25bc1-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25bc1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25bc1-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25bc1-114">Not supported.</span></span>   |
|<span data-ttu-id="25bc1-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25bc1-115">Application</span></span> | <span data-ttu-id="25bc1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25bc1-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="25bc1-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25bc1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /bookingBusinesses/{id}/staffMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="25bc1-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="25bc1-118">Optional query parameters</span></span>
<span data-ttu-id="25bc1-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="25bc1-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="25bc1-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25bc1-120">Request headers</span></span>
| <span data-ttu-id="25bc1-121">Nome</span><span class="sxs-lookup"><span data-stu-id="25bc1-121">Name</span></span>      |<span data-ttu-id="25bc1-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="25bc1-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="25bc1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="25bc1-123">Authorization</span></span>  | <span data-ttu-id="25bc1-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="25bc1-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="25bc1-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25bc1-125">Request body</span></span>
<span data-ttu-id="25bc1-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25bc1-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="25bc1-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="25bc1-127">Response</span></span>
<span data-ttu-id="25bc1-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [bookingStaffMember](../resources/bookingstaffmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25bc1-128">If successful, this method returns a `200 OK` response code and collection of [bookingStaffMember](../resources/bookingstaffmember.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="25bc1-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25bc1-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25bc1-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25bc1-130">Request</span></span>
<span data-ttu-id="25bc1-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="25bc1-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="25bc1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="25bc1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_staffmembers"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffMembers
```
# <a name="c"></a>[<span data-ttu-id="25bc1-133">C#</span><span class="sxs-lookup"><span data-stu-id="25bc1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-staffmembers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="25bc1-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="25bc1-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-staffmembers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="25bc1-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="25bc1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-staffmembers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="25bc1-136">Java</span><span class="sxs-lookup"><span data-stu-id="25bc1-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-staffmembers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="25bc1-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="25bc1-137">Response</span></span>
<span data-ttu-id="25bc1-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="25bc1-138">The following is an example of the response.</span></span> <span data-ttu-id="25bc1-139">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="25bc1-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="25bc1-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25bc1-140">All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": [
  ]
}
-->
