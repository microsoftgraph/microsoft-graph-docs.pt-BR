---
title: tipo de recurso meetingActivityStatistics
description: Representa informações sobre as atividades de reunião para os usuários.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 039d2be82a08057c9f9a5405d3591898304a8bcc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522747"
---
# <a name="meetingactivitystatistics-resource-type"></a><span data-ttu-id="bef60-103">tipo de recurso meetingActivityStatistics</span><span class="sxs-lookup"><span data-stu-id="bef60-103">meetingActivityStatistics resource type</span></span>

<span data-ttu-id="bef60-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bef60-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bef60-105">Representa dados sobre o tempo gasto pelo usuário em reuniões no Microsoft Outlook, Microsoft Teams ou Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="bef60-105">Represents data about the user's time spent in meetings in Microsoft Outlook, Microsoft Teams, or Skype for Business.</span></span> <span data-ttu-id="bef60-106">Isso é baseado no [activityStatistics](../resources/activitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="bef60-106">This is based on [activityStatistics](../resources/activitystatistics.md).</span></span>
<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get meetingActivityStatistics](../api/meetingactivitystatistics-get.md) | [meetingActivityStatistics](meetingactivitystatistics.md) | Read properties and relationships of meetingActivityStatistics object; name of the activity for which statistics are returned as “meeting.” |
-->
## <a name="properties"></a><span data-ttu-id="bef60-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bef60-107">Properties</span></span>

