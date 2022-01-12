---
title: tipo de recurso monitoringRule
description: Regra que define um sinal e um limite a ser monitorado e a ação a ser cumprida quando atendida.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 3ae09d2f4a3badf62ffa22380372e597b7fd6a4f
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61792180"
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

