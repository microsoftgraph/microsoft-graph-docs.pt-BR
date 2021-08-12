---
title: tipo de recurso de mídia
description: O tipo de mídia
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4e97d372e7c243a2cfbc4bbc8f44ec155a8addb70d624972a292ad9516824019
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54252113"
---
# <a name="media-resource-type"></a>tipo de recurso de mídia

Namespace: microsoft.graph.callRecords

Representa a mídia (áudio, vídeo, compartilhamento de tela baseado em vídeo, etc.) usada em uma chamada.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|rótulo|Cadeia de caracteres|Como a mídia foi identificada durante o estágio de negociação de mídia.|
|callerDevice|[microsoft.graph.callRecords.deviceInfo](callrecords-deviceinfo.md)|Informações do dispositivo associadas ao ponto de extremidade do chamador desta mídia.|
|callerNetwork|[microsoft.graph.callRecords.networkInfo](callrecords-networkinfo.md)|Informações de rede associadas ao ponto de extremidade do chamador desta mídia.|
|calleeDevice|[microsoft.graph.callRecords.deviceInfo](callrecords-deviceinfo.md)|Informações do dispositivo associadas ao ponto de extremidade do chamador desta mídia.|
|calleeNetwork|[microsoft.graph.callRecords.networkInfo](callrecords-networkinfo.md)|Informações de rede associadas ao ponto de extremidade do chamador desta mídia.|
|streams|[coleção microsoft.graph.callRecords.mediaStream](callrecords-mediastream.md)|Fluxos de rede associados a essa mídia.|

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
