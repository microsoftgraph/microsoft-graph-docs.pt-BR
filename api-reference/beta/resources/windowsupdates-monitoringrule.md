---
title: tipo de recurso monitoringRule
description: Regra que define um sinal e um limite a ser monitorado e a ação a ser cumprida quando atendida.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 305db31c935329574a2b7d52403dc7664ff53f66
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067793"
---
# <a name="monitoringrule-resource-type"></a>tipo de recurso monitoringRule

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Regra que define um sinal e um limite a ser monitorado e a ação a ser cumprida quando atendida.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ação|microsoft.graph.windowsUpdates.monitoringAction|    A ação acionada quando o limite para o sinal determinado é atendido. Os valores possíveis são: `alertError` e `pauseDeployment`.|
|signal|microsoft.graph.windowsUpdates.monitoringSignal|O sinal a ser monitorado. Os valores possíveis são: `rollback` .|
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

