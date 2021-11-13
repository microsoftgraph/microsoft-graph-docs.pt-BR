---
title: Tipo de recurso deploymentState
description: Descreve e controla o estado atual de uma implantação.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 80b691c6404bac3e98c4c5c6acb9596b5d4c8821
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890826"
---
# <a name="deploymentstate-resource-type"></a>Tipo de recurso deploymentState

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve e controla o estado atual de uma implantação.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|reasons|[coleção microsoft.graph.windowsUpdates.deploymentStateReason](../resources/windowsupdates-deploymentstatereason.md)|Especifica os motivos pelos quais a implantação tem seu valor de estado. Somente leitura.|
|requestedValue|microsoft.graph.windowsUpdates.requestedDeploymentStateValue|Especifica o estado solicitado da implantação. Oferece suporte a um subconjunto dos **valores de requestedDeploymentStateValue**. Os valores possíveis são: `none`, `paused`, `unknownFutureValue`.|
|valor|microsoft.graph.windowsUpdates.deploymentStateValue|Especifica o estado da implantação. Oferece suporte a um subconjunto dos valores **para deploymentStateValue**. Os valores possíveis são: `scheduled`, `offering`, `paused`, `unknownFutureValue`. Somente leitura.|

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

