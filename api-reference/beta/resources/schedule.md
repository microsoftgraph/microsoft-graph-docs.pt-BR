---
title: tipo de recurso Schedule
description: Uma coleção de schedulingGroups, Shifts, timeOffReasons e timesOff dentro de uma equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2fb40dc62e2a8c583c9e3c4f29ad4d9905acb6d6
ms.sourcegitcommit: 02c16375520853d3fa2a82ff012639550f981fc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2020
ms.locfileid: "44154133"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="17888-103">tipo de recurso Schedule</span><span class="sxs-lookup"><span data-stu-id="17888-103">schedule resource type</span></span>

<span data-ttu-id="17888-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17888-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17888-105">Uma coleção de objetos de grupo de [agendamento](schedulinggroup.md) , objetos [Shift](shift.md) , objetos [timeOffReason](timeoffreason.md) e objetos [timeOff](timeoff.md) dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="17888-105">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="17888-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="17888-106">Methods</span></span>

| <span data-ttu-id="17888-107">Método</span><span class="sxs-lookup"><span data-stu-id="17888-107">Method</span></span>       | <span data-ttu-id="17888-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="17888-108">Return Type</span></span>  |<span data-ttu-id="17888-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="17888-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="17888-110">Criar ou substituir agendamento</span><span class="sxs-lookup"><span data-stu-id="17888-110">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="17888-111">Cronograma</span><span class="sxs-lookup"><span data-stu-id="17888-111">schedule</span></span>](schedule.md) | <span data-ttu-id="17888-112">Criar ou substituir uma agenda.</span><span class="sxs-lookup"><span data-stu-id="17888-112">Create or replace a schedule.</span></span>|
|[<span data-ttu-id="17888-113">Obter cronograma</span><span class="sxs-lookup"><span data-stu-id="17888-113">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="17888-114">Cronograma</span><span class="sxs-lookup"><span data-stu-id="17888-114">schedule</span></span>](schedule.md) | <span data-ttu-id="17888-115">Obter um cronograma.</span><span class="sxs-lookup"><span data-stu-id="17888-115">Get a schedule.</span></span>|
|[<span data-ttu-id="17888-116">Compartilhar</span><span class="sxs-lookup"><span data-stu-id="17888-116">Share</span></span>](../api/schedule-share.md) | <span data-ttu-id="17888-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="17888-117">None</span></span> | <span data-ttu-id="17888-118">Compartilhar um intervalo de tempo de agendamento com membros de agendamento.</span><span class="sxs-lookup"><span data-stu-id="17888-118">Share a schedule time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="17888-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="17888-119">Properties</span></span>
|<span data-ttu-id="17888-120">Nome</span><span class="sxs-lookup"><span data-stu-id="17888-120">Name</span></span>                   |<span data-ttu-id="17888-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="17888-121">Type</span></span>           |<span data-ttu-id="17888-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="17888-122">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="17888-123">id</span><span class="sxs-lookup"><span data-stu-id="17888-123">id</span></span>                    |<span data-ttu-id="17888-124">string</span><span class="sxs-lookup"><span data-stu-id="17888-124">string</span></span>  |<span data-ttu-id="17888-125">ID do cronograma.</span><span class="sxs-lookup"><span data-stu-id="17888-125">ID of the schedule.</span></span>|
| <span data-ttu-id="17888-126">enabled</span><span class="sxs-lookup"><span data-stu-id="17888-126">enabled</span></span>               |<span data-ttu-id="17888-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="17888-127">Boolean</span></span>    | <span data-ttu-id="17888-128">Indica se o cronograma está habilitado para a equipe.</span><span class="sxs-lookup"><span data-stu-id="17888-128">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="17888-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17888-129">Required.</span></span>|
| <span data-ttu-id="17888-130">timeZone</span><span class="sxs-lookup"><span data-stu-id="17888-130">timeZone</span></span>              |<span data-ttu-id="17888-131">string</span><span class="sxs-lookup"><span data-stu-id="17888-131">string</span></span>  | <span data-ttu-id="17888-132">Indica o fuso horário da equipe de agendamento usando o formato de banco de dados da TZ.</span><span class="sxs-lookup"><span data-stu-id="17888-132">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="17888-133">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="17888-133">Required.</span></span>|
| <span data-ttu-id="17888-134">provisionStatus</span><span class="sxs-lookup"><span data-stu-id="17888-134">provisionStatus</span></span>       |<span data-ttu-id="17888-135">operationStatus</span><span class="sxs-lookup"><span data-stu-id="17888-135">operationStatus</span></span>    | <span data-ttu-id="17888-136">O status do provisionamento de agendamento.</span><span class="sxs-lookup"><span data-stu-id="17888-136">The status of the schedule provisioning.</span></span> <span data-ttu-id="17888-137">Os valores possíveis são `notStarted`: `running` `completed`,, `failed`,.</span><span class="sxs-lookup"><span data-stu-id="17888-137">The possible values are `notStarted`, `running`, `completed`, `failed`.</span></span> |
| <span data-ttu-id="17888-138">provisionStatusCode</span><span class="sxs-lookup"><span data-stu-id="17888-138">provisionStatusCode</span></span>   |<span data-ttu-id="17888-139">string</span><span class="sxs-lookup"><span data-stu-id="17888-139">string</span></span>  | <span data-ttu-id="17888-140">Informações adicionais sobre por que o provisionamento de agendamento falhou.</span><span class="sxs-lookup"><span data-stu-id="17888-140">Additional information about why schedule provisioning failed.</span></span> |
| <span data-ttu-id="17888-141">timeClockEnabled</span><span class="sxs-lookup"><span data-stu-id="17888-141">timeClockEnabled</span></span>                  |<span data-ttu-id="17888-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="17888-142">Boolean</span></span>  | <span data-ttu-id="17888-143">Indica se o relógio de hora está habilitado para o cronograma.</span><span class="sxs-lookup"><span data-stu-id="17888-143">Indicates whether time clock is enabled for the schedule.</span></span>             |
| <span data-ttu-id="17888-144">openShiftsEnabled</span><span class="sxs-lookup"><span data-stu-id="17888-144">openShiftsEnabled</span></span>                 |<span data-ttu-id="17888-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="17888-145">Boolean</span></span>  | <span data-ttu-id="17888-146">Indica se os turnos abertos estão habilitados para o cronograma.</span><span class="sxs-lookup"><span data-stu-id="17888-146">Indicates whether open shifts are enabled for the schedule.</span></span>             | 
| <span data-ttu-id="17888-147">swapShiftsRequestsEnabled</span><span class="sxs-lookup"><span data-stu-id="17888-147">swapShiftsRequestsEnabled</span></span>                 |<span data-ttu-id="17888-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="17888-148">Boolean</span></span>| <span data-ttu-id="17888-149">Indica se as solicitações de troca alternadas estão habilitadas para o cronograma.</span><span class="sxs-lookup"><span data-stu-id="17888-149">Indicates whether swap shifts requests are enabled for the schedule.</span></span>             |
| <span data-ttu-id="17888-150">offerShiftRequestsEnabled</span><span class="sxs-lookup"><span data-stu-id="17888-150">offerShiftRequestsEnabled</span></span>                 |<span data-ttu-id="17888-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="17888-151">Boolean</span></span>  | <span data-ttu-id="17888-152">Indica se as solicitações de mudança de oferta estão habilitadas para o cronograma.</span><span class="sxs-lookup"><span data-stu-id="17888-152">Indicates whether offer shift requests are enabled for the schedule.</span></span>             | 
| <span data-ttu-id="17888-153">timeOffRequestsEnabled</span><span class="sxs-lookup"><span data-stu-id="17888-153">timeOffRequestsEnabled</span></span>                    |<span data-ttu-id="17888-154">Booliano</span><span class="sxs-lookup"><span data-stu-id="17888-154">Boolean</span></span> | <span data-ttu-id="17888-155">Indica se as solicitações de folga estão habilitadas para o cronograma.</span><span class="sxs-lookup"><span data-stu-id="17888-155">Indicates whether time off requests are enabled for the schedule.</span></span>             | 



