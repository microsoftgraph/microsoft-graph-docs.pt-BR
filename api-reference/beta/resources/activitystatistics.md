---
title: tipo de recurso activityStatistics
description: Representa o tempo gasto em atividades de trabalho, incluindo email, reuniões, trabalho de foco, chats e chamadas.
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 3d2e626535d579b77c27125500d7247401f26915
ms.sourcegitcommit: d419565add1f731be50c9b5911eb1310fa007097
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2020
ms.locfileid: "42280614"
---
# <a name="activitystatistics-resource-type"></a><span data-ttu-id="de41b-103">tipo de recurso activityStatistics</span><span class="sxs-lookup"><span data-stu-id="de41b-103">activityStatistics resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de41b-104">Representa o tempo gasto por um usuário em várias atividades de trabalho durante e fora do horário de trabalho, para o intervalo de tempo especificado na solicitação, que usa um período de agregação de um dia.</span><span class="sxs-lookup"><span data-stu-id="de41b-104">Represents time spent by a user on various work activities during and outside of working hours, for the specified time range in the request, which uses an aggregation period of one day.</span></span>

<span data-ttu-id="de41b-105">Os seguintes tipos de estatísticas são derivados de **activityStatistics**:</span><span class="sxs-lookup"><span data-stu-id="de41b-105">The following types of statistics are derived from **activityStatistics**:</span></span>

* [<span data-ttu-id="de41b-106">Call</span><span class="sxs-lookup"><span data-stu-id="de41b-106">Call</span></span>](callactivitystatistics.md)
* [<span data-ttu-id="de41b-107">Chat</span><span class="sxs-lookup"><span data-stu-id="de41b-107">Chat</span></span>](chatactivitystatistics.md)
* [<span data-ttu-id="de41b-108">Email</span><span class="sxs-lookup"><span data-stu-id="de41b-108">Email</span></span>](emailactivitystatistics.md)
* [<span data-ttu-id="de41b-109">Foco</span><span class="sxs-lookup"><span data-stu-id="de41b-109">Focus</span></span>](focusactivitystatistics.md)
* [<span data-ttu-id="de41b-110">Atenda</span><span class="sxs-lookup"><span data-stu-id="de41b-110">Meeting</span></span>](meetingactivitystatistics.md)

<!--  removing per Mathew 2/6/2020   ### Activity id property

In an HTTP request, to get a specific type of activity statistics within a date range, you can express this information as an ID to the user's collection of activityStatistics in the following format, where `{startdate}` and `{enddate}` are expressed in ISO 8601 calendar date format and `{activity}` can be "call", "chat", "email", "focus", or "meeting":

```
{activity}_{startdate}_{enddate}
```

For example, the ID "email_2019-08-10_2019-08-12" represents the emailActivityStatistics for the specified user between August 10, 2019 and August 12, 2019.
-->
## <a name="methods"></a><span data-ttu-id="de41b-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="de41b-111">Methods</span></span>

| <span data-ttu-id="de41b-112">Método</span><span class="sxs-lookup"><span data-stu-id="de41b-112">Method</span></span>       | <span data-ttu-id="de41b-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="de41b-113">Return Type</span></span> | <span data-ttu-id="de41b-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="de41b-114">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="de41b-115">Listar activityStatistics</span><span class="sxs-lookup"><span data-stu-id="de41b-115">List activityStatistics</span></span>](../api/activitystatistics-list.md) | [<span data-ttu-id="de41b-116">activityStatistics</span><span class="sxs-lookup"><span data-stu-id="de41b-116">activityStatistics</span></span>](activitystatistics.md) | <span data-ttu-id="de41b-117">Recupere as propriedades da coleção de estatísticas de atividade de um usuário para a última semana completa.</span><span class="sxs-lookup"><span data-stu-id="de41b-117">Retrieve the properties for the collection of activity statistics for a user, for the last complete week.</span></span> |

## <a name="properties"></a><span data-ttu-id="de41b-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de41b-118">Properties</span></span>

