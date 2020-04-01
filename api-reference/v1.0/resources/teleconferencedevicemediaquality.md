---
title: tipo de recurso teleconferenceDeviceMediaQuality
description: Dados de qualidade de mídia do dispositivo de teleconferência de vídeo.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: faf9c5c7aca7da0e54f9d7b50899a5340b142a1b
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082704"
---
# <a name="teleconferencedevicemediaquality-resource-type"></a>tipo de recurso teleconferenceDeviceMediaQuality

Namespace: microsoft.graph

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
|localIPAddress|String|o endereço IP local da sessão de mídia.|
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
|remoteIPAddress|String|O endereço IP remoto da sessão de mídia.|
|remotePort|Int32|A porta de mídia remota.|

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
