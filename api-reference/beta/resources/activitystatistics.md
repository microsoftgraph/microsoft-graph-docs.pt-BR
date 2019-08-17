---
title: tipo de recurso activityStatistics
description: Representa o tempo gasto em atividades de trabalho, incluindo email, reuniões, trabalho de foco, chats e chamadas.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5cee94c1ff36bf30d977b7eb97d77f11d4d2ff5e
ms.sourcegitcommit: 9cd96fcbaae9d2ebaa3f3b69e440a1aea106f535
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/17/2019
ms.locfileid: "36450699"
---
# <a name="activitystatistics-resource-type"></a><span data-ttu-id="0eabf-103">tipo de recurso activityStatistics</span><span class="sxs-lookup"><span data-stu-id="0eabf-103">activityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0eabf-104">Representa o tempo gasto por um usuário em várias atividades de trabalho durante e fora do horário de trabalho, para o intervalo de tempo especificado na solicitação, que usa um período de agregação de um dia.</span><span class="sxs-lookup"><span data-stu-id="0eabf-104">Represents time spent by a user on various work activities during and outside of working hours, for the specified time range in the request, which uses an aggregation period of one day.</span></span>

<span data-ttu-id="0eabf-105">Os seguintes tipos de estatísticas são derivados de **activityStatistics**:</span><span class="sxs-lookup"><span data-stu-id="0eabf-105">The following types of statistics are derived from **activityStatistics**:</span></span>

* [<span data-ttu-id="0eabf-106">Call</span><span class="sxs-lookup"><span data-stu-id="0eabf-106">Call</span></span>](callactivitystatistics.md)
* [<span data-ttu-id="0eabf-107">Chat</span><span class="sxs-lookup"><span data-stu-id="0eabf-107">Chat</span></span>](chatactivitystatistics.md)
* [<span data-ttu-id="0eabf-108">Email</span><span class="sxs-lookup"><span data-stu-id="0eabf-108">Email</span></span>](emailactivitystatistics.md)
* [<span data-ttu-id="0eabf-109">Foco</span><span class="sxs-lookup"><span data-stu-id="0eabf-109">Focus</span></span>](focusactivitystatistics.md)
* [<span data-ttu-id="0eabf-110">Atenda</span><span class="sxs-lookup"><span data-stu-id="0eabf-110">Meeting</span></span>](meetingactivitystatistics.md)

### <a name="activity-id-property"></a><span data-ttu-id="0eabf-111">Propriedade ID da atividade</span><span class="sxs-lookup"><span data-stu-id="0eabf-111">Activity id property</span></span>

<span data-ttu-id="0eabf-112">Em uma solicitação HTTP, para obter um tipo específico de estatísticas de atividade dentro de um intervalo de datas, você pode expressar essas informações como uma ID para a coleção de activityStatistics do usuário no seguinte formato `{startdate}` , `{enddate}` onde e são expressas no calendário ISO 8601 formato de data `{activity}` e pode ser "Call", "chat", "email", "foco" ou "reunião":</span><span class="sxs-lookup"><span data-stu-id="0eabf-112">In an HTTP request, to get a specific type of activity statistics within a date range, you can express this information as an ID to the user's collection of activityStatistics in the following format, where `{startdate}` and `{enddate}` are expressed in ISO 8601 calendar date format and `{activity}` can be "call", "chat", "email", "focus", or "meeting":</span></span>

```
{activity}_{startdate}_{enddate}
```

<span data-ttu-id="0eabf-113">Por exemplo, a ID "email_2019-08 -10 _2019-08-12" representa o emailActivityStatistics para o usuário especificado entre 10 de agosto de 2019 e 12 de agosto de 2019.</span><span class="sxs-lookup"><span data-stu-id="0eabf-113">For example, the ID "email_2019-08-10_2019-08-12" represents the emailActivityStatistics for the specified user between August 10, 2019 and August 12, 2019.</span></span>

## <a name="methods"></a><span data-ttu-id="0eabf-114">Métodos</span><span class="sxs-lookup"><span data-stu-id="0eabf-114">Methods</span></span>

| <span data-ttu-id="0eabf-115">Método</span><span class="sxs-lookup"><span data-stu-id="0eabf-115">Method</span></span>       | <span data-ttu-id="0eabf-116">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0eabf-116">Return Type</span></span> | <span data-ttu-id="0eabf-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="0eabf-117">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0eabf-118">Obter activityStatistics</span><span class="sxs-lookup"><span data-stu-id="0eabf-118">Get activityStatistics</span></span>](../api/activitystatistics-get.md) | [<span data-ttu-id="0eabf-119">activityStatistics</span><span class="sxs-lookup"><span data-stu-id="0eabf-119">activityStatistics</span></span>](activitystatistics.md) | <span data-ttu-id="0eabf-120">Obter as propriedades das estatísticas de uma atividade especificada para um usuário, para o intervalo de tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="0eabf-120">Get the properties for a specified activity's statistics for a user, for the specified time range.</span></span> |
| [<span data-ttu-id="0eabf-121">Listar activityStatistics</span><span class="sxs-lookup"><span data-stu-id="0eabf-121">List activityStatistics</span></span>](../api/activitystatistics-list.md) | [<span data-ttu-id="0eabf-122">activityStatistics</span><span class="sxs-lookup"><span data-stu-id="0eabf-122">activityStatistics</span></span>](activitystatistics.md) | <span data-ttu-id="0eabf-123">Recupere as propriedades da coleção de estatísticas de atividade de um usuário para a última semana completa.</span><span class="sxs-lookup"><span data-stu-id="0eabf-123">Retrieve the properties for the collection of activity statistics for a user, for the last complete week.</span></span>|

