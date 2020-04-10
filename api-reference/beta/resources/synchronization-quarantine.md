---
title: tipo de recurso synchronizationQuarantine
description: Fornece informações sobre o estado de quarentena de um synchronizationJob.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dd2641c7327ce0670d3b13ab05701c7da5eb0de6
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217595"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="97e73-103">tipo de recurso synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="97e73-103">synchronizationQuarantine resource type</span></span>

<span data-ttu-id="97e73-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97e73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97e73-105">Fornece informações sobre o estado de quarentena de um [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="97e73-105">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="97e73-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97e73-106">Properties</span></span>
| <span data-ttu-id="97e73-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97e73-107">Property</span></span>     | <span data-ttu-id="97e73-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="97e73-108">Type</span></span>   |<span data-ttu-id="97e73-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="97e73-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97e73-110">currentBegan</span><span class="sxs-lookup"><span data-stu-id="97e73-110">currentBegan</span></span>|<span data-ttu-id="97e73-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97e73-111">DateTimeOffset</span></span>|<span data-ttu-id="97e73-112">Data e hora em que a quarentena foi avaliada pela última vez e imposta.</span><span class="sxs-lookup"><span data-stu-id="97e73-112">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="97e73-113">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="97e73-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="97e73-114">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="97e73-114">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="97e73-115">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="97e73-115">nextAttempt</span></span>|<span data-ttu-id="97e73-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97e73-116">DateTimeOffset</span></span>|<span data-ttu-id="97e73-117">Data e hora em que a próxima tentativa de reavaliar a quarentena será feita.</span><span class="sxs-lookup"><span data-stu-id="97e73-117">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="97e73-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="97e73-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="97e73-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="97e73-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="97e73-120">motivo</span><span class="sxs-lookup"><span data-stu-id="97e73-120">reason</span></span>|<span data-ttu-id="97e73-121">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="97e73-121">String</span></span>|<span data-ttu-id="97e73-122">Um código que significa por que a quarentena foi imposta.</span><span class="sxs-lookup"><span data-stu-id="97e73-122">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="97e73-123">Os valores possíveis são: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="97e73-123">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.</span></span>|
|<span data-ttu-id="97e73-124">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="97e73-124">seriesBegan</span></span>|<span data-ttu-id="97e73-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97e73-125">DateTimeOffset</span></span>|<span data-ttu-id="97e73-126">Data e hora em que a quarentena foi imposta pela primeira vez nesta série (uma série começa quando uma quarentena é imposta pela primeira vez e é redefinida assim que a quarentena é levantada).</span><span class="sxs-lookup"><span data-stu-id="97e73-126">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="97e73-127">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="97e73-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="97e73-128">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="97e73-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="97e73-129">seriesCount</span><span class="sxs-lookup"><span data-stu-id="97e73-129">seriesCount</span></span>|<span data-ttu-id="97e73-130">Int64</span><span class="sxs-lookup"><span data-stu-id="97e73-130">Int64</span></span>|<span data-ttu-id="97e73-131">Número de vezes nesta série, a quarentena foi reavaliada e deixada em vigor (uma série é iniciada quando a quarentena é imposta primeiro e é redefinida assim que a quarentena é levantada).</span><span class="sxs-lookup"><span data-stu-id="97e73-131">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|
|<span data-ttu-id="97e73-132">erro</span><span class="sxs-lookup"><span data-stu-id="97e73-132">error</span></span>|[<span data-ttu-id="97e73-133">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="97e73-133">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="97e73-134">Descreve os erros que ocorreram ao colocar o trabalho de sincronização em quarentena.</span><span class="sxs-lookup"><span data-stu-id="97e73-134">Describes the error(s) that occurred when putting the synchronization job into quarantine.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97e73-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97e73-135">JSON representation</span></span>

<span data-ttu-id="97e73-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="97e73-136">The following is a JSON representation of the resource.</span></span>

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
