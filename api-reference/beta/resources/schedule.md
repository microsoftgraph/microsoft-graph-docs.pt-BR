---
title: tipo de recurso Schedule
description: Uma coleção de schedulingGroups, Shifts, timeOffReasons e timesOff dentro de uma equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 6bc92b18bd0529066ef9ade2df9c6ccee9628add
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895375"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="ae850-103">tipo de recurso Schedule</span><span class="sxs-lookup"><span data-stu-id="ae850-103">schedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae850-104">Uma coleção de objetos de grupo de [agendamento](schedulinggroup.md) , objetos [Shift](shift.md) , objetos [timeOffReason](timeoffreason.md) e objetos [timeOff](timeoff.md) dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="ae850-104">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="ae850-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="ae850-105">Methods</span></span>

| <span data-ttu-id="ae850-106">Método</span><span class="sxs-lookup"><span data-stu-id="ae850-106">Method</span></span>       | <span data-ttu-id="ae850-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ae850-107">Return Type</span></span>  |<span data-ttu-id="ae850-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae850-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ae850-109">Criar ou substituir agendamento</span><span class="sxs-lookup"><span data-stu-id="ae850-109">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="ae850-110">Cronograma</span><span class="sxs-lookup"><span data-stu-id="ae850-110">schedule</span></span>](schedule.md) | <span data-ttu-id="ae850-111">Criar ou substituir uma agenda.</span><span class="sxs-lookup"><span data-stu-id="ae850-111">Create or replace a schedule.</span></span>|
|[<span data-ttu-id="ae850-112">Obter cronograma</span><span class="sxs-lookup"><span data-stu-id="ae850-112">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="ae850-113">Cronograma</span><span class="sxs-lookup"><span data-stu-id="ae850-113">schedule</span></span>](schedule.md) | <span data-ttu-id="ae850-114">Obter um cronograma.</span><span class="sxs-lookup"><span data-stu-id="ae850-114">Get a schedule.</span></span>|
|[<span data-ttu-id="ae850-115">Compartilhar</span><span class="sxs-lookup"><span data-stu-id="ae850-115">Share</span></span>](../api/schedule-share.md) | <span data-ttu-id="ae850-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ae850-116">None</span></span> | <span data-ttu-id="ae850-117">Compartilhar um intervalo de tempo de agendamento com membros de agendamento.</span><span class="sxs-lookup"><span data-stu-id="ae850-117">Share a schedule time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="ae850-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae850-118">Properties</span></span>
|<span data-ttu-id="ae850-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ae850-119">Name</span></span>                   |<span data-ttu-id="ae850-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae850-120">Type</span></span>           |<span data-ttu-id="ae850-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae850-121">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ae850-122">id</span><span class="sxs-lookup"><span data-stu-id="ae850-122">id</span></span>                    |<span data-ttu-id="ae850-123">string</span><span class="sxs-lookup"><span data-stu-id="ae850-123">string</span></span>  |<span data-ttu-id="ae850-124">ID do cronograma.</span><span class="sxs-lookup"><span data-stu-id="ae850-124">ID of the schedule.</span></span>|
| <span data-ttu-id="ae850-125">enabled</span><span class="sxs-lookup"><span data-stu-id="ae850-125">enabled</span></span>               |<span data-ttu-id="ae850-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae850-126">Boolean</span></span>    | <span data-ttu-id="ae850-127">Indica se o cronograma está habilitado para a equipe.</span><span class="sxs-lookup"><span data-stu-id="ae850-127">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="ae850-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae850-128">Required.</span></span>|
| <span data-ttu-id="ae850-129">timeZone</span><span class="sxs-lookup"><span data-stu-id="ae850-129">timeZone</span></span>              |<span data-ttu-id="ae850-130">string</span><span class="sxs-lookup"><span data-stu-id="ae850-130">string</span></span>  | <span data-ttu-id="ae850-131">Indica o fuso horário da equipe de agendamento usando o formato de banco de dados da TZ.</span><span class="sxs-lookup"><span data-stu-id="ae850-131">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="ae850-132">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ae850-132">Required.</span></span>|
| <span data-ttu-id="ae850-133">provisionStatus</span><span class="sxs-lookup"><span data-stu-id="ae850-133">provisionStatus</span></span>       |<span data-ttu-id="ae850-134">operationStatus</span><span class="sxs-lookup"><span data-stu-id="ae850-134">operationStatus</span></span>    | <span data-ttu-id="ae850-135">O status do provisionamento de agendamento.</span><span class="sxs-lookup"><span data-stu-id="ae850-135">The status of the schedule provisioning.</span></span> <span data-ttu-id="ae850-136">Os valores possíveis são `notStarted`: `running` `completed`,, `failed`,.</span><span class="sxs-lookup"><span data-stu-id="ae850-136">The possible values are `notStarted`, `running`, `completed`, `failed`.</span></span> |
| <span data-ttu-id="ae850-137">provisionStatusCode</span><span class="sxs-lookup"><span data-stu-id="ae850-137">provisionStatusCode</span></span>   |<span data-ttu-id="ae850-138">string</span><span class="sxs-lookup"><span data-stu-id="ae850-138">string</span></span>  | <span data-ttu-id="ae850-139">Informações adicionais sobre por que o provisionamento de agendamento falhou.</span><span class="sxs-lookup"><span data-stu-id="ae850-139">Additional information about why schedule provisioning failed.</span></span> |
| <span data-ttu-id="ae850-140">timeClockEnabled</span><span class="sxs-lookup"><span data-stu-id="ae850-140">timeClockEnabled</span></span>                  |<span data-ttu-id="ae850-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="ae850-141">Boolean</span></span>  | <span data-ttu-id="ae850-142">Indica se o relógio de hora está habilitado para o cronograma.</span><span class="sxs-lookup"><span data-stu-id="ae850-142">Indicates whether time clock is enabled for the schedule.</span></span>             |
| <span data-ttu-id="ae850-143">openShiftsEnabled</span><span class="sxs-lookup"><span data-stu-id="ae850-143">openShiftsEnabled</span></span>                 |<span data-ttu-id="ae850-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="ae850-144">Boolean</span></span>  | <span data-ttu-id="ae850-145">Indica se os turnos abertos estão habilitados para o cronograma.</span><span class="sxs-lookup"><span data-stu-id="ae850-145">Indicates whether open shifts are enabled for the schedule.</span></span>             | 
| <span data-ttu-id="ae850-146">swapShiftsRequestsEnabled</span><span class="sxs-lookup"><span data-stu-id="ae850-146">swapShiftsRequestsEnabled</span></span>                 |<span data-ttu-id="ae850-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="ae850-147">Boolean</span></span>| <span data-ttu-id="ae850-148">Indica se as solicitações de troca alternadas estão habilitadas para o cronograma.</span><span class="sxs-lookup"><span data-stu-id="ae850-148">Indicates whether swap shifts requests are enabled for the schedule.</span></span>             |
| <span data-ttu-id="ae850-149">offerShiftRequestsEnabled</span><span class="sxs-lookup"><span data-stu-id="ae850-149">offerShiftRequestsEnabled</span></span>                 |<span data-ttu-id="ae850-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="ae850-150">Boolean</span></span>  | <span data-ttu-id="ae850-151">Indica se as solicitações de mudança de oferta estão habilitadas para o cronograma.</span><span class="sxs-lookup"><span data-stu-id="ae850-151">Indicates whether offer shift requests are enabled for the schedule.</span></span>             | 
| <span data-ttu-id="ae850-152">timeOffRequestsEnabled</span><span class="sxs-lookup"><span data-stu-id="ae850-152">timeOffRequestsEnabled</span></span>                    |<span data-ttu-id="ae850-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="ae850-153">Boolean</span></span> | <span data-ttu-id="ae850-154">Indica se as solicitações de folga estão habilitadas para o cronograma.</span><span class="sxs-lookup"><span data-stu-id="ae850-154">Indicates whether time off requests are enabled for the schedule.</span></span>             | 



