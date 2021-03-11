---
title: Tipo de recurso synchronizationStatus
description: Representa o status atual do synchronizationJob.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 86320e6af31dae39f86ebe87f8490e24c7c33f57
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722052"
---
# <a name="synchronizationstatus-resource-type"></a>Tipo de recurso synchronizationStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status atual do [synchronizationJob](synchronization-synchronizationjob.md).

## <a name="properties"></a>Propriedades

| Propriedade                              | Tipo      | Descrição    |
|:--------------------------------------|:----------|:---------------|
|código|Cadeia de caracteres|Código de status de alto nível do trabalho de sincronização. Os valores possíveis são: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.|
|countSuccessiveCompleteFailures|Int64|Número de vezes consecutivas em que esse trabalho falhou.|
|escrowsPruned|Booliano|`true` se as escrows do trabalho (erros no nível do objeto) foram podadas durante a sincronização inicial. Os escrows podem ser podados se, durante a sincronização inicial, você atingir o limite de erros que normalmente colocariam o trabalho em quarentena. Em vez de entrar em quarentena, o processo de sincronização limpa os erros do trabalho e continua até que a sincronização inicial seja concluída. Quando a sincronização inicial for concluída, o trabalho será pausado e aguardará que o cliente limpe os erros.|
|lastExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Detalhes da última execução do trabalho.|
|lastSuccessfulExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Detalhes da última execução deste trabalho, que não teve erros.|
|lastSuccessfulExecutionWithExports|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Detalhes da última execução do trabalho, que exportou objetos para o diretório de destino.|
|progresso|[Coleção synchronizationProgress](synchronization-synchronizationprogress.md)|Detalhes do andamento de um trabalho para conclusão.|
|quarantine|[synchronizationQuarantine](synchronization-quarantine.md)|Se o trabalho estiver em quarentena, detalhes de quarentena.|
|steadyStateFirstAchievedTime|DateTimeOffset|O tempo em que o estado estável (sem mais alterações no processo) foi atingido pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|steadyStateLastAchievedTime|DateTimeOffset|O tempo em que o estado estável (sem mais alterações no processo) foi atingido pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|synchronizedEntryCountByType|[coleção stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)|Contagem de objetos sincronizados, listados por tipo de objeto.|
|troubleshootingUrl|Cadeia de caracteres|Em caso de erro, a URL com as etapas de solução de problemas para o problema.|

### <a name="synchronization-status-code-details"></a>Detalhes do código de status de sincronização

| Valor                              | Descrição    |
|:-----------------------------------|:---------------|
|NotConfigured                       |O trabalho não foi configurado e nunca executado. Nenhuma autorização foi fornecida. |
|NotRun                              |Job foi configurado e possivelmente iniciado, mas ainda não concluiu sua primeira executar.|
|Ativo                              |O trabalho é executado periodicamente.|
|Em pausa                              |O trabalho foi pausado (geralmente por um administrador) e atualmente não está em execução, mas o estado do trabalho é preservado.|
|Quarentena                          |O trabalho está em quarentena. Isso pode acontecer quando houver um alto volume de erros ou erros críticos, como credenciais revogadas/expiradas. Enquanto estiver em quarentena, o processo de sincronização tentará executar o trabalho com frequência reduzida.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationStatus"
}-->

```json
{
  "code": "String",
  "countSuccessiveCompleteFailures": 1024,
  "escrowsPruned": true,
  "lastExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecution": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "lastSuccessfulExecutionWithExports": {"@odata.type": "microsoft.graph.synchronizationTaskExecution"},
  "progress": [{"@odata.type": "microsoft.graph.synchronizationProgress"}],
  "quarantine": {"@odata.type": "microsoft.graph.synchronizationQuarantine"},
  "steadyStateFirstAchievedTime": "String (timestamp)",
  "steadyStateLastAchievedTime": "String (timestamp)",
  "synchronizedEntryCountByType": [{"@odata.type": "microsoft.graph.stringKeyLongValuePair"}],
  "troubleshootingUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


