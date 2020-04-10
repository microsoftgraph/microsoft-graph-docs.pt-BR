---
title: tipo de recurso synchronizationStatus
description: Representa o status atual do synchronizationJob.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f5c17e28c805fbfde1e59a383899da43b5966628
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217266"
---
# <a name="synchronizationstatus-resource-type"></a>tipo de recurso synchronizationStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status atual do [synchronizationJob](synchronization-synchronizationjob.md).

## <a name="properties"></a>Propriedades

| Propriedade                              | Tipo      | Descrição    |
|:--------------------------------------|:----------|:---------------|
|código|Cadeia de Caracteres|Código de status de alto nível do trabalho de sincronização. Os valores possíveis são: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.|
|countSuccessiveCompleteFailures|Int64|Número de vezes consecutivas que esse trabalho falhou.|
|escrowsPruned|Boolean|`true`Se as caução do trabalho (erros no nível do objeto) foram removidas durante a sincronização inicial. As caução podem ser removidas se durante a sincronização inicial, você atinge o limite de erros que normalmente colocam o trabalho em quarentena. Em vez de entrar em quarentena, o processo de sincronização limpa os erros do trabalho e continua até que a sincronização inicial seja concluída. Quando a sincronização inicial for concluída, o trabalho será pausado e aguardará que o cliente Limpe os erros.|
|lastExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Detalhes da última execução do trabalho.|
|lastSuccessfulExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Detalhes da última execução deste trabalho, que não tinham erros.|
|lastSuccessfulExecutionWithExports|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Detalhes da última execução do trabalho, que exportou objetos para o diretório de destino.|
|progresso|coleção [synchronizationProgress](synchronization-synchronizationprogress.md)|Detalhes do progresso de um trabalho para a conclusão.|
|quarentena|[synchronizationQuarantine](synchronization-quarantine.md)|Se o trabalho estiver em quarentena, detalhes da quarentena.|
|steadyStateFirstAchievedTime|DateTimeOffset|O horário em que o estado Steady (não há mais alterações no processo) foi obtido pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|steadyStateLastAchievedTime|DateTimeOffset|O horário em que o estado Steady (não mais alterações no processo) foi atingido pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|synchronizedEntryCountByType|coleção [stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)|Contagem de objetos sincronizados, listados por tipo de objeto.|
|troubleshootingUrl|Cadeia de Caracteres|No caso de um erro, a URL com as etapas de solução de problemas para o problema.|

### <a name="synchronization-status-code-details"></a>Detalhes do código de status de sincronização

| Valor                              | Descrição    |
|:-----------------------------------|:---------------|
|NotConfigured                       |O trabalho não foi configurado e nunca foi executado. Nenhuma autorização foi fornecida. |
|NotRun                              |O trabalho foi configurado e possivelmente foi iniciado, mas não concluiu sua primeira execução.|
|Ativo                              |O trabalho está sendo executado periodicamente.|
|Em pausa                              |O trabalho foi pausado (geralmente por um administrador) e não está em execução no momento, mas o estado do trabalho é preservado.|
|Quarentena                          |O trabalho está em quarentena. Isso pode acontecer quando há um alto volume de erros ou erros críticos, como credenciais revogadas/expiradas. Enquanto estiver em quarentena, o processo de sincronização tentará executar o trabalho com uma frequência reduzida.|

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
