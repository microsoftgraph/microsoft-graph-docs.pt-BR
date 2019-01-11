---
title: Tipo de recurso daylightTimeZoneOffset
description: Especifica quando um fuso horário muda do horário padrão para o horário de verão.
localization_priority: Normal
ms.openlocfilehash: 740b6da9a934c1a30a382d46e64377f9a73ffaa1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811582"
---
# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="274e0-103">Tipo de recurso daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="274e0-103">daylightTimeZoneOffset resource type</span></span>

<span data-ttu-id="274e0-104">Especifica quando um fuso horário muda do horário padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="274e0-104">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="274e0-105">Por exemplo, se um fuso horário estiver especificado com as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="274e0-105">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="274e0-106">**bias** como 300</span><span class="sxs-lookup"><span data-stu-id="274e0-106">**bias** is 300</span></span>
- <span data-ttu-id="274e0-107">**daylightBias** como -100</span><span class="sxs-lookup"><span data-stu-id="274e0-107">**daylightBias** is -100</span></span>
- <span data-ttu-id="274e0-108">**dayOccurrence** como 4</span><span class="sxs-lookup"><span data-stu-id="274e0-108">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="274e0-109">**dayOfWeek** como "domingo"</span><span class="sxs-lookup"><span data-stu-id="274e0-109">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="274e0-110">**month** como 5</span><span class="sxs-lookup"><span data-stu-id="274e0-110">**month** is 5</span></span>
- <span data-ttu-id="274e0-111">**time** como 02:00:00 _**year** como 0, significa que a hora durante o horário de verão é +300-100=200 minutos adiantada ao UTC.</span><span class="sxs-lookup"><span data-stu-id="274e0-111">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="274e0-112">A transição do fuso horário de horário de verão para o horário padrão ocorre às 2 da manhã no quarto domingo de maio, todos os anos.</span><span class="sxs-lookup"><span data-stu-id="274e0-112">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="274e0-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="274e0-113">Properties</span></span>
| <span data-ttu-id="274e0-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="274e0-114">Property</span></span>     | <span data-ttu-id="274e0-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="274e0-115">Type</span></span>   |<span data-ttu-id="274e0-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="274e0-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="274e0-117">daylightBias</span><span class="sxs-lookup"><span data-stu-id="274e0-117">daylightBias</span></span> | <span data-ttu-id="274e0-118">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="274e0-118">Edm.Int32</span></span> | <span data-ttu-id="274e0-119">A diferença de horário em relação ao UTC (Tempo Universal Coordenado) para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="274e0-119">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="274e0-120">Este valor está em minutos.</span><span class="sxs-lookup"><span data-stu-id="274e0-120">This value is in minutes.</span></span>  |
| <span data-ttu-id="274e0-121">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="274e0-121">dayOccurrence</span></span> | <span data-ttu-id="274e0-122">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="274e0-122">Edm.Int32</span></span> | <span data-ttu-id="274e0-123">Representa a enésima ocorrência do dia da semana em que a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="274e0-123">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="274e0-124">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="274e0-124">dayOfWeek</span></span> | <span data-ttu-id="274e0-125">string</span><span class="sxs-lookup"><span data-stu-id="274e0-125">string</span></span> | <span data-ttu-id="274e0-126">Representa o dia da semana em que a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="274e0-126">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="274e0-127">month</span><span class="sxs-lookup"><span data-stu-id="274e0-127">month</span></span> | <span data-ttu-id="274e0-128">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="274e0-128">Edm.Int32</span></span> | <span data-ttu-id="274e0-129">Representa o mês do ano em que a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="274e0-129">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="274e0-130">time</span><span class="sxs-lookup"><span data-stu-id="274e0-130">time</span></span> | <span data-ttu-id="274e0-131">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="274e0-131">Edm.TimeOfDay</span></span> | <span data-ttu-id="274e0-132">Representa a hora do dia em que a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="274e0-132">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="274e0-133">year</span><span class="sxs-lookup"><span data-stu-id="274e0-133">year</span></span> | <span data-ttu-id="274e0-134">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="274e0-134">Edm.Int32</span></span> | <span data-ttu-id="274e0-135">Representa com que frequência, em anos, a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="274e0-135">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="274e0-136">Por exemplo, um valor 0 significa todos os anos.</span><span class="sxs-lookup"><span data-stu-id="274e0-136">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="274e0-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="274e0-137">JSON representation</span></span>

<span data-ttu-id="274e0-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="274e0-138">Here is a JSON representation of the resource.</span></span>

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
