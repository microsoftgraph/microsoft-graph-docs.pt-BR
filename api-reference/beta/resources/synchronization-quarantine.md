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
# <a name="synchronizationquarantine-resource-type"></a>tipo de recurso de synchronizationQuarantine

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Fornece informações sobre o estado de quarentena de um [synchronizationJob](synchronization-synchronizationjob.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|currentBegan|DateTimeOffset|Data e hora de quando a quarentena foi última avaliada e impostas. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|nextAttempt|DateTimeOffset|Data e hora de quando a próxima tentativa reavalie a quarentena será feita. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|motivo|Cadeia de caracteres|Um código que significa o motivo pelo qual a quarentena foi imposta. Os valores possíveis são: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `Unknown`.|
|seriesBegan|DateTimeOffset|Data e hora de quando a quarentena primeiro foi imposta nesta série (uma série inicia quando uma quarentena é imposta pela primeira vez e é redefinida assim que a quarentena está ativada). O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|seriesCount|Int64|Número de vezes nesta série de quarentena foi avaliado novamente e deixado em vigor (uma série inicia quando quarentena é imposta pela primeira vez e é redefinida tão logo quarentena é elevada).|

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationQuarantine resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
