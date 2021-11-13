---
title: tipo de recurso monitoringRule
description: Regra que define um sinal e um limite a ser monitorado e a ação a ser cumprida quando atendida.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 376de8e06d5fee242dc068362a4daaa99c977cd2
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890434"
---
# <a name="monitoringrule-resource-type"></a>tipo de recurso monitoringRule

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Regra que define um sinal e um limite a ser monitorado e a ação a ser cumprida quando atendida.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|microsoft.graph.windowsUpdates.monitoringAction|    A ação acionada quando o limite para o sinal determinado é atendido. Os valores possíveis são: `alertError`, `pauseDeployment`, `unknownFutureValue`.|
|signal|microsoft.graph.windowsUpdates.monitoringSignal|O sinal a ser monitorado. Os valores possíveis são: `rollback` e `unknownFutureValue`.|
|threshold|Int32|O limite para um sinal no qual disparar a ação. Um inteiro de 1 a 100 (inclusive).|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.monitoringRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.monitoringRule",
  "signal": "String",
  "threshold": "Integer",
  "action": "String"
}
```

