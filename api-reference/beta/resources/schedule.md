---
title: tipo de recurso Schedule
description: Uma coleção de schedulingGroups, Shifts, timeOffReasons e timesOff dentro de uma equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: de3662fcf3c5a8e50493e365f6a10a8641a451df
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563093"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="c1727-103">tipo de recurso Schedule</span><span class="sxs-lookup"><span data-stu-id="c1727-103">schedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1727-104">Uma coleção de objetos de grupo de [agendamento](schedulinggroup.md) , objetos [Shift](shift.md) , objetos [timeOffReason](timeoffreason.md) e objetos [timeOff](timeoff.md) dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="c1727-104">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="c1727-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="c1727-105">Methods</span></span>

| <span data-ttu-id="c1727-106">Método</span><span class="sxs-lookup"><span data-stu-id="c1727-106">Method</span></span>       | <span data-ttu-id="c1727-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c1727-107">Return Type</span></span>  |<span data-ttu-id="c1727-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1727-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c1727-109">Criar ou substituir agendamento</span><span class="sxs-lookup"><span data-stu-id="c1727-109">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="c1727-110">futebol</span><span class="sxs-lookup"><span data-stu-id="c1727-110">schedule</span></span>](schedule.md) | <span data-ttu-id="c1727-111">Criar ou substituir um `schedule`.</span><span class="sxs-lookup"><span data-stu-id="c1727-111">Create or replace a `schedule`.</span></span>|
|[<span data-ttu-id="c1727-112">Obter cronograma</span><span class="sxs-lookup"><span data-stu-id="c1727-112">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="c1727-113">futebol</span><span class="sxs-lookup"><span data-stu-id="c1727-113">schedule</span></span>](schedule.md) | <span data-ttu-id="c1727-114">Obter um `schedule`.</span><span class="sxs-lookup"><span data-stu-id="c1727-114">Get a `schedule`.</span></span>|
|[<span data-ttu-id="c1727-115">share</span><span class="sxs-lookup"><span data-stu-id="c1727-115">share</span></span>](../api/schedule-share.md) | <span data-ttu-id="c1727-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c1727-116">None</span></span> | <span data-ttu-id="c1727-117">Compartilhar um `schedule` intervalo de tempo com membros de agendamento.</span><span class="sxs-lookup"><span data-stu-id="c1727-117">Share a `schedule` time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="c1727-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1727-118">Properties</span></span>
|<span data-ttu-id="c1727-119">Nome</span><span class="sxs-lookup"><span data-stu-id="c1727-119">Name</span></span>                   |<span data-ttu-id="c1727-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1727-120">Type</span></span>           |<span data-ttu-id="c1727-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1727-121">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c1727-122">id</span><span class="sxs-lookup"><span data-stu-id="c1727-122">id</span></span>                    |`string`  |<span data-ttu-id="c1727-123">A ID da tarefa `schedule`.</span><span class="sxs-lookup"><span data-stu-id="c1727-123">ID of the `schedule`.</span></span>|
| <span data-ttu-id="c1727-124">enabled</span><span class="sxs-lookup"><span data-stu-id="c1727-124">enabled</span></span>               |`bool`    | <span data-ttu-id="c1727-125">Indica se o cronograma está habilitado para a equipe.</span><span class="sxs-lookup"><span data-stu-id="c1727-125">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="c1727-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1727-126">Required.</span></span>|
| <span data-ttu-id="c1727-127">timeZone</span><span class="sxs-lookup"><span data-stu-id="c1727-127">timeZone</span></span>              |`string`  | <span data-ttu-id="c1727-128">Indica o fuso horário da equipe de agendamento usando o formato de banco de dados da TZ.</span><span class="sxs-lookup"><span data-stu-id="c1727-128">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="c1727-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c1727-129">Required.</span></span>|
| <span data-ttu-id="c1727-130">provisionStatus</span><span class="sxs-lookup"><span data-stu-id="c1727-130">provisionStatus</span></span>       |`enum`    | <span data-ttu-id="c1727-131">O status do provisionamento de agendamento.</span><span class="sxs-lookup"><span data-stu-id="c1727-131">The status of the schedule provisioning.</span></span> |
| <span data-ttu-id="c1727-132">provisionStatusCode</span><span class="sxs-lookup"><span data-stu-id="c1727-132">provisionStatusCode</span></span>   |`string`  | <span data-ttu-id="c1727-133">Informações adicionais sobre por que o provisionamento de agendamento falhou.</span><span class="sxs-lookup"><span data-stu-id="c1727-133">Additional information about why schedule provisioning failed.</span></span> |


## <a name="relationships"></a><span data-ttu-id="c1727-134">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="c1727-134">Relationships</span></span>
|<span data-ttu-id="c1727-135">Nome</span><span class="sxs-lookup"><span data-stu-id="c1727-135">Name</span></span>                   |<span data-ttu-id="c1727-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1727-136">Type</span></span>           |<span data-ttu-id="c1727-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1727-137">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="c1727-138">desloca</span><span class="sxs-lookup"><span data-stu-id="c1727-138">shifts</span></span>   |`collection(shift)`  | <span data-ttu-id="c1727-139">Os turnos no cronograma.</span><span class="sxs-lookup"><span data-stu-id="c1727-139">The shifts in the schedule.</span></span> |
| <span data-ttu-id="c1727-140">timesOff</span><span class="sxs-lookup"><span data-stu-id="c1727-140">timesOff</span></span>   |`collection(timeOff)`  | <span data-ttu-id="c1727-141">As instâncias de folgas no cronograma.</span><span class="sxs-lookup"><span data-stu-id="c1727-141">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="c1727-142">timeOffReasons</span><span class="sxs-lookup"><span data-stu-id="c1727-142">timeOffReasons</span></span>   |`collection(timeOffReason)`  | <span data-ttu-id="c1727-143">O conjunto de motivos para uma folga no cronograma.</span><span class="sxs-lookup"><span data-stu-id="c1727-143">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="c1727-144">schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="c1727-144">schedulingGroups</span></span>   |`collection(schedulingGroup)`  | <span data-ttu-id="c1727-145">O agrupamento lógico de usuários no cronograma (geralmente por função).</span><span class="sxs-lookup"><span data-stu-id="c1727-145">The logical grouping of users in the schedule (usually by role).</span></span> |


## <a name="json-representation"></a><span data-ttu-id="c1727-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1727-146">JSON representation</span></span>

<span data-ttu-id="c1727-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1727-147">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/schedule.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
