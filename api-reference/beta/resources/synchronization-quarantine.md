---
title: Tipo de recurso synchronizationQuarantine
description: Fornece informações sobre o estado de quarentena de um synchronizationJob.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 1673da71c0fbeaa952bccb89e6edd2c029fad4a6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133130"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="11b07-103">Tipo de recurso synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="11b07-103">synchronizationQuarantine resource type</span></span>

<span data-ttu-id="11b07-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11b07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11b07-105">Fornece informações sobre o estado de quarentena de [um synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="11b07-105">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="11b07-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11b07-106">Properties</span></span>
| <span data-ttu-id="11b07-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11b07-107">Property</span></span>     | <span data-ttu-id="11b07-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="11b07-108">Type</span></span>   |<span data-ttu-id="11b07-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="11b07-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11b07-110">currentBegan</span><span class="sxs-lookup"><span data-stu-id="11b07-110">currentBegan</span></span>|<span data-ttu-id="11b07-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11b07-111">DateTimeOffset</span></span>|<span data-ttu-id="11b07-112">Data e hora em que a quarentena foi avaliada e imposta pela última vez.</span><span class="sxs-lookup"><span data-stu-id="11b07-112">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="11b07-113">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="11b07-113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="11b07-114">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="11b07-114">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="11b07-115">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="11b07-115">nextAttempt</span></span>|<span data-ttu-id="11b07-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11b07-116">DateTimeOffset</span></span>|<span data-ttu-id="11b07-117">Data e hora em que a próxima tentativa de reavaliação da quarentena será feita.</span><span class="sxs-lookup"><span data-stu-id="11b07-117">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="11b07-118">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="11b07-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="11b07-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="11b07-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="11b07-120">motivo</span><span class="sxs-lookup"><span data-stu-id="11b07-120">reason</span></span>|<span data-ttu-id="11b07-121">String</span><span class="sxs-lookup"><span data-stu-id="11b07-121">String</span></span>|<span data-ttu-id="11b07-122">Um código que significa por que a quarentena foi imposta.</span><span class="sxs-lookup"><span data-stu-id="11b07-122">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="11b07-123">Os valores possíveis são: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="11b07-123">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.</span></span>|
|<span data-ttu-id="11b07-124">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="11b07-124">seriesBegan</span></span>|<span data-ttu-id="11b07-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11b07-125">DateTimeOffset</span></span>|<span data-ttu-id="11b07-126">Data e hora em que a quarentena foi imposta pela primeira vez nesta série (uma série começa quando uma quarentena é imposta pela primeira vez e é redefinida assim que a quarentena é suspensa).</span><span class="sxs-lookup"><span data-stu-id="11b07-126">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="11b07-127">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="11b07-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="11b07-128">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="11b07-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="11b07-129">seriesCount</span><span class="sxs-lookup"><span data-stu-id="11b07-129">seriesCount</span></span>|<span data-ttu-id="11b07-130">Int64</span><span class="sxs-lookup"><span data-stu-id="11b07-130">Int64</span></span>|<span data-ttu-id="11b07-131">Número de vezes nesta série que a quarentena foi reavaliada e deixada em vigor (uma série começa quando a quarentena é imposta pela primeira vez e é redefinida assim que a quarentena é suspensa).</span><span class="sxs-lookup"><span data-stu-id="11b07-131">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|
|<span data-ttu-id="11b07-132">erro</span><span class="sxs-lookup"><span data-stu-id="11b07-132">error</span></span>|[<span data-ttu-id="11b07-133">synchronizationError</span><span class="sxs-lookup"><span data-stu-id="11b07-133">synchronizationError</span></span>](synchronization-synchronizationerror.md)|<span data-ttu-id="11b07-134">Descreve os erros ocorridos ao colocar o trabalho de sincronização em quarentena.</span><span class="sxs-lookup"><span data-stu-id="11b07-134">Describes the error(s) that occurred when putting the synchronization job into quarantine.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11b07-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11b07-135">JSON representation</span></span>

<span data-ttu-id="11b07-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11b07-136">The following is a JSON representation of the resource.</span></span>

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


