---
title: tipo de recurso meetingActivityStatistics
description: Representa informações sobre as atividades de reunião para os usuários.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 14d926a41680f1292b7599bd76b458705b426719
ms.sourcegitcommit: 83a053067f6248fb49ec5d473738ab1555fb4295
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/24/2019
ms.locfileid: "36622534"
---
# <a name="meetingactivitystatistics-resource-type"></a><span data-ttu-id="74697-103">tipo de recurso meetingActivityStatistics</span><span class="sxs-lookup"><span data-stu-id="74697-103">meetingActivityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74697-104">Representa dados sobre o tempo gasto pelo usuário em reuniões no Microsoft Outlook, Microsoft Teams ou Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="74697-104">Represents data about the user's time spent in meetings in Microsoft Outlook, Microsoft Teams, or Skype for Business.</span></span> <span data-ttu-id="74697-105">Isso é baseado no [activityStatistics](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="74697-105">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>
<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get meetingActivityStatistics](../api/meetingactivitystatistics-get.md) | [meetingActivityStatistics](meetingactivitystatistics.md) | Read properties and relationships of meetingActivityStatistics object; name of the activity for which statistics are returned as “meeting.” |
-->
## <a name="properties"></a><span data-ttu-id="74697-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74697-106">Properties</span></span>

