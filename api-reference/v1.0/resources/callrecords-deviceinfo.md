---
title: Tipo de recurso deviceInfo
description: O tipo deviceInfo
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cc7482cb7ac1f6f096650db64ae340b273b5aec3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084668"
---
# <a name="deviceinfo-resource-type"></a>Tipo de recurso deviceInfo

Namespace: microsoft.graph.callRecords

Representa informações sobre um dispositivo (microfone, alto-falante, câmera etc.) usado em uma chamada.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|captureDeviceDriver|Cadeia de caracteres|Nome do driver do dispositivo de captura usado pelo ponto de extremidade de mídia.|
|captureDeviceName|String|Nome do dispositivo de captura usado pelo ponto de extremidade de mídia.|
|captureNotFunctioningEventRatio|Duplo|Fração da chamada que o ponto de extremidade de mídia detectou o dispositivo de captura não estava funcionando corretamente.|
|cpuInsufficentEventRatio|Duplo|Fração da chamada que o ponto de extremidade de mídia detectou os recursos de CPU disponíveis eram insuficientes e causavam uma qualidade ruim do áudio enviado e recebido.|
|deviceClippingEventRatio|Duplo|Fração da chamada que o ponto de extremidade de mídia detectou recorte no áudio capturado que causou má qualidade do áudio que está sendo enviado.|
|deviceGlitchEventRatio|Duplo|Fração da chamada que o ponto de extremidade de mídia detectou falhas ou lacunas no áudio tocado ou capturado que causava má qualidade do áudio que está sendo enviado ou recebido.|
|howlingEventCount|Int32|Número de vezes durante a chamada em que o ponto de extremidade de mídia detectou o som de esgrimação ou redução.|
|initialSignalLevelRootMeanSquare|Duplo|O quadrado da média raiz (RMS) do sinal de entrada de até os primeiros 30 segundos da chamada.|
|lowSpeechLevelEventRatio|Duplo|Fração da chamada que o ponto de extremidade de mídia detectou baixo nível de fala que causava má qualidade do áudio que está sendo enviado.|
|lowSpeechToNoiseEventRatio|Duplo|Fração da chamada que o ponto de extremidade de mídia detectou baixo nível de fala para nível de ruído que causava má qualidade do áudio que está sendo enviado.|
|micGlitchRate|Duplo|Falhas por intervalo de 5 minutos para o microfone do ponto de extremidade de mídia.|
|receivedNoiseLevel|Int32|Nível médio de energia do áudio recebido para áudio classificado como ruído mono ou canal esquerdo de ruído estéreo pelo ponto de extremidade de mídia.|
|receivedSignalLevel|Int32|Nível médio de energia do áudio recebido para áudio classificado como fala mono ou canal esquerdo de fala estéreo pelo ponto de extremidade de mídia.|
|renderDeviceDriver|Cadeia de caracteres|Nome do driver de dispositivo de renderização usado pelo ponto de extremidade de mídia.|
|renderDeviceName|Cadeia de caracteres|Nome do dispositivo de renderização usado pelo ponto de extremidade de mídia.|
|renderMuteEventRatio|Duplo|Fração da chamada em que o ponto de extremidade de mídia detectou a renderização do dispositivo é silenciada.|
|renderNotFunctioningEventRatio|Duplo|Fração da chamada que o ponto de extremidade de mídia detectou o dispositivo de renderização não estava funcionando corretamente.|
|renderZeroVolumeEventRatio|Duplo|Fração da chamada que o volume de renderização do dispositivo detectado do ponto de extremidade de mídia está definida como 0.|
|sentNoiseLevel|Int32|Nível médio de energia do áudio enviado para áudio classificado como ruído mono ou canal esquerdo de ruído estéreo pelo ponto de extremidade de mídia.|
|sentSignalLevel|Int32|Nível médio de energia de áudio enviado para áudio classificado como fala mono ou canal esquerdo de fala estéreo pelo ponto de extremidade de mídia.|
|speakerGlitchRate|Duplo|Falhas por 5 minutos internas para o alto-falante do ponto de extremidade de mídia.|


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
