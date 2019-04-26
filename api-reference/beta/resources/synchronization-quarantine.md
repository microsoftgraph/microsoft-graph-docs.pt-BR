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
# <a name="synchronizationquarantine-resource-type"></a>tipo de recurso synchronizationQuarantine

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece informações sobre o estado de quarentena de um [synchronizationJob](synchronization-synchronizationjob.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|currentBegan|DateTimeOffset|Data e hora em que a quarentena foi avaliada pela última vez e imposta. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|nextAttempt|DateTimeOffset|Data e hora em que a próxima tentativa de reavaliar a quarentena será feita. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|motivos|String|Um código que significa por que a quarentena foi imposta. Os valores possíveis são: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.|
|seriesBegan|DateTimeOffset|Data e hora em que a quarentena foi imposta pela primeira vez nesta série (uma série começa quando uma quarentena é imposta pela primeira vez e é redefinida assim que a quarentena é levantada). O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|seriesCount|Int64|Número de vezes nesta série, a quarentena foi reavaliada e deixada em vigor (uma série é iniciada quando a quarentena é imposta primeiro e é redefinida assim que a quarentena é levantada).|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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