## <a name="properties"></a><span data-ttu-id="0eabf-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0eabf-124">Properties</span></span>

| <span data-ttu-id="0eabf-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0eabf-125">Property</span></span>     | <span data-ttu-id="0eabf-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="0eabf-126">Type</span></span>        | <span data-ttu-id="0eabf-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="0eabf-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0eabf-128">atividade</span><span class="sxs-lookup"><span data-stu-id="0eabf-128">activity</span></span>|<span data-ttu-id="0eabf-129">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="0eabf-129">analyticsActivityType</span></span>| <span data-ttu-id="0eabf-130">O tipo de atividade para a qual as estatísticas são retornadas.</span><span class="sxs-lookup"><span data-stu-id="0eabf-130">The type of activity for which statistics are returned.</span></span> <span data-ttu-id="0eabf-131">Os valores possíveis são: `call`, `chat`, `email`, `focus`e `meeting`.</span><span class="sxs-lookup"><span data-stu-id="0eabf-131">The possible values are: `call`, `chat`, `email`, `focus`, and `meeting`.</span></span>|
|<span data-ttu-id="0eabf-132">duration</span><span class="sxs-lookup"><span data-stu-id="0eabf-132">duration</span></span>|<span data-ttu-id="0eabf-133">Duração</span><span class="sxs-lookup"><span data-stu-id="0eabf-133">Duration</span></span>|<span data-ttu-id="0eabf-134">Total de horas gasto na atividade.</span><span class="sxs-lookup"><span data-stu-id="0eabf-134">Total hours spent on the activity.</span></span> <span data-ttu-id="0eabf-135">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="0eabf-135">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="0eabf-136">endDate</span><span class="sxs-lookup"><span data-stu-id="0eabf-136">endDate</span></span>|<span data-ttu-id="0eabf-137">Data</span><span class="sxs-lookup"><span data-stu-id="0eabf-137">Date</span></span>|<span data-ttu-id="0eabf-138">Data em que a atividade foi concluída, expressada no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="0eabf-138">Date when the activity ended, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="0eabf-139">Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="0eabf-139">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="0eabf-140">id</span><span class="sxs-lookup"><span data-stu-id="0eabf-140">id</span></span>|<span data-ttu-id="0eabf-141">String</span><span class="sxs-lookup"><span data-stu-id="0eabf-141">String</span></span>| <span data-ttu-id="0eabf-142">ID somente leitura da atividade, que representa `{activity}_{startdate}_{enddate}`.</span><span class="sxs-lookup"><span data-stu-id="0eabf-142">Read-only ID for the activity, which represents `{activity}_{startdate}_{enddate}`.</span></span>|
|<span data-ttu-id="0eabf-143">startDate</span><span class="sxs-lookup"><span data-stu-id="0eabf-143">startDate</span></span>|<span data-ttu-id="0eabf-144">Date</span><span class="sxs-lookup"><span data-stu-id="0eabf-144">Date</span></span>|<span data-ttu-id="0eabf-145">Data em que a atividade foi iniciada, expressa no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="0eabf-145">Date when the activity started, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="0eabf-146">Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="0eabf-146">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="0eabf-147">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="0eabf-147">timeZoneUsed</span></span>|<span data-ttu-id="0eabf-148">String</span><span class="sxs-lookup"><span data-stu-id="0eabf-148">String</span></span>|<span data-ttu-id="0eabf-149">O fuso horário que o usuário define no Microsoft Outlook é usado para a computação.</span><span class="sxs-lookup"><span data-stu-id="0eabf-149">The time zone that the user sets in Microsoft Outlook is used for the computation.</span></span> <span data-ttu-id="0eabf-150">Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="0eabf-150">For example, the property value could be "Pacific Standard Time."</span></span>|

## <a name="relationships"></a><span data-ttu-id="0eabf-151">Relações</span><span class="sxs-lookup"><span data-stu-id="0eabf-151">Relationships</span></span>

<span data-ttu-id="0eabf-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0eabf-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0eabf-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0eabf-153">JSON representation</span></span>

<span data-ttu-id="0eabf-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0eabf-154">The following is a JSON representation of the resource.</span></span>

<!-- { 
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activityStatistics",
  "keyProperty": "id"
}-->

```json
{
  "activity": "String",
  "duration": "String (ISO 8601 duration)",
  "endDate": "String (ISO 8601 format)",
  "id": "String (identifier)",
  "startDate": "String (ISO 8601 format)",
  "timeZoneUsed": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "activityStatistics resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}--> 