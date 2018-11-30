---
title: Criar bookingStaffMember
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: 01983d5a0831b47c2eddfa45dad917f30bdd7b8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035029"
---
# <a name="create-bookingstaffmember"></a><span data-ttu-id="e4903-104">Criar bookingStaffMember</span><span class="sxs-lookup"><span data-stu-id="e4903-104">Create bookingStaffMember</span></span>

 > <span data-ttu-id="e4903-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e4903-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e4903-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e4903-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="e4903-107">Crie um novo [membro da equipe](../resources/bookingstaffmember.md) no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="e4903-107">Create a new [staff member](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="e4903-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="e4903-108">Permissions</span></span>
<span data-ttu-id="e4903-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4903-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4903-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e4903-111">Permission type</span></span>      | <span data-ttu-id="e4903-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e4903-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4903-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e4903-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="e4903-114">Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="e4903-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="e4903-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e4903-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4903-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4903-116">Not supported.</span></span>   |
|<span data-ttu-id="e4903-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e4903-117">Application</span></span> | <span data-ttu-id="e4903-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e4903-118">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="e4903-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e4903-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/staffMembers

```
## <a name="request-headers"></a><span data-ttu-id="e4903-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4903-120">Request headers</span></span>
| <span data-ttu-id="e4903-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e4903-121">Name</span></span>       | <span data-ttu-id="e4903-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4903-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e4903-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e4903-123">Authorization</span></span>  | <span data-ttu-id="e4903-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="e4903-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4903-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e4903-125">Request body</span></span>
<span data-ttu-id="e4903-126">No corpo da solicitação, fornece uma representação JSON do objeto [bookingStaffMember](../resources/bookingstaffmember.md) .</span><span class="sxs-lookup"><span data-stu-id="e4903-126">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span> <span data-ttu-id="e4903-127">Você deve incluir as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="e4903-127">You must include the following properties:</span></span>

- <span data-ttu-id="e4903-128">**displayName**</span><span class="sxs-lookup"><span data-stu-id="e4903-128">**displayName**</span></span>
- <span data-ttu-id="e4903-129">**emailAddress**</span><span class="sxs-lookup"><span data-stu-id="e4903-129">**emailAddress**</span></span>
- <span data-ttu-id="e4903-130">**função**</span><span class="sxs-lookup"><span data-stu-id="e4903-130">**role**</span></span>


## <a name="response"></a><span data-ttu-id="e4903-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4903-131">Response</span></span>
<span data-ttu-id="e4903-132">Se tiver êxito, este método retornará `201, Created` objeto response de código e [bookingStaffMember](../resources/bookingstaffmember.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e4903-132">If successful, this method returns `201, Created` response code and [bookingStaffMember](../resources/bookingstaffmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4903-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e4903-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4903-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e4903-134">Request</span></span>
<span data-ttu-id="e4903-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="e4903-135">The following is an example of the request.</span></span>
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
<span data-ttu-id="e4903-136">No corpo da solicitação, fornece uma representação JSON do objeto [bookingStaffMember](../resources/bookingstaffmember.md) .</span><span class="sxs-lookup"><span data-stu-id="e4903-136">In the request body, supply a JSON representation of [bookingStaffMember](../resources/bookingstaffmember.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e4903-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="e4903-137">Response</span></span>
<span data-ttu-id="e4903-138">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4903-138">The following is an example of the response.</span></span> <span data-ttu-id="e4903-139">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="e4903-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e4903-140">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e4903-140">All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create bookingStaffMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->