---
title: tipo de recurso synchronizationQuarantine
description: Fornece informações sobre o estado de quarentena de um synchronizationJob.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2a0564630857a7b032ad076e5fa10556f456d064
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520125"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="828f1-103">tipo de recurso synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="828f1-103">synchronizationQuarantine resource type</span></span>

<span data-ttu-id="828f1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="828f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="828f1-105">Fornece informações sobre o estado de quarentena de um [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="828f1-105">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="828f1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="828f1-106">Properties</span></span>
| <span data-ttu-id="828f1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="828f1-107">Property</span></span>     | <span data-ttu-id="828f1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="828f1-108">Type</span></span>   |<span data-ttu-id="828f1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="828f1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="828f1-110">currentBegan</span><span class="sxs-lookup"><span data-stu-id="828f1-110">currentBegan</span></span>|<span data-ttu-id="828f1-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="828f1-111">DateTimeOffset</span></span>|<span data-ttu-id="828f1-112">Data e hora em que a quarentena foi avaliada pela última vez e imposta.</span><span class="sxs-lookup"><span data-stu-id="828f1-112">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="828f1-113">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="828f1-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="828f1-114">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="828f1-114">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="828f1-115">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="828f1-115">nextAttempt</span></span>|<span data-ttu-id="828f1-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="828f1-116">DateTimeOffset</span></span>|<span data-ttu-id="828f1-117">Data e hora em que a próxima tentativa de reavaliar a quarentena será feita.</span><span class="sxs-lookup"><span data-stu-id="828f1-117">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="828f1-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="828f1-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="828f1-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="828f1-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="828f1-120">motivo</span><span class="sxs-lookup"><span data-stu-id="828f1-120">reason</span></span>|<span data-ttu-id="828f1-121">String</span><span class="sxs-lookup"><span data-stu-id="828f1-121">String</span></span>|<span data-ttu-id="828f1-122">Um código que significa por que a quarentena foi imposta.</span><span class="sxs-lookup"><span data-stu-id="828f1-122">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="828f1-123">Os valores possíveis são: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="828f1-123">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.</span></span>|
|<span data-ttu-id="828f1-124">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="828f1-124">seriesBegan</span></span>|<span data-ttu-id="828f1-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="828f1-125">DateTimeOffset</span></span>|<span data-ttu-id="828f1-126">Data e hora em que a quarentena foi imposta pela primeira vez nesta série (uma série começa quando uma quarentena é imposta pela primeira vez e é redefinida assim que a quarentena é levantada).</span><span class="sxs-lookup"><span data-stu-id="828f1-126">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="828f1-127">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="828f1-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="828f1-128">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="828f1-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="828f1-129">seriesCount</span><span class="sxs-lookup"><span data-stu-id="828f1-129">seriesCount</span></span>|<span data-ttu-id="828f1-130">Int64</span><span class="sxs-lookup"><span data-stu-id="828f1-130">Int64</span></span>|<span data-ttu-id="828f1-131">Número de vezes nesta série, a quarentena foi reavaliada e deixada em vigor (uma série é iniciada quando a quarentena é imposta primeiro e é redefinida assim que a quarentena é levantada).</span><span class="sxs-lookup"><span data-stu-id="828f1-131">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|
|<span data-ttu-id="828f1-132">erro</span><span class="sxs-lookup"><span data-stu-id="828f1-132">error</span></span>|[<span data-ttu-id="828f1-133">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="828f1-133">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="828f1-134">Descreve os erros que ocorreram ao colocar o trabalho de sincronização em quarentena.</span><span class="sxs-lookup"><span data-stu-id="828f1-134">Describes the error(s) that occurred when putting the synchronization job into quarantine.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="828f1-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="828f1-135">JSON representation</span></span>

<span data-ttu-id="828f1-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="828f1-136">The following is a JSON representation of the resource.</span></span>

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
