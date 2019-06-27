---
title: Atualizar bookingstaffmember
description: Atualiza as propriedades de um bookingStaffMember no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 97649a47aba9cd63d58e40e388bf9bd8292156b9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262465"
---
# <a name="update-bookingstaffmember"></a><span data-ttu-id="775ca-103">Atualizar bookingstaffmember</span><span class="sxs-lookup"><span data-stu-id="775ca-103">Update bookingstaffmember</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="775ca-104">Atualiza as propriedades de um [bookingStaffMember](../resources/bookingstaffmember.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="775ca-104">Update the properties of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="775ca-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="775ca-105">Permissions</span></span>
<span data-ttu-id="775ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="775ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="775ca-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="775ca-108">Permission type</span></span>      | <span data-ttu-id="775ca-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="775ca-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="775ca-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="775ca-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="775ca-111">Bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="775ca-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="775ca-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="775ca-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="775ca-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="775ca-113">Not supported.</span></span>   |
|<span data-ttu-id="775ca-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="775ca-114">Application</span></span> | <span data-ttu-id="775ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="775ca-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="775ca-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="775ca-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="775ca-117">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="775ca-117">Optional request headers</span></span>
| <span data-ttu-id="775ca-118">Nome</span><span class="sxs-lookup"><span data-stu-id="775ca-118">Name</span></span>       | <span data-ttu-id="775ca-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="775ca-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="775ca-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="775ca-120">Authorization</span></span>  | <span data-ttu-id="775ca-121">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="775ca-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="775ca-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="775ca-122">Request body</span></span>
<span data-ttu-id="775ca-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="775ca-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="775ca-126">Propriedade</span><span class="sxs-lookup"><span data-stu-id="775ca-126">Property</span></span>     | <span data-ttu-id="775ca-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="775ca-127">Type</span></span>   |<span data-ttu-id="775ca-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="775ca-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="775ca-129">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="775ca-129">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="775ca-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="775ca-130">Boolean</span></span>|<span data-ttu-id="775ca-131">True significa que, se o membro da equipe for um usuário do Office 365, a API Books usa o calendário pessoal do membro da equipe no Office 365, bem como a propriedade **workingHours** para determinar a disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="775ca-131">True means that if the staff member is an Office 365 user, the Bookings API uses the staff member's personal calendar in Office 365 as well as the **workingHours** property to determine availability.</span></span> |
|<span data-ttu-id="775ca-132">colorIndex</span><span class="sxs-lookup"><span data-stu-id="775ca-132">colorIndex</span></span>|<span data-ttu-id="775ca-133">Int32</span><span class="sxs-lookup"><span data-stu-id="775ca-133">Int32</span></span>|<span data-ttu-id="775ca-134">Identifica uma cor para representar o membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="775ca-134">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="775ca-135">A cor corresponde à paleta de cores na página de **detalhes da equipe** no aplicativo de reservas.</span><span class="sxs-lookup"><span data-stu-id="775ca-135">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="775ca-136">displayName</span><span class="sxs-lookup"><span data-stu-id="775ca-136">displayName</span></span>|<span data-ttu-id="775ca-137">String</span><span class="sxs-lookup"><span data-stu-id="775ca-137">String</span></span>|<span data-ttu-id="775ca-138">O nome do membro da equipe, conforme exibido para os clientes.</span><span class="sxs-lookup"><span data-stu-id="775ca-138">The name of the staff member, as displayed to customers.</span></span>|
|<span data-ttu-id="775ca-139">emailAddress</span><span class="sxs-lookup"><span data-stu-id="775ca-139">emailAddress</span></span>|<span data-ttu-id="775ca-140">String</span><span class="sxs-lookup"><span data-stu-id="775ca-140">String</span></span>|<span data-ttu-id="775ca-141">O endereço de email do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="775ca-141">The email address of the staff member.</span></span> <span data-ttu-id="775ca-142">Isso pode ser no mesmo locatário do Office 365 que a empresa ou em um domínio de email diferente.</span><span class="sxs-lookup"><span data-stu-id="775ca-142">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="775ca-143">Esse endereço de email será usado se a propriedade **sendConfirmationsToOwner** estiver definida como true na política de agendamento da empresa.</span><span class="sxs-lookup"><span data-stu-id="775ca-143">This email address is used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span>|
|<span data-ttu-id="775ca-144">role</span><span class="sxs-lookup"><span data-stu-id="775ca-144">role</span></span>|<span data-ttu-id="775ca-145">string</span><span class="sxs-lookup"><span data-stu-id="775ca-145">string</span></span>| <span data-ttu-id="775ca-146">A função do membro da equipe na empresa.</span><span class="sxs-lookup"><span data-stu-id="775ca-146">The role of the staff member in the business.</span></span> <span data-ttu-id="775ca-147">Os valores possíveis são: `guest`, `administrator`, `viewer`, `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="775ca-147">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span>|
|<span data-ttu-id="775ca-148">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="775ca-148">useBusinessHours</span></span>|<span data-ttu-id="775ca-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="775ca-149">Boolean</span></span>|<span data-ttu-id="775ca-150">True significa que a disponibilidade do membro da equipe é determinada pela propriedade **businessHours** da empresa.</span><span class="sxs-lookup"><span data-stu-id="775ca-150">True means the staff member's availability is determined by the **businessHours** property of the business.</span></span> <span data-ttu-id="775ca-151">False significa que a disponibilidade é determinada pela configuração da propriedade **workingHouse** do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="775ca-151">False means the availability is determined by the staff member's **workingHouse** property setting.</span></span>|
|<span data-ttu-id="775ca-152">workingHours</span><span class="sxs-lookup"><span data-stu-id="775ca-152">workingHours</span></span>|<span data-ttu-id="775ca-153">coleção [bookingWorkHours](../resources/bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="775ca-153">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="775ca-154">O intervalo de horas por dia da semana em que o membro da equipe está disponível para reserva.</span><span class="sxs-lookup"><span data-stu-id="775ca-154">The range of hours each day of the week that the staff member is available for booking.</span></span>|

## <a name="response"></a><span data-ttu-id="775ca-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="775ca-155">Response</span></span>
<span data-ttu-id="775ca-p107">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="775ca-p107">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="775ca-158">Exemplo</span><span class="sxs-lookup"><span data-stu-id="775ca-158">Example</span></span>
##### <a name="request"></a><span data-ttu-id="775ca-159">Solicitação</span><span class="sxs-lookup"><span data-stu-id="775ca-159">Request</span></span>
<span data-ttu-id="775ca-160">O exemplo a seguir altera a agenda do membro da equipe para que ela tenha opções de segunda-feira.</span><span class="sxs-lookup"><span data-stu-id="775ca-160">The following example changes the staff member's schedule to have Mondays off.</span></span>
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
##### <a name="response"></a><span data-ttu-id="775ca-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="775ca-161">Response</span></span>
<span data-ttu-id="775ca-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="775ca-162">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="775ca-163">Código de amostra do SDK</span><span class="sxs-lookup"><span data-stu-id="775ca-163">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="775ca-164">C#</span><span class="sxs-lookup"><span data-stu-id="775ca-164">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_bookingstaffmember-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="775ca-165">Javascript</span><span class="sxs-lookup"><span data-stu-id="775ca-165">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_bookingstaffmember-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="775ca-166">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="775ca-166">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_bookingstaffmember-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update bookingstaffmember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingstaffmember-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/bookingstaffmember-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/bookingstaffmember-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
