---
title: Tipo de recurso teleconferenceDeviceMediaQuality
description: Dados de qualidade de mídia de dispositivo de teleconferência de vídeo.
ms.localizationpriority: medium
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 45ca9d4bdc34077ea19bdcbac866495a198ea5ab
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59128127"
---
# <a name="teleconferencedevicemediaquality-resource-type"></a>Tipo de recurso teleconferenceDeviceMediaQuality

Namespace: microsoft.graph

Representa dados de qualidade de mídia de dispositivo de teleconferência de vídeo.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|averageInboundJitter|Duration|O treme de rede de fluxo de entrada médio.|
|averageInboundPacketLossRateInPercentage|Duplo|A taxa média de perda de pacotes de fluxo de entrada em porcentagem (0-100). Por exemplo, 0,01 significa 0,01%.|
|averageInboundRoundTripDelay|Duration|O atraso médio da viagem de ida e volta da rede de fluxo de entrada.|
|averageOutboundJitter|Duration|O treme de rede de fluxo de saída médio.|
|averageOutboundPacketLossRateInPercentage|Duplo|A taxa média de perda de pacotes de fluxo de saída em porcentagem (0-100). Por exemplo, 0,01 significa 0,01%.|
|averageOutboundRoundTripDelay|Duration|O atraso médio da viagem de ida e volta da rede de fluxo de saída.|
|channelIndex|Int32|O índice de canal de mídia. A indexação começa com 1.  Se uma sessão de mídia contiver 3 modalidades de vídeo, os índices de canal serão 1, 2 e 3.|
|inboundPackets|Int64|O número total dos pacotes de entrada.|
|localIPAddress|Cadeia de caracteres|o endereço IP local da sessão de mídia.|
|localPort|Int32|A porta de mídia local.|
|maximumInboundJitter|Duration|O treme de rede de fluxo de entrada máximo.|
|maximumInboundPacketLossRateInPercentage|Duplo|A taxa máxima de perda de pacotes de fluxo de entrada em porcentagem (0-100). Por exemplo, 0,01 significa 0,01%.|
|maximumInboundRoundTripDelay|Duration|O atraso máximo de ida e volta da rede de fluxo de entrada.|
|maximumOutboundJitter|Duration|O treme de rede de fluxo de saída máximo.|
|maximumOutboundPacketLossRateInPercentage|Duplo|A taxa máxima de perda de pacotes de fluxo de saída em porcentagem (0-100). Por exemplo, 0,01 significa 0,01%.|
|maximumOutboundRoundTripDelay|Duration|O atraso máximo da viagem de ida e volta de fluxo de saída.|
|mediaDuration|Duration|A duração total da modalidade. Se a mídia estiver habilitada e desabilitada várias vezes, MediaDuration será a soma de todas as durações.|
|networkLinkSpeedInBytes|Int64|A velocidade do link de rede em bytes|
|outboundPackets|Int64|O número total dos pacotes de saída.|
|remoteIPAddress|Cadeia de caracteres|O endereço IP remoto da sessão de mídia.|
|remotePort|Int32|A porta de mídia remota.|

### <a name="derived-types"></a>Tipos derivados

| Tipo                                                 | Descrição                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [teleconferenceDeviceAudioQuality](teleconferencedeviceaudioquality.md)    | Dados de qualidade de áudio do dispositivo de teleconferência de vídeo.                          |
| [teleconferenceDeviceVideoQuality](teleconferencedevicevideoquality.md)    | Dados de qualidade de vídeo de dispositivo de teleconferência de vídeo.                          |
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

