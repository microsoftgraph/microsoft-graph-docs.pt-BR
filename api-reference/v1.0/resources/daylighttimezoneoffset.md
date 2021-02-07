---
title: Tipo de recurso daylightTimeZoneOffset
description: Especifica quando um fuso horário muda do horário padrão para o horário de verão.
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 79e5af9a7a117d3747928d211229bbbd27d046bf
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135143"
---
# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="f1b4f-103">Tipo de recurso daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="f1b4f-103">daylightTimeZoneOffset resource type</span></span>

<span data-ttu-id="f1b4f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1b4f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f1b4f-105">Especifica quando um fuso horário muda do horário padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="f1b4f-105">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="f1b4f-106">Por exemplo, se um fuso horário estiver especificado com as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="f1b4f-106">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="f1b4f-107">**bias** como 300</span><span class="sxs-lookup"><span data-stu-id="f1b4f-107">**bias** is 300</span></span>
- <span data-ttu-id="f1b4f-108">**daylightBias** como -100</span><span class="sxs-lookup"><span data-stu-id="f1b4f-108">**daylightBias** is -100</span></span>
- <span data-ttu-id="f1b4f-109">**dayOccurrence** como 4</span><span class="sxs-lookup"><span data-stu-id="f1b4f-109">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="f1b4f-110">**dayOfWeek** como "domingo"</span><span class="sxs-lookup"><span data-stu-id="f1b4f-110">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="f1b4f-111">**month** como 5</span><span class="sxs-lookup"><span data-stu-id="f1b4f-111">**month** is 5</span></span>
- <span data-ttu-id="f1b4f-112">**time** como 02:00:00 _ **year** como 0, significa que a hora durante o horário de verão é +300-100=200 minutos adiantada ao UTC.</span><span class="sxs-lookup"><span data-stu-id="f1b4f-112">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="f1b4f-113">A transição do fuso horário de horário de verão para o horário padrão ocorre às 2 da manhã no quarto domingo de maio, todos os anos.</span><span class="sxs-lookup"><span data-stu-id="f1b4f-113">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="f1b4f-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f1b4f-114">Properties</span></span>
| <span data-ttu-id="f1b4f-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1b4f-115">Property</span></span>     | <span data-ttu-id="f1b4f-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1b4f-116">Type</span></span>   |<span data-ttu-id="f1b4f-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1b4f-117">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f1b4f-118">daylightBias</span><span class="sxs-lookup"><span data-stu-id="f1b4f-118">daylightBias</span></span> | <span data-ttu-id="f1b4f-119">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="f1b4f-119">Edm.Int32</span></span> | <span data-ttu-id="f1b4f-120">A diferença de horário em relação ao UTC (Tempo Universal Coordenado) para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="f1b4f-120">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="f1b4f-121">Este valor está em minutos.</span><span class="sxs-lookup"><span data-stu-id="f1b4f-121">This value is in minutes.</span></span>  |
| <span data-ttu-id="f1b4f-122">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="f1b4f-122">dayOccurrence</span></span> | <span data-ttu-id="f1b4f-123">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="f1b4f-123">Edm.Int32</span></span> | <span data-ttu-id="f1b4f-124">Representa a enésima ocorrência do dia da semana em que a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="f1b4f-124">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="f1b4f-125">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="f1b4f-125">dayOfWeek</span></span> | <span data-ttu-id="f1b4f-126">string</span><span class="sxs-lookup"><span data-stu-id="f1b4f-126">string</span></span> | <span data-ttu-id="f1b4f-127">Representa o dia da semana em que a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="f1b4f-127">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="f1b4f-128">month</span><span class="sxs-lookup"><span data-stu-id="f1b4f-128">month</span></span> | <span data-ttu-id="f1b4f-129">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="f1b4f-129">Edm.Int32</span></span> | <span data-ttu-id="f1b4f-130">Representa o mês do ano em que a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="f1b4f-130">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="f1b4f-131">time</span><span class="sxs-lookup"><span data-stu-id="f1b4f-131">time</span></span> | <span data-ttu-id="f1b4f-132">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f1b4f-132">Edm.TimeOfDay</span></span> | <span data-ttu-id="f1b4f-133">Representa a hora do dia em que a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="f1b4f-133">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="f1b4f-134">year</span><span class="sxs-lookup"><span data-stu-id="f1b4f-134">year</span></span> | <span data-ttu-id="f1b4f-135">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="f1b4f-135">Edm.Int32</span></span> | <span data-ttu-id="f1b4f-136">Representa com que frequência, em anos, a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="f1b4f-136">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="f1b4f-137">Por exemplo, um valor 0 significa todos os anos.</span><span class="sxs-lookup"><span data-stu-id="f1b4f-137">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f1b4f-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f1b4f-138">JSON representation</span></span>

<span data-ttu-id="f1b4f-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f1b4f-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.standardTimeZoneOffset",
  "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
}-->

```json
{
  "daylightBias": "Int32",
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "daylightTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

