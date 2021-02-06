---
title: Tipo de recurso synchronizationTaskExecution
description: Resume os resultados do trabalho de sincronização executado.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: ac42a91ec35c1d81d81efa52f4306bbd1cfb2f55
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135034"
---
# <a name="synchronizationtaskexecution-resource-type"></a>Tipo de recurso synchronizationTaskExecution

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Resume os resultados do trabalho de sincronização executado.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|activityIdentifier           |String |Identificador do trabalho executado.|
|countEntitled                |Int64  |Contagem de entradas processadas que foram atribuídas para este aplicativo.|
|countEntitledForProvisioning |Int64  |Contagem de entradas processadas que foram atribuídas para provisionamento.|
|countEscrowed                |Int64  |Contagem de entradas que foram escrotadas (erros).|
|countEscrowedRaw             |Int64  |Contagem de entradas que foram escrotadas, incluindo registros gerados pelo sistema.|
|countExported                |Int64  |Contagem de entradas exportadas.|
|countExports                 |Int64  |Contagem de entradas que devem ser exportadas.|
|countImported                |Int64  |Contagem de entradas importadas.|
|countImportedDeltas          |Int64  |Contagem de alterações delta importadas.|
|countImportedReferenceDeltas |Int64  |Contagem de alterações delta importadas referentes às alterações de referência.|
|erro                        |[synchronizationError](synchronization-synchronizationerror.md)|Se um erro foi encontrado, contém um **objeto synchronizationError** com detalhes.|
|estado                        |String |Código resumindo o resultado dessa sequência. Os valores possíveis são: `Succeeded`, `Failed`, `EntryLevelErrors`.|
|timeBegan                    |DateTimeOffset|Hora em que a tarefa foi iniciada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|timeEnded                    |DateTimeOffset|Hora em que a tarefa foi encerrada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|

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


