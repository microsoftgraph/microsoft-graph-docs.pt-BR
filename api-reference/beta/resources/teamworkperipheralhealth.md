---
title: tipo de recurso teamworkPeripheralHealth
description: Representa detalhes de saúde de um dispositivo periférico anexado a um dispositivo Microsoft Teams habilitado para Microsoft Teams usuário.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 914165343623fea7f807b5dc5f8146b79714c90e
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262267"
---
# <a name="teamworkperipheralhealth-resource-type"></a>tipo de recurso teamworkPeripheralHealth

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa detalhes de saúde de um dispositivo periférico anexado a um dispositivo Microsoft Teams habilitado para [Microsoft Teams usuário](../resources/teamworkdevice.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|connection|[teamworkConnection](../resources/teamworkconnection.md)|O estado e a hora conectados desde que o dispositivo periférico foi conectado.|
|isOptional|Booliano|`True` se o periférico for opcional. Usado para computação de saúde.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|periférico|[teamworkPeripheral](../resources/teamworkperipheral.md)|Informações sobre o dispositivo periférico.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkPeripheralHealth",
  "connection": {
    "@odata.type": "microsoft.graph.teamworkConnection"
  },
  "isOptional": "Boolean"
}
```

