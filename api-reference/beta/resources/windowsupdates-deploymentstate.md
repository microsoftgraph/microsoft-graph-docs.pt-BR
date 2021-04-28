---
title: Tipo de recurso deploymentState
description: Descreve e controla o estado atual de uma implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: d05bf09fbad405e93ee994858e2d6ac65a8088a7
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067229"
---
# <a name="deploymentstate-resource-type"></a>Tipo de recurso deploymentState

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve e controla o estado atual de uma implantação.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|reasons|[coleção microsoft.graph.windowsUpdates.deploymentStateReason](../resources/windowsupdates-deploymentstatereason.md)|Especifica os motivos pelos quais a implantação tem seu valor de estado. Somente leitura.|
|requestedValue|microsoft.graph.windowsUpdates.requestedDeploymentStateValue|Especifica o estado solicitado da implantação. Oferece suporte a um subconjunto dos **valores de requestedDeploymentStateValue**. Os valores possíveis são: `none` e `paused`.|
|valor|microsoft.graph.windowsUpdates.deploymentStateValue|Especifica o estado da implantação. Oferece suporte a um subconjunto dos valores **para deploymentStateValue**. Os valores possíveis são: `scheduled`, `offering`, `paused`. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.deploymentState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.deploymentState",
  "value": "String",
  "reasons": [
    {
      "@odata.type": "microsoft.graph.windowsUpdates.deploymentStateReason"
    }
  ],
  "requestedValue": "String",
}
```

