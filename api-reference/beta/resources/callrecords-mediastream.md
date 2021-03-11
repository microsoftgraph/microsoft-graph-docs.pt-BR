---
title: Tipo de recurso mediaStream
description: O tipo mediaStream
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 69555033ddacc9244c910b5094449ca60d1a9633
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720246"
---
# <a name="mediastream-resource-type"></a>Tipo de recurso mediaStream

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações sobre um fluxo de mídia entre dois pontos de extremidade em uma chamada.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|averageAudioDegradation|Duplo|Degradação média de pontuação de opinião de rede para fluxo. Representa o quanto a perda de rede e a tremedeira afetaram a qualidade do áudio recebido.|
|averageAudioNetworkJitter|Duration|Tremido médio para o fluxo calculado conforme especificado no [RFC 3550][], indicado no [formato ISO 8601.][] Por exemplo, 1 segundo é denodo como , onde 'P' é o designador de duração, 'T' é o designador de tempo e 'S' é o `'PT1S'` segundo designador.|
|averageBandwidthEstimate|Int64|Largura de banda estimada média disponível entre dois pontos de extremidade em bits por segundo.|
|averageJitter|Duration|Tremido médio para o fluxo calculado conforme especificado no [RFC 3550][], indicado no [formato ISO 8601.][] Por exemplo, 1 segundo é denodo como , onde 'P' é o designador de duração, 'T' é o designador de tempo e 'S' é o `'PT1S'` segundo designador.|
|averagePacketLossRate|Duplo|Taxa média de perda de pacotes para fluxo.|
|averageRatioOfConcealedSamples|Duplo|Taxa do número de quadros de áudio com exemplos gerados pela ocultação de perda de pacotes para o número total de quadros de áudio.|
|averageReceivedFrameRate|Duplo|Média de quadros por segundo recebidos para todos os fluxos de vídeo calculados durante a sessão.|
|averageRoundTripTime|Duration|Tempo médio de propagação de rede calculado conforme especificado no [RFC 3550][], indicado no [formato ISO 8601.][] Por exemplo, 1 segundo é denodo como , onde 'P' é o designador de duração, 'T' é o designador de tempo e 'S' é o `'PT1S'` segundo designador.|
|averageVideoFrameLossPercentage|Duplo|Porcentagem média de quadros de vídeo perdidos conforme exibido para o usuário.|
|averageVideoFrameRate|Duplo|Quadros médios por segundo recebidos para um fluxo de vídeo, calculados durante a duração da sessão.|
|averageVideoPacketLossRate|Duplo|Fração média de pacotes perdidos, conforme especificado em [RFC 3550][], calculado durante a duração da sessão.|
|endDateTime|DateTimeOffset|Hora UTC quando o fluxo terminou. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|lowFrameRateRatio|Duplo|Fração da chamada em que a taxa de quadros é inferior a 7,5 quadros por segundo.|
|lowVideoProcessingCapabilityRatio|Duplo|Fração da chamada que o cliente está executando menos de 70% do recurso de processamento de vídeo esperado.|
|maxAudioNetworkJitter|Duration|Máximo de tremedeira de rede de áudio calculada em cada uma das janelas de 20 segundos durante a sessão, denotado no [formato ISO 8601.][] Por exemplo, 1 segundo é denodo como , onde 'P' é o designador de duração, 'T' é o designador de tempo e 'S' é o `'PT1S'` segundo designador.|
|maxJitter|Duration|Tremedeira máxima para o fluxo calculado conforme especificado no RFC 3550, indicado no [formato ISO 8601.][] Por exemplo, 1 segundo é denodo como , onde 'P' é o designador de duração, 'T' é o designador de tempo e 'S' é o `'PT1S'` segundo designador.|
|maxPacketLossRate|Duplo|Taxa máxima de perda de pacotes para o fluxo.|
|maxRatioOfConcealedSamples|Duplo|Taxa máxima de pacotes ocultos pelo curador.|
|maxRoundTripTime|Duration|Tempo máximo de propagação de rede calculado conforme especificado no [RFC 3550][], indicado no [formato ISO 8601.][] Por exemplo, 1 segundo é denodo como , onde 'P' é o designador de duração, 'T' é o designador de tempo e 'S' é o `'PT1S'` segundo designador.|
|packetUtilization|Int64|Contagem de pacotes para o fluxo.|
|postForwardErrorCorrectionPacketLossRate|Duplo|Taxa de perda de pacotes após a aplicação do FEC agregada em todos os fluxos de vídeo e codecs.|
|startDateTime|DateTimeOffset|Hora UTC quando o fluxo foi iniciado. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|streamDirection|microsoft.graph.callRecords.mediaStreamDirection|Indica a direção do fluxo de mídia. Os valores possíveis são: `callerToCallee` e `calleeToCaller`.|
|streamId|Cadeia de caracteres|Identificador exclusivo do fluxo.|
|wasMediaBypassed|Booliano|True se o fluxo de mídia ignorar o Servidor de Mediação e ir direto entre cliente e Gateway PSTN/PBX, false caso contrário.|


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

