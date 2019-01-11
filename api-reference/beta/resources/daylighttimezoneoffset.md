---
title: Tipo de recurso daylightTimeZoneOffset
description: Especifica quando um fuso horário muda do horário padrão para o horário de verão.
localization_priority: Normal
ms.openlocfilehash: 37e08ec0e695fd245678510ac4a40bc978b1a93e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825603"
---
# <a name="daylighttimezoneoffset-resource-type"></a><span data-ttu-id="11cdc-103">Tipo de recurso daylightTimeZoneOffset</span><span class="sxs-lookup"><span data-stu-id="11cdc-103">daylightTimeZoneOffset resource type</span></span>

> <span data-ttu-id="11cdc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="11cdc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="11cdc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="11cdc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="11cdc-106">Especifica quando um fuso horário muda do horário padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="11cdc-106">Specifies when a time zone switches from standard time to daylight saving time.</span></span>

<span data-ttu-id="11cdc-107">Por exemplo, se um fuso horário estiver especificado com as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="11cdc-107">For example, if a time zone is specified with the following properties:</span></span>

- <span data-ttu-id="11cdc-108">**bias** como 300</span><span class="sxs-lookup"><span data-stu-id="11cdc-108">**bias** is 300</span></span>
- <span data-ttu-id="11cdc-109">**daylightBias** como -100</span><span class="sxs-lookup"><span data-stu-id="11cdc-109">**daylightBias** is -100</span></span>
- <span data-ttu-id="11cdc-110">**dayOccurrence** como 4</span><span class="sxs-lookup"><span data-stu-id="11cdc-110">**dayOccurrence** is 4</span></span>
- <span data-ttu-id="11cdc-111">**dayOfWeek** como "domingo"</span><span class="sxs-lookup"><span data-stu-id="11cdc-111">**dayOfWeek** is "sunday"</span></span>
- <span data-ttu-id="11cdc-112">**month** como 5</span><span class="sxs-lookup"><span data-stu-id="11cdc-112">**month** is 5</span></span>
- <span data-ttu-id="11cdc-113">**time** como 02:00:00 _**year** como 0, significa que a hora durante o horário de verão é +300-100=200 minutos adiantada ao UTC.</span><span class="sxs-lookup"><span data-stu-id="11cdc-113">**time** is 02:00:00 _ **year** is 0 That means the time during daylight saving time is +300-100=200 minutes ahead of UTC.</span></span> <span data-ttu-id="11cdc-114">A transição do fuso horário de horário de verão para o horário padrão ocorre às 2 da manhã no quarto domingo de maio, todos os anos.</span><span class="sxs-lookup"><span data-stu-id="11cdc-114">The time zone transition from daylight saving time to standard occurs at 2 AM on the fourth Sunday of May, every year.</span></span>


## <a name="properties"></a><span data-ttu-id="11cdc-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11cdc-115">Properties</span></span>
| <span data-ttu-id="11cdc-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11cdc-116">Property</span></span>     | <span data-ttu-id="11cdc-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="11cdc-117">Type</span></span>   |<span data-ttu-id="11cdc-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="11cdc-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="11cdc-119">daylightBias</span><span class="sxs-lookup"><span data-stu-id="11cdc-119">daylightBias</span></span> | <span data-ttu-id="11cdc-120">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="11cdc-120">Edm.Int32</span></span> | <span data-ttu-id="11cdc-121">A diferença de horário em relação ao UTC (Tempo Universal Coordenado) para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="11cdc-121">The time offset from Coordinated Universal Time (UTC) for daylight saving time.</span></span> <span data-ttu-id="11cdc-122">Este valor está em minutos.</span><span class="sxs-lookup"><span data-stu-id="11cdc-122">This value is in minutes.</span></span>  |
| <span data-ttu-id="11cdc-123">dayOccurrence</span><span class="sxs-lookup"><span data-stu-id="11cdc-123">dayOccurrence</span></span> | <span data-ttu-id="11cdc-124">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="11cdc-124">Edm.Int32</span></span> | <span data-ttu-id="11cdc-125">Representa a enésima ocorrência do dia da semana em que a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="11cdc-125">Represents the nth occurrence of the day of week that the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="11cdc-126">dayOfWeek</span><span class="sxs-lookup"><span data-stu-id="11cdc-126">dayOfWeek</span></span> | <span data-ttu-id="11cdc-127">string</span><span class="sxs-lookup"><span data-stu-id="11cdc-127">string</span></span> | <span data-ttu-id="11cdc-128">Representa o dia da semana em que a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="11cdc-128">Represents the day of the week when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="11cdc-129">month</span><span class="sxs-lookup"><span data-stu-id="11cdc-129">month</span></span> | <span data-ttu-id="11cdc-130">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="11cdc-130">Edm.Int32</span></span> | <span data-ttu-id="11cdc-131">Representa o mês do ano em que a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="11cdc-131">Represents the month of the year when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="11cdc-132">time</span><span class="sxs-lookup"><span data-stu-id="11cdc-132">time</span></span> | <span data-ttu-id="11cdc-133">Edm.TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="11cdc-133">Edm.TimeOfDay</span></span> | <span data-ttu-id="11cdc-134">Representa a hora do dia em que a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="11cdc-134">Represents the time of day when the transition from standard time to daylight saving time occurs.</span></span> |
| <span data-ttu-id="11cdc-135">year</span><span class="sxs-lookup"><span data-stu-id="11cdc-135">year</span></span> | <span data-ttu-id="11cdc-136">Edm.Int32</span><span class="sxs-lookup"><span data-stu-id="11cdc-136">Edm.Int32</span></span> | <span data-ttu-id="11cdc-137">Representa com que frequência, em anos, a transição do horário padrão para o horário de verão acontece.</span><span class="sxs-lookup"><span data-stu-id="11cdc-137">Represents how frequently in terms of years the change from standard time to daylight saving time occurs.</span></span> <span data-ttu-id="11cdc-138">Por exemplo, um valor 0 significa todos os anos.</span><span class="sxs-lookup"><span data-stu-id="11cdc-138">For example, a value of 0 means every year.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="11cdc-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11cdc-139">JSON representation</span></span>

<span data-ttu-id="11cdc-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11cdc-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
