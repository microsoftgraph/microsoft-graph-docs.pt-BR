---
title: tipo de recurso synchronizationQuarantine
description: Fornece informações sobre o estado de quarentena de um synchronizationJob.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5cd0766c7631c1874f7c3d2457fc01ab39c5edc3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023884"
---
# <a name="synchronizationquarantine-resource-type"></a>tipo de recurso synchronizationQuarantine

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece informações sobre o estado de quarentena de um [synchronizationJob](synchronization-synchronizationjob.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|currentBegan|DateTimeOffset|Data e hora em que a quarentena foi avaliada pela última vez e imposta. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|nextAttempt|DateTimeOffset|Data e hora em que a próxima tentativa de reavaliar a quarentena será feita. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|motivo|String|Um código que significa por que a quarentena foi imposta. Os valores possíveis são: `EncounteredBaseEscrowThreshold`, `EncounteredTotalEscrowThreshold`, `EncounteredEscrowProportionThreshold`, `EncounteredQuarantineException`, `QuarantinedOnDemand`, `TooManyDeletes`, `Unknown`.|
|seriesBegan|DateTimeOffset|Data e hora em que a quarentena foi imposta pela primeira vez nesta série (uma série começa quando uma quarentena é imposta pela primeira vez e é redefinida assim que a quarentena é levantada). O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|seriesCount|Int64|Número de vezes nesta série, a quarentena foi reavaliada e deixada em vigor (uma série é iniciada quando a quarentena é imposta primeiro e é redefinida assim que a quarentena é levantada).|
|erro|[synchronizationError](synchronization-synchronizationerror.md)|Descreve os erros que ocorreram ao colocar o trabalho de sincronização em quarentena.|

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


