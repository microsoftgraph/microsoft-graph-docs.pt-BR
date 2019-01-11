---
title: tipo de recurso de synchronizationQuarantine
description: Fornece informações sobre o estado de quarentena de um synchronizationJob.
localization_priority: Normal
ms.openlocfilehash: fba0077d48e69ed4c2c190d0b50a6fcfc1749626
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849725"
---
# <a name="synchronizationquarantine-resource-type"></a><span data-ttu-id="38d83-103">tipo de recurso de synchronizationQuarantine</span><span class="sxs-lookup"><span data-stu-id="38d83-103">synchronizationQuarantine resource type</span></span>

> <span data-ttu-id="38d83-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="38d83-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38d83-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="38d83-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="38d83-106">Fornece informações sobre o estado de quarentena de um [synchronizationJob](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="38d83-106">Provides information about the quarantine state of a [synchronizationJob](synchronization-synchronizationjob.md).</span></span>

## <a name="properties"></a><span data-ttu-id="38d83-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="38d83-107">Properties</span></span>
| <span data-ttu-id="38d83-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="38d83-108">Property</span></span>     | <span data-ttu-id="38d83-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="38d83-109">Type</span></span>   |<span data-ttu-id="38d83-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="38d83-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38d83-111">currentBegan</span><span class="sxs-lookup"><span data-stu-id="38d83-111">currentBegan</span></span>|<span data-ttu-id="38d83-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38d83-112">DateTimeOffset</span></span>|<span data-ttu-id="38d83-113">Data e hora de quando a quarentena foi última avaliada e impostas.</span><span class="sxs-lookup"><span data-stu-id="38d83-113">Date and time when the quarantine was last evaluated and imposed.</span></span> <span data-ttu-id="38d83-114">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="38d83-114">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="38d83-115">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="38d83-115">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="38d83-116">nextAttempt</span><span class="sxs-lookup"><span data-stu-id="38d83-116">nextAttempt</span></span>|<span data-ttu-id="38d83-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38d83-117">DateTimeOffset</span></span>|<span data-ttu-id="38d83-118">Data e hora de quando a próxima tentativa reavalie a quarentena será feita.</span><span class="sxs-lookup"><span data-stu-id="38d83-118">Date and time when the next attempt to re-evaluate the quarantine will be made.</span></span> <span data-ttu-id="38d83-119">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="38d83-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="38d83-120">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="38d83-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="38d83-121">motivo</span><span class="sxs-lookup"><span data-stu-id="38d83-121">reason</span></span>|<span data-ttu-id="38d83-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="38d83-122">String</span></span>|<span data-ttu-id="38d83-123">Um código que significa o motivo pelo qual a quarentena foi imposta.</span><span class="sxs-lookup"><span data-stu-id="38d83-123">A code that signifies why the quarantine was imposed.</span></span> <span data-ttu-id="38d83-124">Os valores possíveis são: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span><span class="sxs-lookup"><span data-stu-id="38d83-124">Possible values are: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.</span></span>|
|<span data-ttu-id="38d83-125">seriesBegan</span><span class="sxs-lookup"><span data-stu-id="38d83-125">seriesBegan</span></span>|<span data-ttu-id="38d83-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38d83-126">DateTimeOffset</span></span>|<span data-ttu-id="38d83-127">Data e hora de quando a quarentena primeiro foi imposta nesta série (uma série inicia quando uma quarentena é imposta pela primeira vez e é redefinida assim que a quarentena está ativada).</span><span class="sxs-lookup"><span data-stu-id="38d83-127">Date and time when the quarantine was first imposed in this series (a series starts when a quarantine is first imposed, and is reset as soon as the quarantine is lifted).</span></span> <span data-ttu-id="38d83-128">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="38d83-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="38d83-129">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="38d83-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="38d83-130">seriesCount</span><span class="sxs-lookup"><span data-stu-id="38d83-130">seriesCount</span></span>|<span data-ttu-id="38d83-131">Int64</span><span class="sxs-lookup"><span data-stu-id="38d83-131">Int64</span></span>|<span data-ttu-id="38d83-132">Número de vezes nesta série de quarentena foi avaliado novamente e deixado em vigor (uma série inicia quando quarentena é imposta pela primeira vez e é redefinida tão logo quarentena é elevada).</span><span class="sxs-lookup"><span data-stu-id="38d83-132">Number of times in this series the quarantine was re-evaluated and left in effect (a series starts when quarantine is first imposed, and is reset as soon as quarantine is lifted).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="38d83-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="38d83-133">JSON representation</span></span>

<span data-ttu-id="38d83-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="38d83-134">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationQuarantine resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
