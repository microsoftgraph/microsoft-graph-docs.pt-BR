---
title: tipo de recurso teleconferenceDeviceVideoQuality
description: Representa dados de qualidade de vídeo do dispositivo de teleconferência de vídeo.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8f892fe059828cd7fd71ec19914b5b5db0b9e3cf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086225"
---
# <a name="teleconferencedevicevideoquality-resource-type"></a>tipo de recurso teleconferenceDeviceVideoQuality

Namespace: microsoft.graph

Representa dados de qualidade de vídeo do dispositivo de teleconferência de vídeo.

## <a name="properties"></a>Propriedades

O recurso **teleconferenceDeviceVideoQuality** herda as propriedades de [teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md)e inclui as seguintes propriedades adicionais.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|averageInboundBitRate|Duplo|A taxa média de bits de vídeo de fluxo de entrada por segundo.|
|averageInboundFrameRate|Duplo|A taxa média de quadros de vídeo de fluxo de entrada por segundo.|
|averageOutboundBitRate|Duplo|A taxa média de bits de vídeo de fluxo de saída por segundo.|
|averageOutboundFrameRate|Duplo|A taxa média de quadros de vídeo de fluxo de saída por segundo.|

### <a name="derived-types"></a>Tipos derivados

| Tipo                                                 | Descrição                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [teleconferenceDeviceScreenSharingQuality](teleconferencedevicescreensharingquality.md)    | Dados de qualidade de compartilhamento de tela do dispositivo de teleconferência de vídeo. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.teleconferenceDeviceVideoQuality",
  "baseType": "microsoft.graph.teleconferenceDeviceMediaQuality"
}-->

```json
{
  "averageInboundBitRate": 1024,
  "averageInboundFrameRate": 1024,
  "averageInboundJitter": "String (ISO 8601 duration)",
  "averageInboundPacketLossRateInPercentage": 10,
  "averageInboundRoundTripDelay": "String (ISO 8601 duration)",
  "averageOutboundBitRate": 1024,
  "averageOutboundFrameRate": 1024,
  "averageOutboundJitter": "String (ISO 8601 duration)",
  "averageOutboundPacketLossRateInPercentage": 10,
  "averageOutboundRoundTripDelay": "String (ISO 8601 duration)",
  "channelIndex": 1,
  "inboundPackets": 1024,
  "localIPAddress": "String",
  "localPort": 2000,
  "maximumInboundJitter": "String (ISO 8601 duration)",
  "maximumInboundPacketLossRateInPercentage": 12,
  "maximumInboundRoundTripDelay": "String (ISO 8601 duration)",
  "maximumOutboundJitter": "String (ISO 8601 duration)",
  "maximumOutboundPacketLossRateInPercentage": 12,
  "maximumOutboundRoundTripDelay": "String (ISO 8601 duration)",
  "mediaDuration": "String (ISO 8601 duration)",
  "networkLinkSpeedInBytes": 1000000,
  "outboundPackets": 1024,
  "remoteIPAddress": "String",
  "remotePort": 3000
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teleconferenceDeviceVideoQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

