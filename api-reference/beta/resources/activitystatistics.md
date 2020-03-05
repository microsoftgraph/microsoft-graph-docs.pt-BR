---
title: tipo de recurso activityStatistics
description: Representa o tempo gasto em atividades de trabalho, incluindo email, reuniões, trabalho de foco, chats e chamadas.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 69b90ae911ca956dedf3a7675d7666c7faa4b906
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508426"
---
# <a name="activitystatistics-resource-type"></a><span data-ttu-id="887ed-103">tipo de recurso activityStatistics</span><span class="sxs-lookup"><span data-stu-id="887ed-103">activityStatistics resource type</span></span>

<span data-ttu-id="887ed-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="887ed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="887ed-105">Representa o tempo gasto por um usuário em várias atividades de trabalho durante e fora do horário de trabalho, para o intervalo de tempo especificado na solicitação, que usa um período de agregação de um dia.</span><span class="sxs-lookup"><span data-stu-id="887ed-105">Represents time spent by a user on various work activities during and outside of working hours, for the specified time range in the request, which uses an aggregation period of one day.</span></span>

<span data-ttu-id="887ed-106">Os seguintes tipos de estatísticas são derivados de **activityStatistics**:</span><span class="sxs-lookup"><span data-stu-id="887ed-106">The following types of statistics are derived from **activityStatistics**:</span></span>

* [<span data-ttu-id="887ed-107">Call</span><span class="sxs-lookup"><span data-stu-id="887ed-107">Call</span></span>](callactivitystatistics.md)
* [<span data-ttu-id="887ed-108">Chat</span><span class="sxs-lookup"><span data-stu-id="887ed-108">Chat</span></span>](chatactivitystatistics.md)
* [<span data-ttu-id="887ed-109">Email</span><span class="sxs-lookup"><span data-stu-id="887ed-109">Email</span></span>](emailactivitystatistics.md)
* [<span data-ttu-id="887ed-110">Foco</span><span class="sxs-lookup"><span data-stu-id="887ed-110">Focus</span></span>](focusactivitystatistics.md)
* [<span data-ttu-id="887ed-111">Atenda</span><span class="sxs-lookup"><span data-stu-id="887ed-111">Meeting</span></span>](meetingactivitystatistics.md)

<!--  removing per Mathew 2/6/2020   ### Activity id property

In an HTTP request, to get a specific type of activity statistics within a date range, you can express this information as an ID to the user's collection of activityStatistics in the following format, where `{startdate}` and `{enddate}` are expressed in ISO 8601 calendar date format and `{activity}` can be "call", "chat", "email", "focus", or "meeting":

```
{activity}_{startdate}_{enddate}
```

For example, the ID "email_2019-08-10_2019-08-12" represents the emailActivityStatistics for the specified user between August 10, 2019 and August 12, 2019.
-->
## <a name="methods"></a><span data-ttu-id="887ed-112">Métodos</span><span class="sxs-lookup"><span data-stu-id="887ed-112">Methods</span></span>

| <span data-ttu-id="887ed-113">Método</span><span class="sxs-lookup"><span data-stu-id="887ed-113">Method</span></span>       | <span data-ttu-id="887ed-114">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="887ed-114">Return Type</span></span> | <span data-ttu-id="887ed-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="887ed-115">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="887ed-116">Listar activityStatistics</span><span class="sxs-lookup"><span data-stu-id="887ed-116">List activityStatistics</span></span>](../api/activitystatistics-list.md) | [<span data-ttu-id="887ed-117">activityStatistics</span><span class="sxs-lookup"><span data-stu-id="887ed-117">activityStatistics</span></span>](activitystatistics.md) | <span data-ttu-id="887ed-118">Recupere as propriedades da coleção de estatísticas de atividade de um usuário para a última semana completa.</span><span class="sxs-lookup"><span data-stu-id="887ed-118">Retrieve the properties for the collection of activity statistics for a user, for the last complete week.</span></span> |

## <a name="properties"></a><span data-ttu-id="887ed-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="887ed-119">Properties</span></span>

