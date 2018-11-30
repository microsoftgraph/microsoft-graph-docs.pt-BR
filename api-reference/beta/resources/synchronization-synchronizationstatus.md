---
title: tipo de recurso de synchronizationStatus
description: Representa o status atual do synchronizationJob.
ms.openlocfilehash: cf1b1e79e5ad784f1f43a2e5bf082c68b41e96ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041081"
---
# <a name="synchronizationstatus-resource-type"></a>tipo de recurso de synchronizationStatus

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa o status atual do [synchronizationJob](synchronization-synchronizationjob.md).

## <a name="properties"></a>Propriedades

| Propriedade                              | Tipo      | Descrição    |
|:--------------------------------------|:----------|:---------------|
|código|String|Código de alto nível de status do trabalho de sincronização. Os valores possíveis são: `NotConfigured`, `NotRun`, `Active`, `Paused`, `Quarantine`.|
|countSuccessiveCompleteFailures|Int64|Número de consecutivos vezes esse trabalho falhou.|
|escrowsPruned|Booliano|`true`Se escrows do trabalho (erros de nível de objeto) foram removidos durante a sincronização inicial. Escrows podem ser removidos se durante a sincronização inicial, você atingir o limite de erros que faria normalmente para inserir o trabalho em quarentena. Em vez de entrar em quarentena, o processo de sincronização limpa erros do trabalho e continua até que a sincronização inicial for concluída. Quando a sincronização inicial for concluída, o trabalho será pausar e aguarde o cliente limpar os erros.|
|lastExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Detalhes da última execução do trabalho.|
|lastSuccessfulExecution|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Detalhes da última execução do trabalho, que não teve que quaisquer erros.|
|lastSuccessfulExecutionWithExports|[synchronizationTaskExecution](synchronization-synchronizationtaskexecution.md)|Detalhes da última execução do trabalho, que são exportados de objetos para o diretório de destino.|
|progresso|coleção [synchronizationProgress](synchronization-synchronizationprogress.md)|Detalhes do progresso de um trabalho de conclusão.|
|quarentena|[synchronizationQuarantine](synchronization-quarantine.md)|Se o trabalho estiver em quarentena, detalhes da quarentena.|
|steadyStateFirstAchievedTime|DateTimeOffset|A hora quando estável (sem alterações para o processo de mais) obteve pela primeira vez. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|steadyStateLastAchievedTime|DateTimeOffset|A hora quando estável (sem alterações para o processo de mais) última obteve. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.|
|synchronizedEntryCountByType|coleção [stringKeyLongValuePair](synchronization-stringkeylongvaluepair.md)|Contagem de objetos sincronizados, listados por tipo de objeto.|
|troubleshootingUrl|String|Se ocorrer um erro, a URL com as etapas de solução de problemas para o problema.|

### <a name="synchronization-status-code-details"></a>Detalhes do código de status de sincronização

| Valor                              | Descrição    |
|:-----------------------------------|:---------------|
|Não-configuradas                       |Trabalho não foi configurado e nunca executar. Nenhuma autorização foi fornecida. |
|NotRun                              |Trabalho tiver sido configurado e possivelmente iniciado, mas ainda não concluído sua primeira execução.|
|Ativo                              |Trabalho está sendo executado periodicamente.|
|Em pausa                              |Trabalho foi pausado (geralmente por um administrador) e atualmente não está em execução, mas o estado do trabalho é preservado.|
|Quarentena                          |Trabalho está em quarentena. Isso pode acontecer quando há um alto volume de erros, ou erros críticos como credenciais revogado/expirou. Enquanto em quarentena, o processo de sincronização tentar executar o trabalho com frequência reduzida.|

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
