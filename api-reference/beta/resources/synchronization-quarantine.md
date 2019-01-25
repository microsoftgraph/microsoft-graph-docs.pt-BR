---
title: tipo de recurso de synchronizationQuarantine
description: Fornece informações sobre o estado de quarentena de um synchronizationJob.
localization_priority: Normal
ms.openlocfilehash: 6d5d5c3cbe96eda6b39833287e8efb6e0771b19a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518811"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="90a2f-103">tipo de recurso de synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="90a2f-103">synchronizationQuarantine resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90a2f-104">Fornece informações sobre o estado de quarentena de um [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="90a2f-104">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="90a2f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="90a2f-105">Properties</span></span>
| <span data-ttu-id="90a2f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90a2f-106">Property</span></span>     | <span data-ttu-id="90a2f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="90a2f-107">Type</span></span>   |<span data-ttu-id="90a2f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="90a2f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90a2f-109">currentBegan</span><span class="sxs-lookup"><span data-stu-id="90a2f-109">currentBegan</span></span>|<span data-ttu-id="90a2f-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90a2f-110">DateTimeOffset</span></span>|<span data-ttu-id="90a2f-111">Data e hora de quando a quarentena foi última avaliada e impostas.</span><span class="sxs-lookup"><span data-stu-id="90a2f-111">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="90a2f-112">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="90a2f-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="90a2f-113">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="90a2f-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="90a2f-114">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="90a2f-114">nextAttempt</span></span>|<span data-ttu-id="90a2f-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90a2f-115">DateTimeOffset</span></span>|<span data-ttu-id="90a2f-116">Data e hora de quando a próxima tentativa reavalie a quarentena será feita.</span><span class="sxs-lookup"><span data-stu-id="90a2f-116">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="90a2f-117">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="90a2f-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="90a2f-118">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="90a2f-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="90a2f-119">Reason</span><span class="sxs-lookup"><span data-stu-id="90a2f-119">reason</span></span>|<span data-ttu-id="90a2f-120">String</span><span class="sxs-lookup"><span data-stu-id="90a2f-120">String</span></span>|<span data-ttu-id="90a2f-121">Um código que significa o motivo pelo qual a quarentena foi imposta.</span><span class="sxs-lookup"><span data-stu-id="90a2f-121">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="90a2f-122">Os valores possíveis são: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="90a2f-122">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span></span>|
|<span data-ttu-id="90a2f-123">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="90a2f-123">seriesBegan</span></span>|<span data-ttu-id="90a2f-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="90a2f-124">DateTimeOffset</span></span>|<span data-ttu-id="90a2f-125">Data e hora de quando a quarentena primeiro foi imposta nesta série (uma série inicia quando uma quarentena é imposta pela primeira vez e é redefinida assim que a quarentena está ativada).</span><span class="sxs-lookup"><span data-stu-id="90a2f-125">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="90a2f-126">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="90a2f-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="90a2f-127">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="90a2f-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="90a2f-128">seriesCount</span><span class="sxs-lookup"><span data-stu-id="90a2f-128">seriesCount</span></span>|<span data-ttu-id="90a2f-129">Int64</span><span class="sxs-lookup"><span data-stu-id="90a2f-129">Int64</span></span>|<span data-ttu-id="90a2f-130">Número de vezes nesta série de quarentena foi avaliado novamente e deixado em vigor (uma série inicia quando quarentena é imposta pela primeira vez e é redefinida tão logo quarentena é elevada).</span><span class="sxs-lookup"><span data-stu-id="90a2f-130">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90a2f-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="90a2f-131">JSON representation</span></span>

<span data-ttu-id="90a2f-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="90a2f-132">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-quarantine.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
