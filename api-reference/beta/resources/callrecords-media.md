---
title: tipo de recurso de mídia
description: O tipo de mídia
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1b996c34c3d12984cc512dbcc4d1113d54bd5f69
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394670"
---
# <a name="media-resource-type"></a>tipo de recurso de mídia

Namespace: Microsoft. Graph. callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a mídia (áudio, vídeo, compartilhamento de tela baseado em vídeo, etc.) usada em uma chamada.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|rótulo|String|Como a mídia foi identificada durante o estágio de negociação de mídia.|
|callerDevice|[Microsoft. Graph. callRecords. deviceInfo](callrecords-deviceinfo.md)|Informações do dispositivo associadas ao ponto de extremidade do chamador desta mídia.|
|callerNetwork|[Microsoft. Graph. callRecords. networkInfo](callrecords-networkinfo.md)|Informações de rede associadas ao ponto de extremidade do chamador desta mídia.|
|calleeDevice|[Microsoft. Graph. callRecords. deviceInfo](callrecords-deviceinfo.md)|Informações do dispositivo associadas ao ponto de extremidade do receptor desta mídia.|
|calleeNetwork|[Microsoft. Graph. callRecords. networkInfo](callrecords-networkinfo.md)|Informações de rede associadas ao ponto de extremidade chamado desta mídia.|
|streaming|coleção [Microsoft. Graph. callRecords. mediaStream](callrecords-mediastream.md)|Fluxos de rede associados a essa mídia.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.media",
  "baseType": null
}-->

```json
{
  "label": "String",
  "callerDevice": {"@odata.type": "microsoft.graph.callRecords.deviceInfo"},
  "callerNetwork": {"@odata.type": "microsoft.graph.callRecords.networkInfo"},
  "calleeDevice": {"@odata.type": "microsoft.graph.callRecords.deviceInfo"},
  "calleeNetwork": {"@odata.type": "microsoft.graph.callRecords.networkInfo"},
  "streams": [{"@odata.type": "microsoft.graph.callRecords.mediaStream"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "media resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->