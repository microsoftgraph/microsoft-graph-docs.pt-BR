---
title: tipo de recurso teamworkHardwareDetail
description: Representa os detalhes sobre as propriedades de hardware de um dispositivo Microsoft Teams habilitado para uso.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ec4c292666a8889a34d1dce85c9a3d70630825a7
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262261"
---
# <a name="teamworkhardwaredetail-resource-type"></a>tipo de recurso teamworkHardwareDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes sobre as propriedades de hardware de um dispositivo Microsoft Teams habilitado [para uso.](../resources/teamworkdevice.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|macAddresses|Conjunto de cadeias de caracteres|Endereço MAC.|
|fabricante|String|Fabricante do dispositivo.|
|modelo|String|Modelo de devie.|
|serialNumber|String|Número de série do dispositivo.|
|uniqueId|String|O identificador exclusivo do dispositivo.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkHardwareDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkHardwareDetail",
  "macAddresses": [
    "String"
  ],
  "manufacturer": "String",
  "model": "String",
  "serialNumber": "String",
  "uniqueId": "String"
}
```

