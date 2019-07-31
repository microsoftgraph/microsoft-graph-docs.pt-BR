---
title: tipo de recurso Schedule
description: Uma coleção de schedulingGroups, Shifts, timeOffReasons e timesOff dentro de uma equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: a404c620b20cfcb69076ecc3bac25f907a12216c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965324"
---
# <a name="schedule-resource-type"></a><span data-ttu-id="4436b-103">tipo de recurso Schedule</span><span class="sxs-lookup"><span data-stu-id="4436b-103">schedule resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4436b-104">Uma coleção de objetos de grupo de [agendamento](schedulinggroup.md) , objetos [Shift](shift.md) , objetos [timeOffReason](timeoffreason.md) e objetos [timeOff](timeoff.md) dentro de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="4436b-104">A collection of [schedulingGroup](schedulinggroup.md) objects, [shift](shift.md) objects, [timeOffReason](timeoffreason.md) objects, and [timeOff](timeoff.md) objects within a [team](../resources/team.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="4436b-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="4436b-105">Methods</span></span>

| <span data-ttu-id="4436b-106">Método</span><span class="sxs-lookup"><span data-stu-id="4436b-106">Method</span></span>       | <span data-ttu-id="4436b-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4436b-107">Return Type</span></span>  |<span data-ttu-id="4436b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="4436b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4436b-109">Criar ou substituir agendamento</span><span class="sxs-lookup"><span data-stu-id="4436b-109">Create or replace schedule</span></span>](../api/team-put-schedule.md) | [<span data-ttu-id="4436b-110">Cronograma</span><span class="sxs-lookup"><span data-stu-id="4436b-110">schedule</span></span>](schedule.md) | <span data-ttu-id="4436b-111">Criar ou substituir um `schedule`.</span><span class="sxs-lookup"><span data-stu-id="4436b-111">Create or replace a `schedule`.</span></span>|
|[<span data-ttu-id="4436b-112">Obter cronograma</span><span class="sxs-lookup"><span data-stu-id="4436b-112">Get schedule</span></span>](../api/schedule-get.md) | [<span data-ttu-id="4436b-113">Cronograma</span><span class="sxs-lookup"><span data-stu-id="4436b-113">schedule</span></span>](schedule.md) | <span data-ttu-id="4436b-114">Obter um `schedule`.</span><span class="sxs-lookup"><span data-stu-id="4436b-114">Get a `schedule`.</span></span>|
|[<span data-ttu-id="4436b-115">share</span><span class="sxs-lookup"><span data-stu-id="4436b-115">share</span></span>](../api/schedule-share.md) | <span data-ttu-id="4436b-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4436b-116">None</span></span> | <span data-ttu-id="4436b-117">Compartilhar um `schedule` intervalo de tempo com membros de agendamento.</span><span class="sxs-lookup"><span data-stu-id="4436b-117">Share a `schedule` time range with schedule members.</span></span>|