## <a name="relationships"></a><span data-ttu-id="ae850-155">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="ae850-155">Relationships</span></span>
|<span data-ttu-id="ae850-156">Nome</span><span class="sxs-lookup"><span data-stu-id="ae850-156">Name</span></span>                   |<span data-ttu-id="ae850-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae850-157">Type</span></span>           |<span data-ttu-id="ae850-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae850-158">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ae850-159">desloca</span><span class="sxs-lookup"><span data-stu-id="ae850-159">shifts</span></span>   | <span data-ttu-id="ae850-160">coleção [Shift](shift.md)</span><span class="sxs-lookup"><span data-stu-id="ae850-160">[shift](shift.md) collection</span></span>  | <span data-ttu-id="ae850-161">Os turnos no cronograma.</span><span class="sxs-lookup"><span data-stu-id="ae850-161">The shifts in the schedule.</span></span> |
| <span data-ttu-id="ae850-162">timesOff</span><span class="sxs-lookup"><span data-stu-id="ae850-162">timesOff</span></span>   |<span data-ttu-id="ae850-163">coleção [timeOff](timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="ae850-163">[timeOff](timeoff.md) collection</span></span>  | <span data-ttu-id="ae850-164">As instâncias de folgas no cronograma.</span><span class="sxs-lookup"><span data-stu-id="ae850-164">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="ae850-165">timeOffReasons</span><span class="sxs-lookup"><span data-stu-id="ae850-165">timeOffReasons</span></span>   |<span data-ttu-id="ae850-166">coleção [timeOffReason](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="ae850-166">[timeOffReason](timeoffreason.md) collection</span></span>  | <span data-ttu-id="ae850-167">O conjunto de motivos para uma folga no cronograma.</span><span class="sxs-lookup"><span data-stu-id="ae850-167">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="ae850-168">schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="ae850-168">schedulingGroups</span></span>   |<span data-ttu-id="ae850-169">[schedulingGroup](schedulinggroup.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="ae850-169">[schedulingGroup](schedulinggroup.md) collection</span></span>  | <span data-ttu-id="ae850-170">O agrupamento lógico de usuários no cronograma (geralmente por função).</span><span class="sxs-lookup"><span data-stu-id="ae850-170">The logical grouping of users in the schedule (usually by role).</span></span> |
| <span data-ttu-id="ae850-171">openshifts</span><span class="sxs-lookup"><span data-stu-id="ae850-171">openshifts</span></span>   |<span data-ttu-id="ae850-172">coleção [openShift](openshift.md)</span><span class="sxs-lookup"><span data-stu-id="ae850-172">[openShift](openshift.md) collection</span></span> | <span data-ttu-id="ae850-173">O conjunto de turnos abertos em um grupo de agendamento no cronograma.</span><span class="sxs-lookup"><span data-stu-id="ae850-173">The set of open shifts in a scheduling group in the schedule.</span></span> |
| <span data-ttu-id="ae850-174">workforceintegrations</span><span class="sxs-lookup"><span data-stu-id="ae850-174">workforceintegrations</span></span>   |<span data-ttu-id="ae850-175">coleção [workforceIntegration](workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="ae850-175">[workforceIntegration](workforceintegration.md) collection</span></span>  | <span data-ttu-id="ae850-176">Uma instância de uma integração de força de funcionários por equipe com fluxo de dados de saída em notificações de alteração síncrona (para entidades com suporte).</span><span class="sxs-lookup"><span data-stu-id="ae850-176">An instance of a workforce integration per team with outbound data flow on synchronous change notifications (for supported entities).</span></span> |
| <span data-ttu-id="ae850-177">swapshiftchangerequests</span><span class="sxs-lookup"><span data-stu-id="ae850-177">swapshiftchangerequests</span></span>   |<span data-ttu-id="ae850-178">coleção [swapShiftsChangeRequest](swapshiftschangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="ae850-178">[swapShiftsChangeRequest](swapshiftschangerequest.md) collection</span></span>  | <span data-ttu-id="ae850-179">As solicitações de troca de turnos no cronograma.</span><span class="sxs-lookup"><span data-stu-id="ae850-179">The swap requests for shifts in the schedule.</span></span> |
| <span data-ttu-id="ae850-180">openshiftchangerequests</span><span class="sxs-lookup"><span data-stu-id="ae850-180">openshiftchangerequests</span></span>   |<span data-ttu-id="ae850-181">coleção [openShiftChangeRequest](openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="ae850-181">[openShiftChangeRequest](openshiftchangerequest.md) collection</span></span>  | <span data-ttu-id="ae850-182">As solicitações de mudança abertas no cronograma.</span><span class="sxs-lookup"><span data-stu-id="ae850-182">The open shift requests in the schedule.</span></span> |
| <span data-ttu-id="ae850-183">timeoffrequest</span><span class="sxs-lookup"><span data-stu-id="ae850-183">timeoffrequest</span></span>   |<span data-ttu-id="ae850-184">coleção [timeOffRequest](timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="ae850-184">[timeOffRequest](timeoffrequest.md) collection</span></span>  | <span data-ttu-id="ae850-185">As solicitações de folga no cronograma.</span><span class="sxs-lookup"><span data-stu-id="ae850-185">The time off requests in the schedule.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ae850-186">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae850-186">JSON representation</span></span>

<span data-ttu-id="ae850-187">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ae850-187">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.schedule"
}-->

```json
{
  "id": "833fc4df-c88b-4398-992f-d8afcfe41df2",
  "enabled": true,
  "timeZone": "America/Chicago",
  "provisionStatus": "Completed",
  "provisionStatusCode": null
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "schedule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