| <span data-ttu-id="74697-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74697-107">Property</span></span>     | <span data-ttu-id="74697-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="74697-108">Type</span></span>        | <span data-ttu-id="74697-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="74697-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="74697-110">atividade</span><span class="sxs-lookup"><span data-stu-id="74697-110">activity</span></span>|<span data-ttu-id="74697-111">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="74697-111">analyticsActivityType</span></span>| <span data-ttu-id="74697-112">Atividade de reunião para a qual as estatísticas são retornadas.</span><span class="sxs-lookup"><span data-stu-id="74697-112">Meeting activity for which statistics are returned.</span></span>|
|<span data-ttu-id="74697-113">duration</span><span class="sxs-lookup"><span data-stu-id="74697-113">duration</span></span>|<span data-ttu-id="74697-114">Duração</span><span class="sxs-lookup"><span data-stu-id="74697-114">Duration</span></span>|<span data-ttu-id="74697-115">Total de horas gasto em reuniões.</span><span class="sxs-lookup"><span data-stu-id="74697-115">Total hours spent on meetings.</span></span> <span data-ttu-id="74697-116">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="74697-116">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="74697-117">endDate</span><span class="sxs-lookup"><span data-stu-id="74697-117">endDate</span></span>|<span data-ttu-id="74697-118">Data</span><span class="sxs-lookup"><span data-stu-id="74697-118">Date</span></span>|<span data-ttu-id="74697-119">Data de término da atividade da reunião.</span><span class="sxs-lookup"><span data-stu-id="74697-119">Date when the meeting activity ended.</span></span> <span data-ttu-id="74697-120">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="74697-120">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="74697-121">Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="74697-121">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="74697-122">id</span><span class="sxs-lookup"><span data-stu-id="74697-122">id</span></span>|<span data-ttu-id="74697-123">String</span><span class="sxs-lookup"><span data-stu-id="74697-123">String</span></span>| <span data-ttu-id="74697-124">ID somente leitura da atividade da reunião.</span><span class="sxs-lookup"><span data-stu-id="74697-124">Read-only ID for the meeting activity.</span></span>|
|<span data-ttu-id="74697-125">startDate</span><span class="sxs-lookup"><span data-stu-id="74697-125">startDate</span></span>|<span data-ttu-id="74697-126">Date</span><span class="sxs-lookup"><span data-stu-id="74697-126">Date</span></span>|<span data-ttu-id="74697-127">Data de início da atividade da reunião.</span><span class="sxs-lookup"><span data-stu-id="74697-127">Date when the meeting activity started.</span></span> <span data-ttu-id="74697-128">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="74697-128">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="74697-129">Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="74697-129">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="74697-130">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="74697-130">timeZoneUsed</span></span>|<span data-ttu-id="74697-131">String</span><span class="sxs-lookup"><span data-stu-id="74697-131">String</span></span>|<span data-ttu-id="74697-132">O fuso horário do Outlook definido pelo usuário no calendário do Outlook é usado para a computação.</span><span class="sxs-lookup"><span data-stu-id="74697-132">The Outlook time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="74697-133">Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="74697-133">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="74697-134">afterHours</span><span class="sxs-lookup"><span data-stu-id="74697-134">afterHours</span></span>|<span data-ttu-id="74697-135">Duração</span><span class="sxs-lookup"><span data-stu-id="74697-135">Duration</span></span>|<span data-ttu-id="74697-136">Tempo gasto em reuniões fora do horário de trabalho, que se baseia na configuração de calendário do Outlook do usuário para horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="74697-136">Time spent on meetings outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="74697-137">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="74697-137">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="74697-138">conflitantes</span><span class="sxs-lookup"><span data-stu-id="74697-138">conflicting</span></span>|<span data-ttu-id="74697-139">Duração</span><span class="sxs-lookup"><span data-stu-id="74697-139">Duration</span></span>|<span data-ttu-id="74697-140">Tempo gasto em reuniões conflitantes (reuniões que se sobrepõem a outras reuniões que a pessoa aceitou e onde o status da pessoa está definido como ocupado).</span><span class="sxs-lookup"><span data-stu-id="74697-140">Time spent in conflicting meetings (meetings that overlap with other meetings that the person accepted and where the person’s status is set to Busy).</span></span> <span data-ttu-id="74697-141">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="74697-141">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="74697-142">long</span><span class="sxs-lookup"><span data-stu-id="74697-142">long</span></span>|<span data-ttu-id="74697-143">Duração</span><span class="sxs-lookup"><span data-stu-id="74697-143">Duration</span></span>|<span data-ttu-id="74697-144">Tempo gasto em reuniões longas (mais de uma hora em duração).</span><span class="sxs-lookup"><span data-stu-id="74697-144">Time spent in long meetings (more than an hour in duration).</span></span> <span data-ttu-id="74697-145">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="74697-145">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="74697-146">multitarefas</span><span class="sxs-lookup"><span data-stu-id="74697-146">multitasking</span></span>|<span data-ttu-id="74697-147">Duração</span><span class="sxs-lookup"><span data-stu-id="74697-147">Duration</span></span>|<span data-ttu-id="74697-148">Tempo gasto em reuniões em que a pessoa estava multitarefa (leitura/envio de mais de um número mínimo de emails e/ou envio de mais de um número mínimo de mensagens no Microsoft Teams ou no Skype for Business).</span><span class="sxs-lookup"><span data-stu-id="74697-148">Time spent in meetings where the person was multitasking (read/sent more than a minimum number of emails and/or sent more than a minimum number of messages in Teams or in Skype for Business).</span></span> <span data-ttu-id="74697-149">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="74697-149">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="74697-150">organiza</span><span class="sxs-lookup"><span data-stu-id="74697-150">organized</span></span>|<span data-ttu-id="74697-151">Duração</span><span class="sxs-lookup"><span data-stu-id="74697-151">Duration</span></span>|<span data-ttu-id="74697-152">Tempo gasto em reuniões organizadas pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="74697-152">Time spent in meetings organized by the user.</span></span> <span data-ttu-id="74697-153">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="74697-153">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="74697-154">recorrente</span><span class="sxs-lookup"><span data-stu-id="74697-154">recurring</span></span>|<span data-ttu-id="74697-155">Duração</span><span class="sxs-lookup"><span data-stu-id="74697-155">Duration</span></span>|<span data-ttu-id="74697-156">Tempo gasto em reuniões recorrentes.</span><span class="sxs-lookup"><span data-stu-id="74697-156">Time spent on recurring meetings.</span></span> <span data-ttu-id="74697-157">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="74697-157">The value is represented in ISO 8601 format for durations.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74697-158">Relações</span><span class="sxs-lookup"><span data-stu-id="74697-158">Relationships</span></span>

<span data-ttu-id="74697-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74697-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74697-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74697-160">JSON representation</span></span>

<span data-ttu-id="74697-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74697-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.activityStatistics",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingActivityStatistics"
}--> 

```json
{
  "activity": "string",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601)",
  "timeZoneUsed": "String",
  "afterHours": "String (ISO 8601 duration)",
  "conflicting": "String (ISO 8601 duration)",
  "long": "String (ISO 8601 duration)",
  "multitasking": "String (ISO 8601 duration)",
  "organized": "String (ISO 8601 duration)",
  "recurring": "String (ISO 8601 duration)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingActivityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->