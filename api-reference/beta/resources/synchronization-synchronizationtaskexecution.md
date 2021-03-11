---
title: Tipo de recurso synchronizationTaskExecution
description: Resume os resultados do trabalho de sincronização executado.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: d83092949e1f27c9dac9744d2b4b16be4bcbae0d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722045"
---
# <a name="synchronizationtaskexecution-resource-type"></a>Tipo de recurso synchronizationTaskExecution

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Resume os resultados do trabalho de sincronização executado.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|activityIdentifier           |Cadeia de caracteres |Identificador do trabalho executado.|
|countEntitled                |Int64  |Contagem de entradas processadas atribuídas a esse aplicativo.|
|countEntitledForProvisioning |Int64  |Contagem de entradas processadas atribuídas ao provisionamento.|
|countEscrowed                |Int64  |Contagem de entradas que foram escrotadas (erros).|
|countEscrowedRaw             |Int64  |Contagem de entradas que foram escrotadas, incluindo escrows gerados pelo sistema.|
|countExported                |Int64  |Contagem de entradas exportadas.|
|countExports                 |Int64  |Contagem de entradas que eram esperadas para serem exportadas.|
|countImported                |Int64  |Contagem de entradas importadas.|
|countImportedDeltas          |Int64  |Contagem de alterações delta importadas.|
|countImportedReferenceDeltas |Int64  |Contagem de alterações delta importadas relacionadas a alterações de referência.|
|erro                        |[synchronizationError](synchronization-synchronizationerror.md)|Se um erro foi encontrado, contém um objeto **synchronizationError** com detalhes.|
|estado                        |Cadeia de caracteres |Code summarizing the result of this run. Os valores possíveis são: `Succeeded`, `Failed`, `EntryLevelErrors`.|
|timeBegan                    |DateTimeOffset|Hora em que esse trabalho foi executado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|timeEnded                    |DateTimeOffset|Hora em que esse trabalho foi executado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|

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


