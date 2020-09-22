---
title: Criar bookingStaffMember
description: Criar um novo membro da equipe no bookingbusiness especificado.
localization_priority: Normal
author: arvindmicrosoft
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: 19679d2f6a513017fe9d89a8922477641070da6e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47987985"
---
# <a name="create-bookingstaffmember"></a><span data-ttu-id="bdf91-103">Criar bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="bdf91-103">Create bookingStaffMember</span></span>

<span data-ttu-id="bdf91-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bdf91-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdf91-105">Criar um novo [membro da equipe](../resources/bookingstaffmember.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="bdf91-105">Create a new [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="bdf91-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="bdf91-106">Permissions</span></span>
<span data-ttu-id="bdf91-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdf91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bdf91-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdf91-109">Permission type</span></span>      | <span data-ttu-id="bdf91-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bdf91-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdf91-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdf91-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="bdf91-112">Bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="bdf91-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="bdf91-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdf91-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdf91-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdf91-114">Not supported.</span></span>   |
|<span data-ttu-id="bdf91-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdf91-115">Application</span></span> | <span data-ttu-id="bdf91-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bdf91-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="bdf91-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdf91-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/staffMembers

```
## <a name="request-headers"></a><span data-ttu-id="bdf91-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdf91-118">Request headers</span></span>
| <span data-ttu-id="bdf91-119">Nome</span><span class="sxs-lookup"><span data-stu-id="bdf91-119">Name</span></span>       | <span data-ttu-id="bdf91-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdf91-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bdf91-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdf91-121">Authorization</span></span>  | <span data-ttu-id="bdf91-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="bdf91-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="bdf91-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdf91-123">Request body</span></span>
<span data-ttu-id="bdf91-124">No corpo da solicitação, forneça uma representação JSON do objeto [bookingStaffMember](../resources/bookingstaffmember.md) .</span><span class="sxs-lookup"><span data-stu-id="bdf91-124">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span> <span data-ttu-id="bdf91-125">Você deve incluir as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="bdf91-125">You must include the following properties:</span></span>

- <span data-ttu-id="bdf91-126">**displayName**</span><span class="sxs-lookup"><span data-stu-id="bdf91-126">**displayName**</span></span>
- <span data-ttu-id="bdf91-127">**emailAddress**</span><span class="sxs-lookup"><span data-stu-id="bdf91-127">**emailAddress**</span></span>
- <span data-ttu-id="bdf91-128">**Role**</span><span class="sxs-lookup"><span data-stu-id="bdf91-128">**role**</span></span>


## <a name="response"></a><span data-ttu-id="bdf91-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdf91-129">Response</span></span>
<span data-ttu-id="bdf91-130">Se bem-sucedido, este método retorna o `201, Created` código de resposta e o objeto [bookingStaffMember](../resources/bookingstaffmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdf91-130">If successful, this method returns `201, Created` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdf91-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bdf91-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bdf91-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdf91-132">Request</span></span>
<span data-ttu-id="bdf91-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdf91-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bdf91-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="bdf91-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_bookingstaffmember_from_bookingbusiness"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/{id}/staffMembers
Content-type: application/json
Content-length: 309

{
    "@odata.type":"#microsoft.graph.bookingStaffMember",
    "colorIndex":1,
    "displayName":"Dana Swope",
    "emailAddress":"danas@contoso.com",
    "role@odata.type":"#microsoft.graph.bookingStaffRole",
    "role":"externalGuest",
    "useBusinessHours":true,
    "workingHours@odata.type":"#Collection(microsoft.graph.bookingWorkHours)",
    "workingHours":[
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"monday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"tuesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"wednesday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"thursday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        },
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"friday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
                {
                    "@odata.type":"#microsoft.graph.bookingWorkTimeSlot",
                    "end":"17:00:00.0000000",
                    "start":"08:00:00.0000000"
                }
            ]
        }
    ]
}
```
# <a name="c"></a>[<span data-ttu-id="bdf91-135">C#</span><span class="sxs-lookup"><span data-stu-id="bdf91-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bookingstaffmember-from-bookingbusiness-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bdf91-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bdf91-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bookingstaffmember-from-bookingbusiness-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bdf91-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bdf91-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bookingstaffmember-from-bookingbusiness-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="bdf91-138">No corpo da solicitação, forneça uma representação JSON do objeto [bookingStaffMember](../resources/bookingstaffmember.md) .</span><span class="sxs-lookup"><span data-stu-id="bdf91-138">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="bdf91-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdf91-139">Response</span></span>
<span data-ttu-id="bdf91-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bdf91-140">The following is an example of the response.</span></span> <span data-ttu-id="bdf91-141">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="bdf91-141">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="bdf91-142">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bdf91-142">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingStaffMember"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#bookingBusinesses('Contosolunchdelivery%40M365B489948.onmicrosoft.com')/staffMembers/$entity",
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
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


