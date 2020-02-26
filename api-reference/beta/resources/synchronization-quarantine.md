---
title: tipo de recurso synchronizationQuarantine
description: Fornece informações sobre o estado de quarentena de um synchronizationJob.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d5e36d62c26225a3dda5fe0adb4610c56c226b79
ms.sourcegitcommit: d419565add1f731be50c9b5911eb1310fa007097
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2020
ms.locfileid: "42280698"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="dd3b5-103">tipo de recurso synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="dd3b5-103">synchronizationQuarantine resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd3b5-104">Fornece informações sobre o estado de quarentena de um [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="dd3b5-104">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dd3b5-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd3b5-105">Properties</span></span>
| <span data-ttu-id="dd3b5-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd3b5-106">Property</span></span>     | <span data-ttu-id="dd3b5-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd3b5-107">Type</span></span>   |<span data-ttu-id="dd3b5-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd3b5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd3b5-109">currentBegan</span><span class="sxs-lookup"><span data-stu-id="dd3b5-109">currentBegan</span></span>|<span data-ttu-id="dd3b5-110">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd3b5-110">DateTimeOffset</span></span>|<span data-ttu-id="dd3b5-111">Data e hora em que a quarentena foi avaliada pela última vez e imposta.</span><span class="sxs-lookup"><span data-stu-id="dd3b5-111">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="dd3b5-112">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="dd3b5-112">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="dd3b5-113">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="dd3b5-113">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="dd3b5-114">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="dd3b5-114">nextAttempt</span></span>|<span data-ttu-id="dd3b5-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd3b5-115">DateTimeOffset</span></span>|<span data-ttu-id="dd3b5-116">Data e hora em que a próxima tentativa de reavaliar a quarentena será feita.</span><span class="sxs-lookup"><span data-stu-id="dd3b5-116">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="dd3b5-117">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="dd3b5-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="dd3b5-118">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="dd3b5-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="dd3b5-119">motivo</span><span class="sxs-lookup"><span data-stu-id="dd3b5-119">reason</span></span>|<span data-ttu-id="dd3b5-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd3b5-120">String</span></span>|<span data-ttu-id="dd3b5-121">Um código que significa por que a quarentena foi imposta.</span><span class="sxs-lookup"><span data-stu-id="dd3b5-121">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="dd3b5-122">Os valores possíveis são: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="dd3b5-122">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.</span></span>|
|<span data-ttu-id="dd3b5-123">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="dd3b5-123">seriesBegan</span></span>|<span data-ttu-id="dd3b5-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd3b5-124">DateTimeOffset</span></span>|<span data-ttu-id="dd3b5-125">Data e hora em que a quarentena foi imposta pela primeira vez nesta série (uma série começa quando uma quarentena é imposta pela primeira vez e é redefinida assim que a quarentena é levantada).</span><span class="sxs-lookup"><span data-stu-id="dd3b5-125">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="dd3b5-126">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="dd3b5-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="dd3b5-127">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="dd3b5-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="dd3b5-128">seriesCount</span><span class="sxs-lookup"><span data-stu-id="dd3b5-128">seriesCount</span></span>|<span data-ttu-id="dd3b5-129">Int64</span><span class="sxs-lookup"><span data-stu-id="dd3b5-129">Int64</span></span>|<span data-ttu-id="dd3b5-130">Número de vezes nesta série, a quarentena foi reavaliada e deixada em vigor (uma série é iniciada quando a quarentena é imposta primeiro e é redefinida assim que a quarentena é levantada).</span><span class="sxs-lookup"><span data-stu-id="dd3b5-130">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|
|<span data-ttu-id="dd3b5-131">erro</span><span class="sxs-lookup"><span data-stu-id="dd3b5-131">error</span></span>|[<span data-ttu-id="dd3b5-132">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="dd3b5-132">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="dd3b5-133">Descreve os erros que ocorreram ao colocar o trabalho de sincronização em quarentena.</span><span class="sxs-lookup"><span data-stu-id="dd3b5-133">Describes the error(s) that occurred when putting the synchronization job into quarantine.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dd3b5-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd3b5-134">JSON representation</span></span>

<span data-ttu-id="dd3b5-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd3b5-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationQuarantine"
}-->

```json
{
  "error": {"@odata.type": "microsoft.graph.synchronizationError"},
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