| <span data-ttu-id="bef60-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bef60-108">Property</span></span>     | <span data-ttu-id="bef60-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bef60-109">Type</span></span>        | <span data-ttu-id="bef60-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bef60-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bef60-111">atividade</span><span class="sxs-lookup"><span data-stu-id="bef60-111">activity</span></span>|<span data-ttu-id="bef60-112">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="bef60-112">analyticsActivityType</span></span>| <span data-ttu-id="bef60-113">Atividade de reunião para a qual as estatísticas são retornadas.</span><span class="sxs-lookup"><span data-stu-id="bef60-113">Meeting activity for which statistics are returned.</span></span>|
|<span data-ttu-id="bef60-114">duration</span><span class="sxs-lookup"><span data-stu-id="bef60-114">duration</span></span>|<span data-ttu-id="bef60-115">Duração</span><span class="sxs-lookup"><span data-stu-id="bef60-115">Duration</span></span>|<span data-ttu-id="bef60-116">Total de horas gasto em reuniões.</span><span class="sxs-lookup"><span data-stu-id="bef60-116">Total hours spent on meetings.</span></span> <span data-ttu-id="bef60-117">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="bef60-117">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="bef60-118">endDate</span><span class="sxs-lookup"><span data-stu-id="bef60-118">endDate</span></span>|<span data-ttu-id="bef60-119">Data</span><span class="sxs-lookup"><span data-stu-id="bef60-119">Date</span></span>|<span data-ttu-id="bef60-120">Data de término da atividade da reunião.</span><span class="sxs-lookup"><span data-stu-id="bef60-120">Date when the meeting activity ended.</span></span> <span data-ttu-id="bef60-121">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="bef60-121">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="bef60-122">Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="bef60-122">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="bef60-123">id</span><span class="sxs-lookup"><span data-stu-id="bef60-123">id</span></span>|<span data-ttu-id="bef60-124">String</span><span class="sxs-lookup"><span data-stu-id="bef60-124">String</span></span>| <span data-ttu-id="bef60-125">ID somente leitura da atividade da reunião.</span><span class="sxs-lookup"><span data-stu-id="bef60-125">Read-only ID for the meeting activity.</span></span>|
|<span data-ttu-id="bef60-126">startDate</span><span class="sxs-lookup"><span data-stu-id="bef60-126">startDate</span></span>|<span data-ttu-id="bef60-127">Date</span><span class="sxs-lookup"><span data-stu-id="bef60-127">Date</span></span>|<span data-ttu-id="bef60-128">Data de início da atividade da reunião.</span><span class="sxs-lookup"><span data-stu-id="bef60-128">Date when the meeting activity started.</span></span> <span data-ttu-id="bef60-129">O valor é representado no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="bef60-129">The value is represented in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="bef60-130">Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="bef60-130">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="bef60-131">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="bef60-131">timeZoneUsed</span></span>|<span data-ttu-id="bef60-132">String</span><span class="sxs-lookup"><span data-stu-id="bef60-132">String</span></span>|<span data-ttu-id="bef60-133">O fuso horário do Outlook definido pelo usuário no calendário do Outlook é usado para a computação.</span><span class="sxs-lookup"><span data-stu-id="bef60-133">The Outlook time zone that the user sets in Outlook calendar is used for the computation.</span></span> <span data-ttu-id="bef60-134">Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="bef60-134">For example, the property value could be "Pacific Standard Time."</span></span>|
|<span data-ttu-id="bef60-135">afterHours</span><span class="sxs-lookup"><span data-stu-id="bef60-135">afterHours</span></span>|<span data-ttu-id="bef60-136">Duração</span><span class="sxs-lookup"><span data-stu-id="bef60-136">Duration</span></span>|<span data-ttu-id="bef60-137">Tempo gasto em reuniões fora do horário de trabalho, que se baseia na configuração de calendário do Outlook do usuário para horário de trabalho.</span><span class="sxs-lookup"><span data-stu-id="bef60-137">Time spent on meetings outside of working hours, which is based on the user's Outlook calendar setting for work hours.</span></span> <span data-ttu-id="bef60-138">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="bef60-138">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="bef60-139">conflitantes</span><span class="sxs-lookup"><span data-stu-id="bef60-139">conflicting</span></span>|<span data-ttu-id="bef60-140">Duração</span><span class="sxs-lookup"><span data-stu-id="bef60-140">Duration</span></span>|<span data-ttu-id="bef60-141">Tempo gasto em reuniões conflitantes (reuniões que se sobrepõem a outras reuniões que a pessoa aceitou e onde o status da pessoa está definido como ocupado).</span><span class="sxs-lookup"><span data-stu-id="bef60-141">Time spent in conflicting meetings (meetings that overlap with other meetings that the person accepted and where the person’s status is set to Busy).</span></span> <span data-ttu-id="bef60-142">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="bef60-142">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="bef60-143">long</span><span class="sxs-lookup"><span data-stu-id="bef60-143">long</span></span>|<span data-ttu-id="bef60-144">Duração</span><span class="sxs-lookup"><span data-stu-id="bef60-144">Duration</span></span>|<span data-ttu-id="bef60-145">Tempo gasto em reuniões longas (mais de uma hora em duração).</span><span class="sxs-lookup"><span data-stu-id="bef60-145">Time spent in long meetings (more than an hour in duration).</span></span> <span data-ttu-id="bef60-146">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="bef60-146">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="bef60-147">multitarefas</span><span class="sxs-lookup"><span data-stu-id="bef60-147">multitasking</span></span>|<span data-ttu-id="bef60-148">Duração</span><span class="sxs-lookup"><span data-stu-id="bef60-148">Duration</span></span>|<span data-ttu-id="bef60-149">Tempo gasto em reuniões em que a pessoa estava multitarefa (leitura/envio de mais de um número mínimo de emails e/ou envio de mais de um número mínimo de mensagens no Microsoft Teams ou no Skype for Business).</span><span class="sxs-lookup"><span data-stu-id="bef60-149">Time spent in meetings where the person was multitasking (read/sent more than a minimum number of emails and/or sent more than a minimum number of messages in Teams or in Skype for Business).</span></span> <span data-ttu-id="bef60-150">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="bef60-150">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="bef60-151">organiza</span><span class="sxs-lookup"><span data-stu-id="bef60-151">organized</span></span>|<span data-ttu-id="bef60-152">Duração</span><span class="sxs-lookup"><span data-stu-id="bef60-152">Duration</span></span>|<span data-ttu-id="bef60-153">Tempo gasto em reuniões organizadas pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="bef60-153">Time spent in meetings organized by the user.</span></span> <span data-ttu-id="bef60-154">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="bef60-154">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="bef60-155">recorrente</span><span class="sxs-lookup"><span data-stu-id="bef60-155">recurring</span></span>|<span data-ttu-id="bef60-156">Duração</span><span class="sxs-lookup"><span data-stu-id="bef60-156">Duration</span></span>|<span data-ttu-id="bef60-157">Tempo gasto em reuniões recorrentes.</span><span class="sxs-lookup"><span data-stu-id="bef60-157">Time spent on recurring meetings.</span></span> <span data-ttu-id="bef60-158">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="bef60-158">The value is represented in ISO 8601 format for durations.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bef60-159">Relações</span><span class="sxs-lookup"><span data-stu-id="bef60-159">Relationships</span></span>

<span data-ttu-id="bef60-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bef60-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bef60-161">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bef60-161">JSON representation</span></span>

<span data-ttu-id="bef60-162">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bef60-162">The following is a JSON representation of the resource.</span></span>

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