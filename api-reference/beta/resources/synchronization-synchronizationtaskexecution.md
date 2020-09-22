---
title: tipo de recurso synchronizationTaskExecution
description: Resume os resultados da execução do trabalho de sincronização.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5d777a575290699c2a936902614aa8ef0e8b042d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094908"
---
# <a name="synchronizationtaskexecution-resource-type"></a>tipo de recurso synchronizationTaskExecution

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Resume os resultados da execução do trabalho de sincronização.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|activityIdentifier           |Cadeia de caracteres |Identificador do trabalho executado.|
|countEntitled                |Int64  |Contagem de entradas processadas que foram atribuídas para este aplicativo.|
|countEntitledForProvisioning |Int64  |Contagem de entradas processadas que foram atribuídas para provisionamento.|
|countEscrowed                |Int64  |Contagem de entradas que foram caução (erros).|
|countEscrowedRaw             |Int64  |Contagem de entradas que foram caução, incluindo caução geradas pelo sistema.|
|countExported                |Int64  |Contagem de entradas exportadas.|
|countExports                 |Int64  |Contagem de entradas que devem ser exportadas.|
|countImported                |Int64  |Contagem de entradas importadas.|
|countImportedDeltas          |Int64  |Contagem de alterações delta importadas.|
|countImportedReferenceDeltas |Int64  |Contagem de alterações delta importadas referentes a alterações de referência.|
|erro                        |[synchronizationError](synchronization-synchronizationerror.md)|Se for encontrado um erro, conterá um objeto **synchronizationError** com detalhes.|
|state                        |Cadeia de caracteres |Código que resume o resultado desta execução. Os valores possíveis são: `Succeeded`, `Failed`, `EntryLevelErrors`.|
|timecomeçou                    |DateTimeOffset|Hora em que esta execução de trabalho começou. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|timeterminou                    |DateTimeOffset|Hora em que esse trabalho foi executado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationTaskExecution"
}-->

```json
{
  "activityIdentifier": "String",
  "countEntitled": 1024,
  "countEntitledForProvisioning": 1024,
  "countEscrowed": 1024,
  "countEscrowedRaw": 1024,
  "countExported": 1024,
  "countExports": 1024,
  "countImported": 1024,
  "countImportedDeltas": 1024,
  "countImportedReferenceDeltas": 1024,
  "error": {"@odata.type": "microsoft.graph.synchronizationError"},
  "state": "String",
  "timeBegan": "String (timestamp)",
  "timeEnded": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


