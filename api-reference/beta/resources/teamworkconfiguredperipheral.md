---
title: tipo de recurso teamworkConfiguredPeripheral
description: Representa os detalhes sobre um dispositivo periférico configurado para um dispositivo Microsoft Teams habilitado para Microsoft Teams.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 07a25c847acb1b9b7e3584b2a1a5ef86d7bff046
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262295"
---
# <a name="teamworkconfiguredperipheral-resource-type"></a>tipo de recurso teamworkConfiguredPeripheral

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes sobre um dispositivo periférico configurado para um dispositivo Microsoft Teams habilitado para [Microsoft Teams.](../resources/teamworkdevice.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isOptional|Booliano|`True` se o periférico atual for opcional. Se definido como `false`, essa propriedade também será usada como parte do cálculo do estado de saúde do dispositivo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|periférico|[teamworkPeripheral](../resources/teamworkperipheral.md)|Detalhes sobre os dispositivos periféricos anexados.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkConfiguredPeripheral"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkConfiguredPeripheral",
  "isOptional": "Boolean"
}
```

