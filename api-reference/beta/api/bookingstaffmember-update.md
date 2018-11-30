---
title: Atualizar bookingstaffmember
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: 99501f31ccd2b810d6a0c7f836d5b70bb98f223b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034121"
---
# <a name="update-bookingstaffmember"></a><span data-ttu-id="e3825-104">Atualizar bookingstaffmember</span><span class="sxs-lookup"><span data-stu-id="e3825-104">Update bookingstaffmember</span></span>

 > <span data-ttu-id="e3825-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e3825-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3825-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e3825-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="e3825-107">Atualize as propriedades de um [bookingStaffMember](../resources/bookingstaffmember.md) no especificado [bookingbusiness](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="e3825-107">Update the properties of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="e3825-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="e3825-108">Permissions</span></span>
<span data-ttu-id="e3825-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3825-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3825-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3825-111">Permission type</span></span>      | <span data-ttu-id="e3825-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3825-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3825-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3825-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="e3825-114">Bookings.ReadWrite.All, Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="e3825-114">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="e3825-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3825-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3825-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3825-116">Not supported.</span></span>   |
|<span data-ttu-id="e3825-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3825-117">Application</span></span> | <span data-ttu-id="e3825-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3825-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="e3825-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3825-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="e3825-120">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="e3825-120">Optional request headers</span></span>
| <span data-ttu-id="e3825-121">Nome</span><span class="sxs-lookup"><span data-stu-id="e3825-121">Name</span></span>       | <span data-ttu-id="e3825-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3825-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e3825-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3825-123">Authorization</span></span>  | <span data-ttu-id="e3825-124">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="e3825-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3825-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3825-125">Request body</span></span>
<span data-ttu-id="e3825-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="e3825-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e3825-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3825-129">Property</span></span>     | <span data-ttu-id="e3825-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3825-130">Type</span></span>   |<span data-ttu-id="e3825-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3825-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3825-132">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="e3825-132">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="e3825-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="e3825-133">Boolean</span></span>|<span data-ttu-id="e3825-134">True significa que, se o membro da equipe é um usuário do Office 365, a API de reservas usa a calendário pessoal do membro da equipe no Office 365, bem como a propriedade **workingHours** para determinar a disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="e3825-134">True means that if the staff member is an Office 365 user, the Bookings API uses the staff member's personal calendar in Office 365 as well as the **workingHours** property to determine availability.</span></span> |
|<span data-ttu-id="e3825-135">colorIndex</span><span class="sxs-lookup"><span data-stu-id="e3825-135">colorIndex</span></span>|<span data-ttu-id="e3825-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e3825-136">Int32</span></span>|<span data-ttu-id="e3825-137">Identifica uma cor para representar o membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="e3825-137">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="e3825-138">A cor corresponde à paleta de cores na página **detalhes da equipe** no aplicativo reservas.</span><span class="sxs-lookup"><span data-stu-id="e3825-138">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="e3825-139">displayName</span><span class="sxs-lookup"><span data-stu-id="e3825-139">displayName</span></span>|<span data-ttu-id="e3825-140">String</span><span class="sxs-lookup"><span data-stu-id="e3825-140">String</span></span>|<span data-ttu-id="e3825-141">O nome do membro da equipe, como exibido aos clientes.</span><span class="sxs-lookup"><span data-stu-id="e3825-141">The name of the staff member, as displayed to customers.</span></span>|
|<span data-ttu-id="e3825-142">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e3825-142">emailAddress</span></span>|<span data-ttu-id="e3825-143">String</span><span class="sxs-lookup"><span data-stu-id="e3825-143">String</span></span>|<span data-ttu-id="e3825-144">O endereço de email do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="e3825-144">The email address of the staff member.</span></span> <span data-ttu-id="e3825-145">Isso pode ser em inquilino do Office 365 como a empresa ou em um domínio de email diferentes.</span><span class="sxs-lookup"><span data-stu-id="e3825-145">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="e3825-146">Esse endereço de email é usado se a propriedade **sendConfirmationsToOwner** estiver definida como true na diretiva de agendamento dos negócios.</span><span class="sxs-lookup"><span data-stu-id="e3825-146">This email address is used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span>|
|<span data-ttu-id="e3825-147">role</span><span class="sxs-lookup"><span data-stu-id="e3825-147">role</span></span>|<span data-ttu-id="e3825-148">string</span><span class="sxs-lookup"><span data-stu-id="e3825-148">string</span></span>| <span data-ttu-id="e3825-149">A função de membro da equipe de negócios.</span><span class="sxs-lookup"><span data-stu-id="e3825-149">The role of the staff member in the business.</span></span> <span data-ttu-id="e3825-150">Os valores possíveis são: `guest`, `administrator`, `viewer`, `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="e3825-150">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span>|
|<span data-ttu-id="e3825-151">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="e3825-151">useBusinessHours</span></span>|<span data-ttu-id="e3825-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="e3825-152">Boolean</span></span>|<span data-ttu-id="e3825-153">True significa a que disponibilidade do membro da equipe é determinada pela propriedade **businessHours** dos negócios.</span><span class="sxs-lookup"><span data-stu-id="e3825-153">True means the staff member's availability is determined by the **businessHours** property of the business.</span></span> <span data-ttu-id="e3825-154">False significa que a disponibilidade é determinada pela configuração da propriedade **workingHouse** do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="e3825-154">False means the availability is determined by the staff member's **workingHouse** property setting.</span></span>|
|<span data-ttu-id="e3825-155">workingHours</span><span class="sxs-lookup"><span data-stu-id="e3825-155">workingHours</span></span>|<span data-ttu-id="e3825-156">coleção [bookingWorkHours](../resources/bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="e3825-156">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="e3825-157">O intervalo de horas por dia da semana em que o membro da equipe está disponível para marcação.</span><span class="sxs-lookup"><span data-stu-id="e3825-157">The range of hours each day of the week that the staff member is available for booking.</span></span>|

## <a name="response"></a><span data-ttu-id="e3825-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3825-158">Response</span></span>
<span data-ttu-id="e3825-p109">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3825-p109">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e3825-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3825-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3825-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3825-162">Request</span></span>
<span data-ttu-id="e3825-163">O exemplo a seguir altera a agenda do membro da equipe ter segundas-feiras.</span><span class="sxs-lookup"><span data-stu-id="e3825-163">The following example changes the staff member's schedule to have Mondays off.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_bookingstaffmember"
}-->
```http
PATCH https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/staffmembers/8ee1c803-a1fa-406d-8259-7ab53233f148
Content-type: application/json

{
    "workingHours":[
        {
            "@odata.type":"#microsoft.graph.bookingWorkHours",
            "day@odata.type":"#microsoft.graph.dayOfWeek",
            "day":"monday",
            "timeSlots@odata.type":"#Collection(microsoft.graph.bookingWorkTimeSlot)",
            "timeSlots":[
   
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
##### <a name="response"></a><span data-ttu-id="e3825-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3825-164">Response</span></span>
<span data-ttu-id="e3825-165">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="e3825-165">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update bookingstaffmember",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->