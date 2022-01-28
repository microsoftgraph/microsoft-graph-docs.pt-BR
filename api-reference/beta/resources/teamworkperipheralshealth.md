---
title: tipo de recurso teamworkPeripheralsHealth
description: Representa detalhes de saúde para todos os dispositivos periféricos anexados a um dispositivo Microsoft Teams habilitado para Microsoft Teams usuário.
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: d48c0351a20ed1074f5bb2fd4443d40bf96d52d6
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262285"
---
# <a name="teamworkperipheralshealth-resource-type"></a>tipo de recurso teamworkPeripheralsHealth

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa detalhes de saúde para todos os dispositivos periféricos anexados a um dispositivo Microsoft Teams habilitado para [Microsoft Teams usuário](../resources/teamworkdevice.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|communicationSpeakerHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|Os detalhes de saúde sobre o alto-falante de comunicação.|
|contentCameraHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|Os detalhes de saúde sobre a câmera de conteúdo.|
|displayHealthCollection|[coleção teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|Os detalhes de saúde sobre as exibições.|
|microphoneHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|Os detalhes de saúde sobre o microfone.|
|roomCameraHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|Os detalhes de saúde sobre a câmera de sala.|
|speakerHealth|[teamworkPeripheralHealth](../resources/teamworkperipheralhealth.md)|Os detalhes de saúde sobre o alto-falante.|


## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamworkPeripheralsHealth"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamworkPeripheralsHealth",
  "communicationSpeakerHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  },
  "contentCameraHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  },
  "displayHealthCollection": [
    {
      "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
    }
  ],
  "microphoneHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  },
  "roomCameraHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  },
  "speakerHealth": {
    "@odata.type": "microsoft.graph.teamworkPeripheralHealth"
  }
}
```

