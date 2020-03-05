---
title: Atualizar bookingstaffmember
description: Atualiza as propriedades de um bookingStaffMember no bookingbusiness especificado.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: apiPageType
ms.openlocfilehash: e710d98ffd287e2c763608d899f74ddf2e6ce82c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441064"
---
# <a name="update-bookingstaffmember"></a><span data-ttu-id="2483c-103">Atualizar bookingstaffmember</span><span class="sxs-lookup"><span data-stu-id="2483c-103">Update bookingstaffmember</span></span>

<span data-ttu-id="2483c-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2483c-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2483c-105">Atualiza as propriedades de um [bookingStaffMember](../resources/bookingstaffmember.md) no [bookingbusiness](../resources/bookingbusiness.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="2483c-105">Update the properties of a [bookingStaffMember](../resources/bookingstaffmember.md) in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="2483c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="2483c-106">Permissions</span></span>
<span data-ttu-id="2483c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2483c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2483c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2483c-109">Permission type</span></span>      | <span data-ttu-id="2483c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2483c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2483c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2483c-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="2483c-112">Bookings. ReadWrite. All, bookings. Manage. All</span><span class="sxs-lookup"><span data-stu-id="2483c-112">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="2483c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2483c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2483c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2483c-114">Not supported.</span></span>   |
|<span data-ttu-id="2483c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2483c-115">Application</span></span> | <span data-ttu-id="2483c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2483c-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="2483c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2483c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /bookingBusinesses/{id}/staffMembers/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="2483c-118">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="2483c-118">Optional request headers</span></span>
| <span data-ttu-id="2483c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="2483c-119">Name</span></span>       | <span data-ttu-id="2483c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2483c-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2483c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2483c-121">Authorization</span></span>  | <span data-ttu-id="2483c-122">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="2483c-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="2483c-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2483c-123">Request body</span></span>
<span data-ttu-id="2483c-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2483c-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2483c-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2483c-127">Property</span></span>     | <span data-ttu-id="2483c-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="2483c-128">Type</span></span>   |<span data-ttu-id="2483c-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="2483c-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2483c-130">availabilityIsAffectedByPersonalCalendar</span><span class="sxs-lookup"><span data-stu-id="2483c-130">availabilityIsAffectedByPersonalCalendar</span></span>|<span data-ttu-id="2483c-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="2483c-131">Boolean</span></span>|<span data-ttu-id="2483c-132">True significa que, se o membro da equipe for um usuário do Office 365, a API Books usa o calendário pessoal do membro da equipe no Office 365, bem como a propriedade **workingHours** para determinar a disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="2483c-132">True means that if the staff member is an Office 365 user, the Bookings API uses the staff member's personal calendar in Office 365 as well as the **workingHours** property to determine availability.</span></span> |
|<span data-ttu-id="2483c-133">colorIndex</span><span class="sxs-lookup"><span data-stu-id="2483c-133">colorIndex</span></span>|<span data-ttu-id="2483c-134">Int32</span><span class="sxs-lookup"><span data-stu-id="2483c-134">Int32</span></span>|<span data-ttu-id="2483c-135">Identifica uma cor para representar o membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="2483c-135">Identifies a color to represent the staff member.</span></span> <span data-ttu-id="2483c-136">A cor corresponde à paleta de cores na página de **detalhes da equipe** no aplicativo de reservas.</span><span class="sxs-lookup"><span data-stu-id="2483c-136">The color corresponds to the color palette in the **Staff details** page in the Bookings app.</span></span>|
|<span data-ttu-id="2483c-137">displayName</span><span class="sxs-lookup"><span data-stu-id="2483c-137">displayName</span></span>|<span data-ttu-id="2483c-138">String</span><span class="sxs-lookup"><span data-stu-id="2483c-138">String</span></span>|<span data-ttu-id="2483c-139">O nome do membro da equipe, conforme exibido para os clientes.</span><span class="sxs-lookup"><span data-stu-id="2483c-139">The name of the staff member, as displayed to customers.</span></span>|
|<span data-ttu-id="2483c-140">emailAddress</span><span class="sxs-lookup"><span data-stu-id="2483c-140">emailAddress</span></span>|<span data-ttu-id="2483c-141">String</span><span class="sxs-lookup"><span data-stu-id="2483c-141">String</span></span>|<span data-ttu-id="2483c-142">O endereço de email do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="2483c-142">The email address of the staff member.</span></span> <span data-ttu-id="2483c-143">Isso pode ser no mesmo locatário do Office 365 que a empresa ou em um domínio de email diferente.</span><span class="sxs-lookup"><span data-stu-id="2483c-143">This can be in the same Office 365 tenant as the business, or in a different email domain.</span></span> <span data-ttu-id="2483c-144">Esse endereço de email será usado se a propriedade **sendConfirmationsToOwner** estiver definida como true na política de agendamento da empresa.</span><span class="sxs-lookup"><span data-stu-id="2483c-144">This email address is used if the **sendConfirmationsToOwner** property is set to true in the scheduling policy of the business.</span></span>|
|<span data-ttu-id="2483c-145">role</span><span class="sxs-lookup"><span data-stu-id="2483c-145">role</span></span>|<span data-ttu-id="2483c-146">string</span><span class="sxs-lookup"><span data-stu-id="2483c-146">string</span></span>| <span data-ttu-id="2483c-147">A função do membro da equipe na empresa.</span><span class="sxs-lookup"><span data-stu-id="2483c-147">The role of the staff member in the business.</span></span> <span data-ttu-id="2483c-148">Os valores possíveis são: `guest`, `administrator`, `viewer`, `externalGuest`.</span><span class="sxs-lookup"><span data-stu-id="2483c-148">Possible values are: `guest`, `administrator`, `viewer`, `externalGuest`.</span></span>|
|<span data-ttu-id="2483c-149">useBusinessHours</span><span class="sxs-lookup"><span data-stu-id="2483c-149">useBusinessHours</span></span>|<span data-ttu-id="2483c-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="2483c-150">Boolean</span></span>|<span data-ttu-id="2483c-151">True significa que a disponibilidade do membro da equipe é determinada pela propriedade **businessHours** da empresa.</span><span class="sxs-lookup"><span data-stu-id="2483c-151">True means the staff member's availability is determined by the **businessHours** property of the business.</span></span> <span data-ttu-id="2483c-152">False significa que a disponibilidade é determinada pela configuração da propriedade **workingHouse** do membro da equipe.</span><span class="sxs-lookup"><span data-stu-id="2483c-152">False means the availability is determined by the staff member's **workingHouse** property setting.</span></span>|
|<span data-ttu-id="2483c-153">workingHours</span><span class="sxs-lookup"><span data-stu-id="2483c-153">workingHours</span></span>|<span data-ttu-id="2483c-154">coleção [bookingWorkHours](../resources/bookingworkhours.md)</span><span class="sxs-lookup"><span data-stu-id="2483c-154">[bookingWorkHours](../resources/bookingworkhours.md) collection</span></span>|<span data-ttu-id="2483c-155">O intervalo de horas por dia da semana em que o membro da equipe está disponível para reserva.</span><span class="sxs-lookup"><span data-stu-id="2483c-155">The range of hours each day of the week that the staff member is available for booking.</span></span>|

## <a name="response"></a><span data-ttu-id="2483c-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="2483c-156">Response</span></span>
<span data-ttu-id="2483c-p107">Se bem-sucedido, este método retorna um código de resposta `204 No content`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2483c-p107">If successful, this method returns a `204 No content` response code. It does not return anything in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2483c-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2483c-159">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2483c-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2483c-160">Request</span></span>
<span data-ttu-id="2483c-161">O exemplo a seguir altera a agenda do membro da equipe para que ela tenha opções de segunda-feira.</span><span class="sxs-lookup"><span data-stu-id="2483c-161">The following example changes the staff member's schedule to have Mondays off.</span></span>

# <a name="http"></a>[<span data-ttu-id="2483c-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="2483c-162">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2483c-163">C#</span><span class="sxs-lookup"><span data-stu-id="2483c-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-bookingstaffmember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2483c-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2483c-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-bookingstaffmember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2483c-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2483c-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-bookingstaffmember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="2483c-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="2483c-166">Response</span></span>
<span data-ttu-id="2483c-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2483c-167">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
