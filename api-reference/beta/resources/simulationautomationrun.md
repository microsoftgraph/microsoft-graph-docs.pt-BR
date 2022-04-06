---
title: Tipo de recurso simulationAutomationRun
description: Representa uma executar uma automação de simulação de ataque em um locatário.
author: Gopal-MSFT
ms.localizationpriority: medium
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: d5ca41d575ec90e150e8f0d54a37f0278b6b6bdb
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63758306"
---
# <a name="simulationautomationrun-resource-type"></a>Tipo de recurso simulationAutomationRun

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma executar uma automação de simulação de ataque em um locatário.


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar executa](../api/simulationautomation-list-runs.md)|[Coleção simulationAutomationRun](../resources/simulationautomationrun.md)|Obter uma lista de executações de automação de simulação de ataque.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|endDateTime|DateTimeOffset|Data e hora em que a executar termina em uma automação de simulação de ataque.|
|id|String|Identificador exclusivo para a executar uma automação de simulação de ataque.|
|simulationId|Cadeia de Caracteres|Identificador exclusivo da campanha de simulação de ataque iniciada na operação de automação de simulação de ataque.|
|startDateTime|DateTimeOffset|Data e hora em que a executar é iniciada em uma automação de simulação de ataque.|
|status|[simulationAutomationRunStatus](#simulationautomationrunstatus-values)|Status da executar uma automação de simulação de ataque. Os valores possíveis são: `unknown`, `running`, `succeeded`, `failed`, `skipped`, `unknownFutureValue`.|

### <a name="simulationautomationrunstatus-values"></a>valores simulationAutomationRunStatus

|Member|Descrição |
|:---|:---|
|desconhecido| O status de uma corrida de uma automação de simulação não está definido. |
|running| A execução de uma automação de simulação está em execução. |
|bem-sucedido| A executar uma automação de simulação foi bem-sucedida. |
|failed| A executar uma automação de simulação falhou. |
|ignorado| A executar uma automação de simulação foi ignorada. |
|unknownFutureValue| Valor de sentinela de enumeração evolvável. Não usar. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.simulationAutomationRun",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.simulationAutomationRun",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "simulationId": "String",
  "startDateTime": "String (timestamp)",
  "status": "String"
}
```

