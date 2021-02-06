---
title: Tipo de recurso synchronizationStatus
description: Representa o status atual do synchronizationJob.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: bb832fa8d62f2c666b430c242a49bd9138de1b57
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135048"
---
# <a name="synchronizationstatus-resource-type"></a>Tipo de recurso synchronizationStatus

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o status atual do [synchronizationJob](synchronization-synchronizationjob.md).

## <a name="properties"></a>Propriedades

| Propriedade                              | Tipo      | Descrição    |
|:--------------------------------------|:----------|:---------------|
|código|String|Código de status de alto nível do trabalho de sincronização. Os valores possíveis são: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.|
|countSuccessiveCompleteFailures|Int64|Número de vezes consecutivas que esse trabalho falhou.|
|escrowsPruned|Boolean|`true` se os escrows do trabalho (erros no nível do objeto) foram remoção durante a sincronização inicial. Os escrows podem ser desaparados se, durante a sincronização inicial, você atingir o limite de erros que normalmente colocariam o trabalho em quarentena. Em vez de entrar em quarentena, o processo de sincronização limpa os erros do trabalho e continua até que a sincronização inicial seja concluída. Quando a sincronização inicial for concluída, o trabalho será pausado e aguardará até que o cliente limpe os erros.|
|lastExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Detalhes da última execução do trabalho.|
|lastSuccessfulExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Detalhes da última execução deste trabalho, que não teve erros.|
|lastSuccessfulExecutionWithExports|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Detalhes da última execução do trabalho, que exportou objetos para o diretório de destino.|
|progresso|[Coleção synchronizationProgress](synchronization-synchronizationprogress.md)|Detalhes do progresso de um trabalho até a conclusão.|
|quarentena|[synchronizationQuarantine](synchronization-quarantine.md)|Se o trabalho estiver em quarentena, coloque os detalhes em quarentena.|
|steadyStateFirstAchievedTime|DateTimeOffset|O tempo em que o estado estável (sem mais alterações no processo) foi atingido pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|steadyStateLastAchievedTime|DateTimeOffset|O tempo em que o estado estável (sem mais alterações no processo) foi atingido pela última vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|synchronizedEntryCountByType|[Coleção stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)|Contagem de objetos sincronizados, listados por tipo de objeto.|
|troubleshootingUrl|String|Em caso de erro, a URL com as etapas de solução de problemas para o problema.|

### <a name="synchronization-status-code-details"></a>Detalhes do código de status de sincronização

| Valor                              | Descrição    |
|:-----------------------------------|:---------------|
|NotConfigured                       |O trabalho não foi configurado e nunca foi executado. Nenhuma autorização foi fornecida. |
|NotRun                              |O trabalho foi configurado e possivelmente iniciado, mas ainda não concluiu sua primeira vez.|
|Ativo                              |O trabalho é executado periodicamente.|
|Em pausa                              |O trabalho foi pausado (geralmente por um administrador) e atualmente não está em execução, mas o estado do trabalho é preservado.|
|Quarentena                          |O trabalho está em quarentena. Isso pode acontecer quando há um grande volume de erros ou erros críticos, como credenciais revogadas/expiradas. Enquanto estiver em quarentena, o processo de sincronização tentará executar o trabalho com frequência reduzida.|

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


