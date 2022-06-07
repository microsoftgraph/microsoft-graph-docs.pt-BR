---
title: Tipo de recurso mediaStream
description: O tipo mediaStream
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 180936a2a3bc36e1f7ccd9fe684439caf4531fd7
ms.sourcegitcommit: 69b150e408c0b9a0705bf33229269f6e5371bc6c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2022
ms.locfileid: "65924090"
---
# <a name="mediastream-resource-type"></a>Tipo de recurso mediaStream

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações sobre um fluxo de mídia entre dois pontos de extremidade em uma chamada.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|audioCodec|microsoft.graph.callRecords.audioCodec|Nome do codec usado para codificar áudio para transmissão na rede. Os valores possíveis são: , , , , , , , , `multiChannelAudio``g7221c``g729``g722``g7221`, . `unknownFutureValue``xmsRTA``siren``silkWide``satinFullband``silk``satin``rtAudio8``opus``rtAudio16``silkNarrow``muchv2``amrWide``pcmu``pcma``cn``invalid``unknown`|
|averageAudioDegradation|Duplo|Degradação média da pontuação de opinião média de rede para fluxo. Representa o quanto a perda de rede e tremulação afetaram a qualidade do áudio recebido.|
|averageAudioNetworkJitter|Duration|Tremulação média para o fluxo calculado conforme especificado no [RFC 3550][], indicado no [formato ISO 8601][] . Por exemplo, 1 segundo `'PT1S'`é indicado como , em que 'P' é o designador de duração, 'T' é o designador de tempo e 'S' é o segundo designador.|
|averageBandwidthEstimate|Int64|Largura de banda estimada média disponível entre dois pontos de extremidade em bits por segundo.|
|averageJitter|Duration|Tremulação média para o fluxo calculado conforme especificado no [RFC 3550][], indicado no [formato ISO 8601][] . Por exemplo, 1 segundo `'PT1S'`é indicado como , em que 'P' é o designador de duração, 'T' é o designador de tempo e 'S' é o segundo designador.|
|averagePacketLossRate|Duplo|Taxa média de perda de pacotes para fluxo.|
|averageRatioOfConcealedSamples|Duplo|Proporção do número de quadros de áudio com amostras geradas pela ocultação de perda de pacotes para o número total de quadros de áudio.|
|averageReceivedFrameRate|Duplo|Média de quadros por segundo recebidos para todos os fluxos de vídeo calculados durante a sessão.|
|averageRoundTripTime|Duration|Tempo médio de ida e volta de propagação de rede calculado conforme especificado no [RFC 3550][], indicado no [formato ISO 8601][] . Por exemplo, 1 segundo `'PT1S'`é indicado como , em que 'P' é o designador de duração, 'T' é o designador de tempo e 'S' é o segundo designador.|
|averageVideoFrameLossPercentage|Duplo|Percentual médio de quadros de vídeo perdidos conforme exibido para o usuário.|
|averageVideoFrameRate|Duplo|Média de quadros por segundo recebidos para um fluxo de vídeo, calculados durante a sessão.|
|averageVideoPacketLossRate|Duplo|Fração média de pacotes perdidos, conforme especificado no [RFC 3550][], computado durante a sessão.|
|endDateTime|DateTimeOffset|Hora UTC em que o fluxo terminou. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|lowFrameRateRatio|Duplo|Fração da chamada em que a taxa de quadros é menor que 7,5 quadros por segundo.|
|lowVideoProcessingCapabilityRatio|Duplo|Fração da chamada em que o cliente está executando menos de 70% da capacidade esperada de processamento de vídeo.|
|maxAudioNetworkJitter|Duration|Máximo de tremulação de rede de áudio computada em cada uma das janelas de 20 segundos durante a sessão, indicada no [formato ISO 8601][] . Por exemplo, 1 segundo `'PT1S'`é indicado como , em que 'P' é o designador de duração, 'T' é o designador de tempo e 'S' é o segundo designador.|
|maxJitter|Duration|Tremulação máxima para o fluxo calculado conforme especificado no RFC 3550, indicado no [formato ISO 8601][] . Por exemplo, 1 segundo `'PT1S'`é indicado como , em que 'P' é o designador de duração, 'T' é o designador de tempo e 'S' é o segundo designador.|
|maxPacketLossRate|Duplo|Taxa máxima de perda de pacotes para o fluxo.|
|maxRatioOfConcealedSamples|Duplo|Taxa máxima de pacotes ocultados pelo curador.|
|maxRoundTripTime|Duration|Tempo de ida e volta de propagação de rede máximo calculado conforme especificado no [RFC 3550][], indicado no [formato ISO 8601][] . Por exemplo, 1 segundo `'PT1S'`é indicado como , em que 'P' é o designador de duração, 'T' é o designador de tempo e 'S' é o segundo designador.|
|packetUtilization|Int64|Contagem de pacotes para o fluxo.|
|postForwardErrorCorrectionPacketLossRate|Duplo|Taxa de perda de pacotes após a agregação do FEC em todos os fluxos de vídeo e codecs.|
|startDateTime|DateTimeOffset|Hora UTC em que o fluxo foi iniciado. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|streamDirection|microsoft.graph.callRecords.mediaStreamDirection|Indica a direção do fluxo de mídia. Os valores possíveis são: `callerToCallee` e `calleeToCaller`.|
|streamId|Cadeia de caracteres|Identificador exclusivo do fluxo.|
|videoCodec|microsoft.graph.callRecords.videoCodec|Nome do codec usado para codificar vídeo para transmissão na rede. Os valores possíveis são: `unknown`, `invalid`, `av1`, `h263`, `h264`, `h264s`, `h264uc`, `h265`, `rtvc1`, `rtVideo`, `xrtvc1`, `unknownFutureValue`.|
|wasMediaBypassed|Booleano|True se o fluxo de mídia ignorar o Servidor de Mediação e ir direto entre o cliente e o Gateway PSTN/PBX, caso contrário, false.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.mediaStream",
  "baseType": null
}-->

```json
{
  "audioCodec": "String",
  "averageAudioDegradation": "Double",
  "averageAudioNetworkJitter": "String (duration)",
  "averageBandwidthEstimate": 1024,
  "averageJitter": "String (duration)",
  "averagePacketLossRate": "Double",
  "averageRatioOfConcealedSamples": "Double",
  "averageReceivedFrameRate": "Double",
  "averageRoundTripTime": "String (duration)",
  "averageVideoFrameLossPercentage": "Double",
  "averageVideoFrameRate": "Double",
  "averageVideoPacketLossRate": "Double",
  "endDateTime": "String (timestamp)",
  "lowFrameRateRatio": "Double",
  "lowVideoProcessingCapabilityRatio": "Double",
  "maxAudioNetworkJitter": "String (duration)",
  "maxJitter": "String (duration)",
  "maxPacketLossRate": "Double",
  "maxRatioOfConcealedSamples": "Double",
  "maxRoundTripTime": "String (duration)",
  "packetUtilization": 1024,
  "postForwardErrorCorrectionPacketLossRate": "Double",
  "startDateTime": "String (timestamp)",
  "streamDirection": "String",
  "streamId": "String",
  "videoCodec": "String",
  "wasMediaBypassed": true
}
```

[ISO 8601]: https://www.iso.org/iso/iso8601
[RFC 3550]: https://tools.ietf.org/html/rfc3550

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath&quot;: &quot;"
}-->

