---
title: tipo de recurso teamworkActivePeripherals
description: Representa os detalhes sobre os dispositivos periféricos ativos anexados a um dispositivo Microsoft Teams habilitado para uso.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e1f740a347f4adc717588dccc49acafc145e42c8
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262363"
---
# <a name="teamworkactiveperipherals-resource-type"></a>tipo de recurso teamworkActivePeripherals

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes sobre os dispositivos periféricos ativos anexados a um dispositivo Microsoft Teams habilitado [para uso.](../resources/teamworkdevice.md)

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|communicationSpeaker|[teamworkPeripheral](../resources/teamworkperipheral.md)|Detalhes do alto-falante de comunicação vinculado.|
|contentCamera|[teamworkPeripheral](../resources/teamworkperipheral.md)|Detalhes da câmera de conteúdo vinculado.|
|microphone|[teamworkPeripheral](../resources/teamworkperipheral.md)|Detalhes do microfone vinculados.|
|roomCamera|[teamworkPeripheral](../resources/teamworkperipheral.md)|Detalhes da câmera de sala vinculada.|
|speaker|[teamworkPeripheral](../resources/teamworkperipheral.md)|Detalhes do alto-falante vinculado.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkActivePeripherals"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkActivePeripherals"
}
```

