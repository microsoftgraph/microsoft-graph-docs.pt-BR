---
title: tipo de recurso teleconferenceDeviceMediaQuality
description: Dados de qualidade de mídia do dispositivo de teleconferência de vídeo.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a01dd135c85288fd511975cce8781912f2975f4f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046305"
---
# <a name="teleconferencedevicemediaquality-resource-type"></a>tipo de recurso teleconferenceDeviceMediaQuality

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa dados de qualidade de mídia do dispositivo de teleconferência de vídeo.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|averageInboundJitter|Duração|A tremulação média da rede de fluxo de entrada.|
|averageInboundPacketLossRateInPercentage|Duplo|A taxa média de perda de pacote de fluxo de entrada em porcentagem (0-100). Por exemplo, 0, 1 significa 0, 1%.|
|averageInboundRoundTripDelay|Duração|O intervalo médio de ida e volta da rede de fluxo de entrada.|
|averageOutboundJitter|Duração|A tremulação média da rede de fluxo de saída.|
|averageOutboundPacketLossRateInPercentage|Duplo|A taxa média de perda de pacotes de fluxo de saída em porcentagem (0-100). Por exemplo, 0, 1 significa 0, 1%.|
|averageOutboundRoundTripDelay|Duração|O intervalo médio de ida e volta da rede de fluxo de saída.|
|channelIndex|Int32|O índice de canal da mídia. A indexação começa com 1.  Se uma sessão de mídia contiver três modalidades de vídeo, os índices de canal serão 1, 2 e 3.|
|inboundPackets|Int64|O número total de pacotes de entrada.|
|localIPAddress|Cadeia de caracteres|o endereço IP local da sessão de mídia.|
|localPort|Int32|A porta de mídia local.|
|maximumInboundJitter|Duração|A tremulação máxima da rede de fluxo de entrada.|
|maximumInboundPacketLossRateInPercentage|Duplo|A taxa máxima de perda de pacote de fluxo de entrada em porcentagem (0-100). Por exemplo, 0, 1 significa 0, 1%.|
|maximumInboundRoundTripDelay|Duração|O intervalo máximo de ida e volta da rede de fluxo de entrada.|
|maximumOutboundJitter|Duração|A tremulação de rede de fluxo de saída máximo.|
|maximumOutboundPacketLossRateInPercentage|Duplo|A taxa máxima de perda de pacotes de fluxo de saída em porcentagem (0-100). Por exemplo, 0, 1 significa 0, 1%.|
|maximumOutboundRoundTripDelay|Duração|O atraso máximo de ida e volta da rede de fluxo de saída.|
|mediaDuration|Duração|A duração da modalidade total. Se a mídia habilitada e desabilitada várias vezes, MediaDuration será a soma de todas as durações.|
|networkLinkSpeedInBytes|Int64|A velocidade do link de rede em bytes|
|outboundPackets|Int64|O número total dos pacotes de saída.|
|remoteIPAddress|Cadeia de caracteres|O endereço IP remoto da sessão de mídia.|
|remotePort|Int32|A porta de mídia remota.|

### <a name="derived-types"></a>Tipos derivados

| Tipo                                                 | Descrição                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [teleconferenceDeviceAudioQuality](teleconferencedeviceaudioquality.md)    | Dados de qualidade de áudio do dispositivo de teleconferência de vídeo.                          |
| [teleconferenceDeviceVideoQuality](teleconferencedevicevideoquality.md)    | Dados de qualidade de vídeo do dispositivo de teleconferência de vídeo.                          |
| [teleconferenceDeviceScreenSharingQuality](teleconferencedevicescreensharingquality.md)    | Dados de qualidade de compartilhamento de tela do dispositivo de teleconferência de vídeo. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.teleconferenceDeviceMediaQuality",
  "baseType": null
}-->

```json
{
  "averageInboundJitter": "String (ISO 8601 duration)",
  "averageInboundPacketLossRateInPercentage": 10,
  "averageInboundRoundTripDelay": "String (ISO 8601 duration)",
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
  "description": "teleconferenceDeviceMediaQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