| <span data-ttu-id="de41b-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de41b-119">Property</span></span>     | <span data-ttu-id="de41b-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="de41b-120">Type</span></span>        | <span data-ttu-id="de41b-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="de41b-121">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="de41b-122">atividade</span><span class="sxs-lookup"><span data-stu-id="de41b-122">activity</span></span> |<span data-ttu-id="de41b-123">analyticsActivityType</span><span class="sxs-lookup"><span data-stu-id="de41b-123">analyticsActivityType</span></span> |<span data-ttu-id="de41b-124">O tipo de atividade para a qual as estatísticas são retornadas.</span><span class="sxs-lookup"><span data-stu-id="de41b-124">The type of activity for which statistics are returned.</span></span> <span data-ttu-id="de41b-125">Os valores possíveis são: `call`, `chat`, `email`, `focus`e `meeting`.</span><span class="sxs-lookup"><span data-stu-id="de41b-125">The possible values are: `call`, `chat`, `email`, `focus`, and `meeting`.</span></span> |
|<span data-ttu-id="de41b-126">duration</span><span class="sxs-lookup"><span data-stu-id="de41b-126">duration</span></span> |<span data-ttu-id="de41b-127">Duração</span><span class="sxs-lookup"><span data-stu-id="de41b-127">Duration</span></span> |<span data-ttu-id="de41b-128">Total de horas gasto na atividade.</span><span class="sxs-lookup"><span data-stu-id="de41b-128">Total hours spent on the activity.</span></span> <span data-ttu-id="de41b-129">O valor é representado no formato ISO 8601 para durações.</span><span class="sxs-lookup"><span data-stu-id="de41b-129">The value is represented in ISO 8601 format for durations.</span></span> |
|<span data-ttu-id="de41b-130">endDate</span><span class="sxs-lookup"><span data-stu-id="de41b-130">endDate</span></span> |<span data-ttu-id="de41b-131">Data</span><span class="sxs-lookup"><span data-stu-id="de41b-131">Date</span></span> |<span data-ttu-id="de41b-132">Data em que a atividade foi concluída, expressada no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="de41b-132">Date when the activity ended, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="de41b-133">Por exemplo, o valor da propriedade poderia ser "2019-07-03" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="de41b-133">For example, the property value could be "2019-07-03" that follows the YYYY-MM-DD format.</span></span> |
|<span data-ttu-id="de41b-134">id</span><span class="sxs-lookup"><span data-stu-id="de41b-134">id</span></span> |<span data-ttu-id="de41b-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de41b-135">String</span></span> |<span data-ttu-id="de41b-136">ID somente leitura da atividade.</span><span class="sxs-lookup"><span data-stu-id="de41b-136">Read-only ID for the activity.</span></span> <span data-ttu-id="de41b-137">Não analise ou personalize o valor para seus cenários.</span><span class="sxs-lookup"><span data-stu-id="de41b-137">Do not parse or customize the value for your scenarios.</span></span> |
|<span data-ttu-id="de41b-138">startDate</span><span class="sxs-lookup"><span data-stu-id="de41b-138">startDate</span></span> |<span data-ttu-id="de41b-139">Date</span><span class="sxs-lookup"><span data-stu-id="de41b-139">Date</span></span> |<span data-ttu-id="de41b-140">Data em que a atividade foi iniciada, expressa no formato ISO 8601 para datas do calendário.</span><span class="sxs-lookup"><span data-stu-id="de41b-140">Date when the activity started, expressed in ISO 8601 format for calendar dates.</span></span> <span data-ttu-id="de41b-141">Por exemplo, o valor da propriedade poderia ser "2019-07-04" que segue o formato AAAA-MM-DD.</span><span class="sxs-lookup"><span data-stu-id="de41b-141">For example, the property value could be "2019-07-04" that follows the YYYY-MM-DD format.</span></span> |
|<span data-ttu-id="de41b-142">timeZoneUsed</span><span class="sxs-lookup"><span data-stu-id="de41b-142">timeZoneUsed</span></span> |<span data-ttu-id="de41b-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de41b-143">String</span></span> |<span data-ttu-id="de41b-144">O fuso horário que o usuário define no Microsoft Outlook é usado para a computação.</span><span class="sxs-lookup"><span data-stu-id="de41b-144">The time zone that the user sets in Microsoft Outlook is used for the computation.</span></span> <span data-ttu-id="de41b-145">Por exemplo, o valor da propriedade poderia ser "hora padrão do Pacífico".</span><span class="sxs-lookup"><span data-stu-id="de41b-145">For example, the property value could be "Pacific Standard Time."</span></span> |

## <a name="relationships"></a><span data-ttu-id="de41b-146">Relações</span><span class="sxs-lookup"><span data-stu-id="de41b-146">Relationships</span></span>

<span data-ttu-id="de41b-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de41b-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de41b-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de41b-148">JSON representation</span></span>

<span data-ttu-id="de41b-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de41b-149">The following is a JSON representation of the resource.</span></span>

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