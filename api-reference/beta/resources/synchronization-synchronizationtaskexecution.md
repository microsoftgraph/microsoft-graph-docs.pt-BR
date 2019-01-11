---
title: tipo de recurso de synchronizationTaskExecution
description: Resume os resultados da execução do trabalho de sincronização.
localization_priority: Normal
ms.openlocfilehash: 99b6c66b15577ee4c6cbbf5ffe44e17cf0672696
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851503"
---
# <a name="synchronizationtaskexecution-resource-type"></a>tipo de recurso de synchronizationTaskExecution

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Resume os resultados da execução do trabalho de sincronização.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|activityIdentifier           |Cadeia de caracteres |Identificador da execução do trabalho.|
|countEntitled                |Int64  |Contagem de entradas processadas que foram atribuídas para esse aplicativo.|
|countEntitledForProvisioning |Int64  |Contagem de entradas processadas que foram atribuídas pelo provisionamento.|
|countEscrowed                |Int64  |Contagem de entradas que foram caucionados (erros).|
|countEscrowedRaw             |Int64  |Contagem de entradas que foram caucionadas, incluindo escrows gerada pelo sistema.|
|countExported                |Int64  |Contagem de entradas exportadas.|
|countExports                 |Int64  |Contagem de entradas que eram esperados a ser exportado.|
|countImported                |Int64  |Contagem de entradas importadas.|
|countImportedDeltas          |Int64  |Contagem de alterações de delta importadas.|
|countImportedReferenceDeltas |Int64  |Contagem de alterações de delta importadas referentes às alterações de referência.|
|erro                        |[synchronizationError](synchronization-synchronizationerror.md)|Se foi encontrado um erro, contém um objeto **synchronizationError** com detalhes.|
|estado                        |Cadeia de caracteres |Resumindo o resultado dessa execução de código. Os valores possíveis são: `Succeeded`, `Failed`, `EntryLevelErrors`.|
|timeBegan                    |DateTimeOffset|Começou a hora quando esse trabalho é executado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|timeEnded                    |DateTimeOffset|Quando esse trabalho é executado de tempo é encerrada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTaskExecution resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
