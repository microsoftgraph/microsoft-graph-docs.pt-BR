---
title: tipo de recurso synchronizationQuarantine
description: Fornece informações sobre o estado de quarentena de um synchronizationJob.
localization_priority: Normal
ms.openlocfilehash: 7036e07b7f812717304e26d8223676d3bb462266
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342883"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="5e7cb-103">tipo de recurso synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="5e7cb-103">synchronizationQuarantine resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e7cb-104">Fornece informações sobre o estado de quarentena de um [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="5e7cb-104">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5e7cb-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5e7cb-105">Properties</span></span>
| <span data-ttu-id="5e7cb-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5e7cb-106">Property</span></span>     | <span data-ttu-id="5e7cb-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5e7cb-107">Type</span></span>   |<span data-ttu-id="5e7cb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5e7cb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5e7cb-109">currentBegan</span><span class="sxs-lookup"><span data-stu-id="5e7cb-109">currentBegan</span></span>|<span data-ttu-id="5e7cb-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e7cb-110">DateTimeOffset</span></span>|<span data-ttu-id="5e7cb-111">Data e hora em que a quarentena foi avaliada pela última vez e imposta.</span><span class="sxs-lookup"><span data-stu-id="5e7cb-111">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="5e7cb-112">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5e7cb-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5e7cb-113">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5e7cb-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="5e7cb-114">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="5e7cb-114">nextAttempt</span></span>|<span data-ttu-id="5e7cb-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e7cb-115">DateTimeOffset</span></span>|<span data-ttu-id="5e7cb-116">Data e hora em que a próxima tentativa de reavaliar a quarentena será feita.</span><span class="sxs-lookup"><span data-stu-id="5e7cb-116">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="5e7cb-117">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5e7cb-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5e7cb-118">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5e7cb-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="5e7cb-119">motivos</span><span class="sxs-lookup"><span data-stu-id="5e7cb-119">reason</span></span>|<span data-ttu-id="5e7cb-120">String</span><span class="sxs-lookup"><span data-stu-id="5e7cb-120">String</span></span>|<span data-ttu-id="5e7cb-121">Um código que significa por que a quarentena foi imposta.</span><span class="sxs-lookup"><span data-stu-id="5e7cb-121">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="5e7cb-122">Os valores possíveis são: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="5e7cb-122">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span></span>|
|<span data-ttu-id="5e7cb-123">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="5e7cb-123">seriesBegan</span></span>|<span data-ttu-id="5e7cb-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5e7cb-124">DateTimeOffset</span></span>|<span data-ttu-id="5e7cb-125">Data e hora em que a quarentena foi imposta pela primeira vez nesta série (uma série começa quando uma quarentena é imposta pela primeira vez e é redefinida assim que a quarentena é levantada).</span><span class="sxs-lookup"><span data-stu-id="5e7cb-125">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="5e7cb-126">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5e7cb-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5e7cb-127">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="5e7cb-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="5e7cb-128">seriesCount</span><span class="sxs-lookup"><span data-stu-id="5e7cb-128">seriesCount</span></span>|<span data-ttu-id="5e7cb-129">Int64</span><span class="sxs-lookup"><span data-stu-id="5e7cb-129">Int64</span></span>|<span data-ttu-id="5e7cb-130">Número de vezes nesta série, a quarentena foi reavaliada e deixada em vigor (uma série é iniciada quando a quarentena é imposta primeiro e é redefinida assim que a quarentena é levantada).</span><span class="sxs-lookup"><span data-stu-id="5e7cb-130">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5e7cb-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5e7cb-131">JSON representation</span></span>

<span data-ttu-id="5e7cb-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5e7cb-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationQuarantine"
}-->

```json
{
  "currentBegan": "String (timestamp)",
  "nextAttempt": "String (timestamp)",
  "reason": "String",
  "seriesBegan": "String (timestamp)",
  "seriesCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationQuarantine resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