## <a name="properties"></a><span data-ttu-id="4436b-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4436b-118">Properties</span></span>
|<span data-ttu-id="4436b-119">Nome</span><span class="sxs-lookup"><span data-stu-id="4436b-119">Name</span></span>                   |<span data-ttu-id="4436b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="4436b-120">Type</span></span>           |<span data-ttu-id="4436b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="4436b-121">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4436b-122">id</span><span class="sxs-lookup"><span data-stu-id="4436b-122">id</span></span>                    |`string`  |<span data-ttu-id="4436b-123">A ID da tarefa `schedule`.</span><span class="sxs-lookup"><span data-stu-id="4436b-123">ID of the `schedule`.</span></span>|
| <span data-ttu-id="4436b-124">enabled</span><span class="sxs-lookup"><span data-stu-id="4436b-124">enabled</span></span>               |`bool`    | <span data-ttu-id="4436b-125">Indica se o cronograma está habilitado para a equipe.</span><span class="sxs-lookup"><span data-stu-id="4436b-125">Indicates whether the schedule is enabled for the team.</span></span> <span data-ttu-id="4436b-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4436b-126">Required.</span></span>|
| <span data-ttu-id="4436b-127">timeZone</span><span class="sxs-lookup"><span data-stu-id="4436b-127">timeZone</span></span>              |`string`  | <span data-ttu-id="4436b-128">Indica o fuso horário da equipe de agendamento usando o formato de banco de dados da TZ.</span><span class="sxs-lookup"><span data-stu-id="4436b-128">Indicates the time zone of the schedule team using tz database format.</span></span> <span data-ttu-id="4436b-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4436b-129">Required.</span></span>|
| <span data-ttu-id="4436b-130">provisionStatus</span><span class="sxs-lookup"><span data-stu-id="4436b-130">provisionStatus</span></span>       |`operationStatus`    | <span data-ttu-id="4436b-131">O status do provisionamento de agendamento.</span><span class="sxs-lookup"><span data-stu-id="4436b-131">The status of the schedule provisioning.</span></span> <span data-ttu-id="4436b-132">Os valores possíveis são `notStarted`: `running` `completed`,, `failed`,.</span><span class="sxs-lookup"><span data-stu-id="4436b-132">The possible values are `notStarted`, `running`, `completed`, `failed`.</span></span> |
| <span data-ttu-id="4436b-133">provisionStatusCode</span><span class="sxs-lookup"><span data-stu-id="4436b-133">provisionStatusCode</span></span>   |`string`  | <span data-ttu-id="4436b-134">Informações adicionais sobre por que o provisionamento de agendamento falhou.</span><span class="sxs-lookup"><span data-stu-id="4436b-134">Additional information about why schedule provisioning failed.</span></span> |


## <a name="relationships"></a><span data-ttu-id="4436b-135">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="4436b-135">Relationships</span></span>
|<span data-ttu-id="4436b-136">Nome</span><span class="sxs-lookup"><span data-stu-id="4436b-136">Name</span></span>                   |<span data-ttu-id="4436b-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="4436b-137">Type</span></span>           |<span data-ttu-id="4436b-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="4436b-138">Description</span></span>                                                                                                                                      |
|-----------------------|---------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4436b-139">desloca</span><span class="sxs-lookup"><span data-stu-id="4436b-139">shifts</span></span>   |`collection(shift)`  | <span data-ttu-id="4436b-140">Os turnos no cronograma.</span><span class="sxs-lookup"><span data-stu-id="4436b-140">The shifts in the schedule.</span></span> |
| <span data-ttu-id="4436b-141">timesOff</span><span class="sxs-lookup"><span data-stu-id="4436b-141">timesOff</span></span>   |`collection(timeOff)`  | <span data-ttu-id="4436b-142">As instâncias de folgas no cronograma.</span><span class="sxs-lookup"><span data-stu-id="4436b-142">The instances of times off in the schedule.</span></span> |
| <span data-ttu-id="4436b-143">timeOffReasons</span><span class="sxs-lookup"><span data-stu-id="4436b-143">timeOffReasons</span></span>   |`collection(timeOffReason)`  | <span data-ttu-id="4436b-144">O conjunto de motivos para uma folga no cronograma.</span><span class="sxs-lookup"><span data-stu-id="4436b-144">The set of reasons for a time off in the schedule.</span></span> |
| <span data-ttu-id="4436b-145">schedulingGroups</span><span class="sxs-lookup"><span data-stu-id="4436b-145">schedulingGroups</span></span>   |`collection(schedulingGroup)`  | <span data-ttu-id="4436b-146">O agrupamento lógico de usuários no cronograma (geralmente por função).</span><span class="sxs-lookup"><span data-stu-id="4436b-146">The logical grouping of users in the schedule (usually by role).</span></span> |


## <a name="json-representation"></a><span data-ttu-id="4436b-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4436b-147">JSON representation</span></span>

<span data-ttu-id="4436b-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4436b-148">Here is a JSON representation of the resource.</span></span>

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
