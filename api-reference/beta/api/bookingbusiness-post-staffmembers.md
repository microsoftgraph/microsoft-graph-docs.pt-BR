---
title: Criar bookingStaffMember
description: Criar um novo membro da equipe no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: f3f13f30f646da8bf0fc8e32075002c0e591e902
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461651"
---
# <a name="create-bookingstaffmember"></a><span data-ttu-id="72b91-103">Criar bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="72b91-103">Create bookingStaffMember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72b91-104">Criar um novo [membro da equipe](../resources/bookingstaffmember.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="72b91-104">Create a new [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="72b91-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="72b91-105">Permissions</span></span>
<span data-ttu-id="72b91-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72b91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72b91-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72b91-108">Permission type</span></span>      | <span data-ttu-id="72b91-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72b91-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72b91-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72b91-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="72b91-111">Bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="72b91-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="72b91-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72b91-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72b91-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72b91-113">Not supported.</span></span>   |
|<span data-ttu-id="72b91-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72b91-114">Application</span></span> | <span data-ttu-id="72b91-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72b91-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="72b91-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72b91-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/staffMembers

```
## <a name="request-headers"></a><span data-ttu-id="72b91-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72b91-117">Request headers</span></span>
| <span data-ttu-id="72b91-118">Nome</span><span class="sxs-lookup"><span data-stu-id="72b91-118">Name</span></span>       | <span data-ttu-id="72b91-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="72b91-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="72b91-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="72b91-120">Authorization</span></span>  | <span data-ttu-id="72b91-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="72b91-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="72b91-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72b91-122">Request body</span></span>
<span data-ttu-id="72b91-123">No corpo da solicitação, forneça uma representação JSON do objeto [bookingStaffMember](../resources/bookingstaffmember.md) .</span><span class="sxs-lookup"><span data-stu-id="72b91-123">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span> <span data-ttu-id="72b91-124">Você deve incluir as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="72b91-124">You must include the following properties:</span></span>

- <span data-ttu-id="72b91-125">**displayName**</span><span class="sxs-lookup"><span data-stu-id="72b91-125">**displayName**</span></span>
- <span data-ttu-id="72b91-126">**emailAddress**</span><span class="sxs-lookup"><span data-stu-id="72b91-126">**emailAddress**</span></span>
- <span data-ttu-id="72b91-127">**Role**</span><span class="sxs-lookup"><span data-stu-id="72b91-127">**role**</span></span>


## <a name="response"></a><span data-ttu-id="72b91-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="72b91-128">Response</span></span>
<span data-ttu-id="72b91-129">Se bem-sucedido, este método retorna `201, Created` o código de resposta e o objeto [bookingStaffMember](../resources/bookingstaffmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72b91-129">If successful, this method returns `201, Created` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72b91-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72b91-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="72b91-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72b91-131">Request</span></span>
<span data-ttu-id="72b91-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="72b91-132">The following is an example of the request.</span></span>
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
<span data-ttu-id="72b91-133">No corpo da solicitação, forneça uma representação JSON do objeto [bookingStaffMember](../resources/bookingstaffmember.md) .</span><span class="sxs-lookup"><span data-stu-id="72b91-133">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="72b91-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="72b91-134">Response</span></span>
<span data-ttu-id="72b91-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="72b91-135">The following is an example of the response.</span></span> <span data-ttu-id="72b91-136">Observação: o objeto de resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="72b91-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="72b91-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72b91-137">All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/bookingbusiness-post-staffmembers.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
