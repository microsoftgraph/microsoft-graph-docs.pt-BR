---
title: tipo de recurso mediaStream
description: O tipo mediaStream
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0c75b49c25f0344fa64d56493523c0828d9794a8
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394669"
---
# <a name="mediastream-resource-type"></a>tipo de recurso mediaStream

Namespace: Microsoft. Graph. callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações sobre um fluxo de mídia entre dois pontos de extremidade em uma chamada.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|averageAudioDegradation|Duplo|Média da redução da pontuação média de opinião de rede para o Stream. Representa o quanto a perda e a tremulação da rede impactaram a qualidade do áudio recebido.|
|averageAudioNetworkJitter|Duração|Variação média do fluxo calculado conforme especificado em [RFC 3550][], indicado no formato [ISO 8601][] . Por exemplo, 1 segundo é indicado como `'PT1S'`, em que ' P ' é o designador de duração, ' T' é o designador de tempo e ' é o segundo designador.|
|averageBandwidthEstimate|Int64|Largura de banda estimada média disponível entre dois pontos de extremidade em bits por segundo.|
|averageJitter|Duração|Variação média do fluxo calculado conforme especificado em [RFC 3550][], indicado no formato [ISO 8601][] . Por exemplo, 1 segundo é indicado como `'PT1S'`, em que ' P ' é o designador de duração, ' T' é o designador de tempo e ' é o segundo designador.|
|averagePacketLossRate|Duplo|Taxa média de perda de pacotes para Stream.|
|averageRatioOfConcealedSamples|Duplo|Taxa do número de quadros de áudio com amostras geradas por ocultação de perda de pacotes para o número total de quadros de áudio.|
|averageReceivedFrameRate|Duplo|Média de quadros por segundo recebidos para todos os fluxos de vídeo calculados durante a sessão.|
|averageRoundTripTime|Duração|Tempo médio de ida e volta da propagação de rede calculado conforme especificado na [RFC 3550][], indicado no formato [ISO 8601][] . Por exemplo, 1 segundo é indicado como `'PT1S'`, em que ' P ' é o designador de duração, ' T' é o designador de tempo e ' é o segundo designador.|
|averageVideoFrameLossPercentage|Duplo|Porcentagem média de quadros de vídeo perdidos, conforme exibido para o usuário.|
|averageVideoFrameRate|Duplo|Média de quadros por segundo recebidos para um fluxo de vídeo, calculado sobre a duração da sessão.|
|averageVideoPacketLossRate|Duplo|Fração média de pacotes perdidos, conforme especificado em [RFC 3550][], calculado durante a sessão.|
|endDateTime|DateTimeOffset|Hora UTC em que o Stream terminou. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|lowFrameRateRatio|Duplo|Fração da chamada em que a taxa de quadros é menor que 7,5 quadros por segundo.|
|lowVideoProcessingCapabilityRatio|Duplo|Fração da chamada em que o cliente está executando menos de 70% da capacidade de processamento de vídeo esperada.|
|maxAudioNetworkJitter|Duração|Máximo de tremulação de rede de áudio calculada sobre cada uma das 20 segundos janelas durante a sessão, indicada no formato [ISO 8601][] . Por exemplo, 1 segundo é indicado como `'PT1S'`, em que ' P ' é o designador de duração, ' T' é o designador de tempo e ' é o segundo designador.|
|maxJitter|Duração|Variação máxima do Stream computada conforme especificado em RFC 3550, indicado no formato [ISO 8601][] . Por exemplo, 1 segundo é indicado como `'PT1S'`, em que ' P ' é o designador de duração, ' T' é o designador de tempo e ' é o segundo designador.|
|maxPacketLossRate|Duplo|Taxa máxima de perda de pacotes para o fluxo.|
|maxRatioOfConcealedSamples|Duplo|Taxa máxima de pacotes ocultos pelo reparo.|
|maxRoundTripTime|Duração|Tempo máximo de ida e volta da propagação de rede calculado conforme especificado na [RFC 3550][], indicado no formato [ISO 8601][] . Por exemplo, 1 segundo é indicado como `'PT1S'`, em que ' P ' é o designador de duração, ' T' é o designador de tempo e ' é o segundo designador.|
|packetUtilization|Int64|Contagem de pacotes para o Stream.|
|postForwardErrorCorrectionPacketLossRate|Duplo|Taxa de perda de pacotes após o FEC ter sido aplicado em todos os fluxos de vídeo e codecs.|
|startDateTime|DateTimeOffset|Hora UTC quando o fluxo é iniciado. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|streamDirection|String|Indica a direção do fluxo de mídia. Os valores possíveis são: `callerToCallee` e `calleeToCaller`.|
|streamid|String|Identificador exclusivo do Stream.|
|wasMediaBypassed|Boolean|True se o fluxo de mídia ignorar o servidor de mediação e passou diretamente entre o cliente e gateway PSTN/PBX; caso contrário, false.|


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
  "tocPath": ""
}-->