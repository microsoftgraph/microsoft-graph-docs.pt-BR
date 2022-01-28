---
title: tipo de recurso teamworkHardwareConfiguration
description: Representa os detalhes sobre a configuração de hardware de um dispositivo Microsoft Teams habilitado para uso.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 118c2cda70a9751ce8c02a9af52d89982141dfef
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262272"
---
# <a name="teamworkhardwareconfiguration-resource-type"></a>tipo de recurso teamworkHardwareConfiguration

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes sobre a configuração de hardware de um dispositivo Microsoft Teams habilitado [para uso.](../resources/teamworkdevice.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|processorModel|Cadeia de caracteres|O modelo de CPU no dispositivo.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|compute|[teamworkPeripheral](../resources/teamworkperipheral.md)|Os detalhes do sistema para um [trabalho em equipeDevice](../resources/teamworkdevice.md).|
|hdmiIngest|[teamworkPeripheral](../resources/teamworkperipheral.md)|Os detalhes do produto sobre a ingestão HDMI de um dispositivo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkHardwareConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkHardwareConfiguration",
  "processorModel": "String"
}
```