| <span data-ttu-id="887ed-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="887ed-120">Property</span></span>     | <span data-ttu-id="887ed-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="887ed-121">Type</span></span>        | <span data-ttu-id="887ed-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="887ed-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="887ed-123">atividade</span><span class="sxs-lookup"><span data-stu-id="887ed-123">activity</span></span> |<span data-ttu-id="887ed-124">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="887ed-124">analyticsActivityType</span></span> |<span data-ttu-id="887ed-125">O tipo de atividade para a qual as estatísticas são retornadas.</span><span class="sxs-lookup"><span data-stu-id="887ed-125">The type of activity for which statistics are returned.</span></span> <span data-ttu-id="887ed-126">Os valores possíveis são: `call`, `chat`, `email`, `focus`e `meeting`.</span><span class="sxs-lookup"><span data-stu-id="887ed-126">The possible values are: `call`, `chat`, `email`, `focus`, and `meeting`.</span></span> |
|<span data-ttu-id="887ed-127">duration</span><span class="sxs-lookup"><span data-stu-id="887ed-127">duration</span></span> |<span data-ttu-id="887ed-128">Duração</span><span class="sxs-lookup"><span data-stu-id="887ed-128">Duration</span></span> |<span data-ttu-id="887ed-129">Total de horas gasto na atividade.</span><span class="sxs-lookup"><span data-stu-id="887ed-129">Total hours spent on the activity.</span></span> <span data-ttu-id="887ed-130">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="887ed-130">The value is represented in ISO 8601 format for durations.</span></span> |
|<span data-ttu-id="887ed-131">endDate</span><span class="sxs-lookup"><span data-stu-id="887ed-131">endDate</span></span> |<span data-ttu-id="887ed-132">Data</span><span class="sxs-lookup"><span data-stu-id="887ed-132">Date</span></span> |<span data-ttu-id="887ed-133">Data em que a atividade foi concluída, expressada no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="887ed-133">Date when the activity ended, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="887ed-134">Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="887ed-134">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span> |
|<span data-ttu-id="887ed-135">id</span><span class="sxs-lookup"><span data-stu-id="887ed-135">id</span></span> |<span data-ttu-id="887ed-136">String</span><span class="sxs-lookup"><span data-stu-id="887ed-136">String</span></span> |<span data-ttu-id="887ed-137">ID somente leitura da atividade.</span><span class="sxs-lookup"><span data-stu-id="887ed-137">Read-only ID for the activity.</span></span> <span data-ttu-id="887ed-138">Não analise ou personalize o valor para seus cenários.</span><span class="sxs-lookup"><span data-stu-id="887ed-138">Do not parse or customize the value for your scenarios.</span></span> |
|<span data-ttu-id="887ed-139">startDate</span><span class="sxs-lookup"><span data-stu-id="887ed-139">startDate</span></span> |<span data-ttu-id="887ed-140">Date</span><span class="sxs-lookup"><span data-stu-id="887ed-140">Date</span></span> |<span data-ttu-id="887ed-141">Data em que a atividade foi iniciada, expressa no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="887ed-141">Date when the activity started, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="887ed-142">Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="887ed-142">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span> |
|<span data-ttu-id="887ed-143">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="887ed-143">timeZoneUsed</span></span> |<span data-ttu-id="887ed-144">String</span><span class="sxs-lookup"><span data-stu-id="887ed-144">String</span></span> |<span data-ttu-id="887ed-145">O fuso horário que o usuário define no Microsoft Outlook é usado para a computação.</span><span class="sxs-lookup"><span data-stu-id="887ed-145">The time zone that the user sets in Microsoft Outlook is used for the computation.</span></span> <span data-ttu-id="887ed-146">Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="887ed-146">For example, the property value could be "Pacific Standard Time."</span></span> |

## <a name="relationships"></a><span data-ttu-id="887ed-147">Relações</span><span class="sxs-lookup"><span data-stu-id="887ed-147">Relationships</span></span>

<span data-ttu-id="887ed-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="887ed-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="887ed-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="887ed-149">JSON representation</span></span>

<span data-ttu-id="887ed-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="887ed-150">The following is a JSON representation of the resource.</span></span>

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