## <a name="relationships"></a><span data-ttu-id="17888-156">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="17888-156">Relationships</span></span>
|<span data-ttu-id="17888-157">Nome</span><span class="sxs-lookup"><span data-stu-id="17888-157">Name</span></span>                   |<span data-ttu-id="17888-158">Tipo</span><span class="sxs-lookup"><span data-stu-id="17888-158">Type</span></span>           |<span data-ttu-id="17888-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="17888-159">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="17888-160">desloca</span><span class="sxs-lookup"><span data-stu-id="17888-160">shifts</span></span>   | <span data-ttu-id="17888-161">coleção [Shift](shift.md)</span><span class="sxs-lookup"><span data-stu-id="17888-161">[shift](shift.md) collection</span></span>  | <span data-ttu-id="17888-162">Os turnos no cronograma.</span><span class="sxs-lookup"><span data-stu-id="17888-162">The shifts in the schedule.</span></span> |
| <span data-ttu-id="17888-163">timesOff</span><span class="sxs-lookup"><span data-stu-id="17888-163">timesOff</span></span>   |<span data-ttu-id="17888-164">coleção [timeOff](timeoff.md)</span><span class="sxs-lookup"><span data-stu-id="17888-164">[timeOff](timeoff.md) collection</span></span>  | <span data-ttu-id="17888-165">As instâncias de folgas no cronograma.</span><span class="sxs-lookup"><span data-stu-id="17888-165">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="17888-166">timeOffReasons</span><span class="sxs-lookup"><span data-stu-id="17888-166">timeOffReasons</span></span>   |<span data-ttu-id="17888-167">coleção [timeOffReason](timeoffreason.md)</span><span class="sxs-lookup"><span data-stu-id="17888-167">[timeOffReason](timeoffreason.md) collection</span></span>  | <span data-ttu-id="17888-168">O conjunto de motivos para uma folga no cronograma.</span><span class="sxs-lookup"><span data-stu-id="17888-168">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="17888-169">schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="17888-169">schedulingGroups</span></span>   |<span data-ttu-id="17888-170">[schedulingGroup](schedulinggroup.md) conjunto</span><span class="sxs-lookup"><span data-stu-id="17888-170">[schedulingGroup](schedulinggroup.md) collection</span></span>  | <span data-ttu-id="17888-171">O agrupamento lógico de usuários no cronograma (geralmente por função).</span><span class="sxs-lookup"><span data-stu-id="17888-171">The logical grouping of users in the schedule (usually by role).</span></span> |
| <span data-ttu-id="17888-172">openshifts</span><span class="sxs-lookup"><span data-stu-id="17888-172">openshifts</span></span>   |<span data-ttu-id="17888-173">coleção [openShift](openshift.md)</span><span class="sxs-lookup"><span data-stu-id="17888-173">[openShift](openshift.md) collection</span></span> | <span data-ttu-id="17888-174">O conjunto de turnos abertos em um grupo de agendamento no cronograma.</span><span class="sxs-lookup"><span data-stu-id="17888-174">The set of open shifts in a scheduling group in the schedule.</span></span> |
| <span data-ttu-id="17888-175">workforceintegrations</span><span class="sxs-lookup"><span data-stu-id="17888-175">workforceintegrations</span></span>   |<span data-ttu-id="17888-176">coleção [workforceIntegration](workforceintegration.md)</span><span class="sxs-lookup"><span data-stu-id="17888-176">[workforceIntegration](workforceintegration.md) collection</span></span>  | <span data-ttu-id="17888-177">Uma instância de uma integração de força de funcionários por equipe com fluxo de dados de saída em notificações de alteração síncrona (para entidades com suporte).</span><span class="sxs-lookup"><span data-stu-id="17888-177">An instance of a workforce integration per team with outbound data flow on synchronous change notifications (for supported entities).</span></span> |
| <span data-ttu-id="17888-178">swapshiftchangerequests</span><span class="sxs-lookup"><span data-stu-id="17888-178">swapshiftchangerequests</span></span>   |<span data-ttu-id="17888-179">coleção [swapShiftsChangeRequest](swapshiftschangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="17888-179">[swapShiftsChangeRequest](swapshiftschangerequest.md) collection</span></span>  | <span data-ttu-id="17888-180">As solicitações de troca de turnos no cronograma.</span><span class="sxs-lookup"><span data-stu-id="17888-180">The swap requests for shifts in the schedule.</span></span> |
| <span data-ttu-id="17888-181">openshiftchangerequests</span><span class="sxs-lookup"><span data-stu-id="17888-181">openshiftchangerequests</span></span>   |<span data-ttu-id="17888-182">coleção [openShiftChangeRequest](openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="17888-182">[openShiftChangeRequest](openshiftchangerequest.md) collection</span></span>  | <span data-ttu-id="17888-183">As solicitações de mudança abertas no cronograma.</span><span class="sxs-lookup"><span data-stu-id="17888-183">The open shift requests in the schedule.</span></span> |
| <span data-ttu-id="17888-184">timeoffrequest</span><span class="sxs-lookup"><span data-stu-id="17888-184">timeoffrequest</span></span>   |<span data-ttu-id="17888-185">coleção [timeOffRequest](timeoffrequest.md)</span><span class="sxs-lookup"><span data-stu-id="17888-185">[timeOffRequest](timeoffrequest.md) collection</span></span>  | <span data-ttu-id="17888-186">As solicitações de folga no cronograma.</span><span class="sxs-lookup"><span data-stu-id="17888-186">The time off requests in the schedule.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="17888-187">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17888-187">JSON representation</span></span>

<span data-ttu-id="17888-188">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="17888-188">The following is a JSON representation of the resource.</span></span>

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
