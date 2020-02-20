---
title: tipo de recurso activityStatistics
description: Representa o tempo gasto em atividades de trabalho, incluindo email, reuniões, trabalho de foco, chats e chamadas.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 18d675b38dd3155b5a06c67fc3164fd315d7c0b2
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42162495"
---
# <a name="activitystatistics-resource-type"></a><span data-ttu-id="74165-103">tipo de recurso activityStatistics</span><span class="sxs-lookup"><span data-stu-id="74165-103">activityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74165-104">Representa o tempo gasto por um usuário em várias atividades de trabalho durante e fora do horário de trabalho, para o intervalo de tempo especificado na solicitação, que usa um período de agregação de um dia.</span><span class="sxs-lookup"><span data-stu-id="74165-104">Represents time spent by a user on various work activities during and outside of working hours, for the specified time range in the request, which uses an aggregation period of one day.</span></span>

<span data-ttu-id="74165-105">Os seguintes tipos de estatísticas são derivados de **activityStatistics**:</span><span class="sxs-lookup"><span data-stu-id="74165-105">The following types of statistics are derived from **activityStatistics**:</span></span>

* [<span data-ttu-id="74165-106">Call</span><span class="sxs-lookup"><span data-stu-id="74165-106">Call</span></span>](callactivitystatistics.md)
* [<span data-ttu-id="74165-107">Chat</span><span class="sxs-lookup"><span data-stu-id="74165-107">Chat</span></span>](chatactivitystatistics.md)
* [<span data-ttu-id="74165-108">Email</span><span class="sxs-lookup"><span data-stu-id="74165-108">Email</span></span>](emailactivitystatistics.md)
* [<span data-ttu-id="74165-109">Foco</span><span class="sxs-lookup"><span data-stu-id="74165-109">Focus</span></span>](focusactivitystatistics.md)
* [<span data-ttu-id="74165-110">Atenda</span><span class="sxs-lookup"><span data-stu-id="74165-110">Meeting</span></span>](meetingactivitystatistics.md)

<!--  removing per Mathew 2/6/2020   ### Activity id property

In an HTTP request, to get a specific type of activity statistics within a date range, you can express this information as an ID to the user's collection of activityStatistics in the following format, where `{startdate}` and `{enddate}` are expressed in ISO 8601 calendar date format and `{activity}` can be "call", "chat", "email", "focus", or "meeting":

```
{activity}_{startdate}_{enddate}
```

For example, the ID "email_2019-08-10_2019-08-12" represents the emailActivityStatistics for the specified user between August 10, 2019 and August 12, 2019.
-->
## <a name="methods"></a><span data-ttu-id="74165-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="74165-111">Methods</span></span>

| <span data-ttu-id="74165-112">Método</span><span class="sxs-lookup"><span data-stu-id="74165-112">Method</span></span>       | <span data-ttu-id="74165-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="74165-113">Return Type</span></span> | <span data-ttu-id="74165-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="74165-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="74165-115">Listar activityStatistics</span><span class="sxs-lookup"><span data-stu-id="74165-115">List activityStatistics</span></span>](../api/activitystatistics-list.md) | [<span data-ttu-id="74165-116">activityStatistics</span><span class="sxs-lookup"><span data-stu-id="74165-116">activityStatistics</span></span>](activitystatistics.md) | <span data-ttu-id="74165-117">Recupere as propriedades da coleção de estatísticas de atividade de um usuário para a última semana completa.</span><span class="sxs-lookup"><span data-stu-id="74165-117">Retrieve the properties for the collection of activity statistics for a user, for the last complete week.</span></span>|

## <a name="properties"></a><span data-ttu-id="74165-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="74165-118">Properties</span></span>

| <span data-ttu-id="74165-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="74165-119">Property</span></span>     | <span data-ttu-id="74165-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="74165-120">Type</span></span>        | <span data-ttu-id="74165-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="74165-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="74165-122">atividade</span><span class="sxs-lookup"><span data-stu-id="74165-122">activity</span></span>|<span data-ttu-id="74165-123">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="74165-123">analyticsActivityType</span></span>| <span data-ttu-id="74165-124">O tipo de atividade para a qual as estatísticas são retornadas.</span><span class="sxs-lookup"><span data-stu-id="74165-124">The type of activity for which statistics are returned.</span></span> <span data-ttu-id="74165-125">Os valores possíveis são: `call`, `chat`, `email`, `focus`e `meeting`.</span><span class="sxs-lookup"><span data-stu-id="74165-125">The possible values are: `call`, `chat`, `email`, `focus`, and `meeting`.</span></span>|
|<span data-ttu-id="74165-126">duration</span><span class="sxs-lookup"><span data-stu-id="74165-126">duration</span></span>|<span data-ttu-id="74165-127">Duração</span><span class="sxs-lookup"><span data-stu-id="74165-127">Duration</span></span>|<span data-ttu-id="74165-128">Total de horas gasto na atividade.</span><span class="sxs-lookup"><span data-stu-id="74165-128">Total hours spent on the activity.</span></span> <span data-ttu-id="74165-129">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="74165-129">The value is represented in ISO 8601 format for durations.</span></span>|
|<span data-ttu-id="74165-130">endDate</span><span class="sxs-lookup"><span data-stu-id="74165-130">endDate</span></span>|<span data-ttu-id="74165-131">Data</span><span class="sxs-lookup"><span data-stu-id="74165-131">Date</span></span>|<span data-ttu-id="74165-132">Data em que a atividade foi concluída, expressada no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="74165-132">Date when the activity ended, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="74165-133">Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="74165-133">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="74165-134">id</span><span class="sxs-lookup"><span data-stu-id="74165-134">id</span></span>|<span data-ttu-id="74165-135">String</span><span class="sxs-lookup"><span data-stu-id="74165-135">String</span></span>| <span data-ttu-id="74165-136">ID somente leitura da atividade, que representa `{activity}_{startdate}_{enddate}`.</span><span class="sxs-lookup"><span data-stu-id="74165-136">Read-only ID for the activity, which represents `{activity}_{startdate}_{enddate}`.</span></span>|
|<span data-ttu-id="74165-137">startDate</span><span class="sxs-lookup"><span data-stu-id="74165-137">startDate</span></span>|<span data-ttu-id="74165-138">Date</span><span class="sxs-lookup"><span data-stu-id="74165-138">Date</span></span>|<span data-ttu-id="74165-139">Data em que a atividade foi iniciada, expressa no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="74165-139">Date when the activity started, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="74165-140">Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="74165-140">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span>|
|<span data-ttu-id="74165-141">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="74165-141">timeZoneUsed</span></span>|<span data-ttu-id="74165-142">String</span><span class="sxs-lookup"><span data-stu-id="74165-142">String</span></span>|<span data-ttu-id="74165-143">O fuso horário que o usuário define no Microsoft Outlook é usado para a computação.</span><span class="sxs-lookup"><span data-stu-id="74165-143">The time zone that the user sets in Microsoft Outlook is used for the computation.</span></span> <span data-ttu-id="74165-144">Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="74165-144">For example, the property value could be "Pacific Standard Time."</span></span>|

## <a name="relationships"></a><span data-ttu-id="74165-145">Relações</span><span class="sxs-lookup"><span data-stu-id="74165-145">Relationships</span></span>

<span data-ttu-id="74165-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="74165-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74165-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="74165-147">JSON representation</span></span>

<span data-ttu-id="74165-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="74165-148">The following is a JSON representation of the resource.</span></span>

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