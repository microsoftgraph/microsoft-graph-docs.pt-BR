---
title: tipo de recurso deviceInfo
description: O tipo deviceInfo
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 17ebc8d0a7ffe9a59dd5225439e90af41aaa688a
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394674"
---
# <a name="deviceinfo-resource-type"></a>tipo de recurso deviceInfo

Namespace: Microsoft. Graph. callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações sobre um dispositivo (microfone, alto-falante, câmera, etc.) usados em uma chamada.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|captureDeviceDriver|String|Nome do driver do dispositivo de captura usado pelo ponto de extremidade de mídia.|
|captureDeviceName|String|Nome do dispositivo de captura usado pelo ponto de extremidade de mídia.|
|captureNotFunctioningEventRatio|Duplo|Fração da chamada em que o ponto de extremidade de mídia detectou que o dispositivo de captura não estava funcionando corretamente.|
|cpuInsufficentEventRatio|Duplo|Fração da chamada em que o ponto de extremidade de mídia detectou que os recursos de CPU disponíveis eram insuficientes e causaram baixa qualidade do áudio enviado e recebido.|
|deviceClippingEventRatio|Duplo|Fração da chamada que o ponto de extremidade de mídia detectou o corte no áudio capturado que causou baixa qualidade do áudio que está sendo enviado.|
|deviceGlitchEventRatio|Duplo|Fração da chamada em que o ponto de extremidade de mídia detectou falhas ou intervalos no áudio reproduzido ou capturado que causou baixa qualidade do áudio enviado ou recebido.|
|howlingEventCount|Int32|Número de vezes durante a chamada em que o ponto de extremidade de mídia detectou o Howling ou o arranhão Audio.|
|initialSignalLevelRootMeanSquare|Duplo|O quadrado de raiz média (RMS) do sinal de entrada de até os primeiros 30 segundos da chamada.|
|lowSpeechLevelEventRatio|Duplo|Fração da chamada que o ponto de extremidade de mídia detectou baixo nível de fala que causou baixa qualidade do áudio que está sendo enviado.|
|lowSpeechToNoiseEventRatio|Duplo|Fração da chamada em que o ponto de extremidade de mídia detectou baixa fala no nível de ruído que causou baixa qualidade do áudio que está sendo enviado.|
|micGlitchRate|Duplo|Falhas por intervalo de 5 minutos para o microfone do ponto de extremidade de mídia.|
|receivedNoiseLevel|Int32|Nível de energia médio do áudio recebido para áudio classificado como ruído mono ou canal esquerdo de ruído estéreo pelo ponto de extremidade da mídia.|
|receivedSignalLevel|Int32|Nível de energia médio do áudio recebido para áudio classificado como fala mono ou canal esquerdo de fala estéreo pelo ponto de extremidade de mídia.|
|renderDeviceDriver|String|Nome do driver de dispositivo de renderização usado pelo ponto de extremidade de mídia.|
|renderDeviceName|String|Nome do dispositivo de renderização usado pelo ponto de extremidade de mídia.|
|renderMuteEventRatio|Duplo|Fração da chamada em que o ponto de extremidade de mídia detectou o processamento do dispositivo está com mudo ativado.|
|renderNotFunctioningEventRatio|Duplo|Fração da chamada em que o ponto de extremidade de mídia detectou que o dispositivo de renderização não estava funcionando corretamente.|
|renderZeroVolumeEventRatio|Duplo|Fração da chamada que o ponto de extremidade de mídia detectou que o volume de renderização do dispositivo está definido como 0.|
|sentNoiseLevel|Int32|Nível de energia médio do áudio enviado para áudio classificado como ruído mono ou canal esquerdo de ruído estéreo pelo ponto de extremidade da mídia.|
|sentSignalLevel|Int32|Nível de energia médio do áudio enviado para áudio classificado como fala mono ou canal esquerdo de fala estéreo pelo ponto de extremidade de mídia.|
|speakerGlitchRate|Duplo|Falhas por 5 minutos internas para o ponto de extremidade de mídia Loudspeaker.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.deviceInfo",
  "baseType": null
}-->

```json
{
  "captureDeviceDriver": "String",
  "captureDeviceName": "String",
  "captureNotFunctioningEventRatio": "Double",
  "cpuInsufficentEventRatio": "Double",
  "deviceClippingEventRatio": "Double",
  "deviceGlitchEventRatio": "Double",
  "howlingEventCount": 1024,
  "initialSignalLevelRootMeanSquare": "Double",
  "lowSpeechLevelEventRatio": "Double",
  "lowSpeechToNoiseEventRatio": "Double",
  "micGlitchRate": "Double",
  "receivedNoiseLevel": 1024,
  "receivedSignalLevel": 1024,
  "renderDeviceDriver": "String",
  "renderDeviceName": "String",
  "renderMuteEventRatio": "Double",
  "renderNotFunctioningEventRatio": "Double",
  "renderZeroVolumeEventRatio": "Double",
  "sentNoiseLevel": 1024,
  "sentSignalLevel": 1024,
  "speakerGlitchRate": "Double"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->