---
title: tipo de recurso networkInfo
description: O tipo networkInfo
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 048b0cc3d6714286f079dc02843184809c70c617
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491967"
---
# <a name="networkinfo-resource-type"></a>tipo de recurso networkInfo

Namespace: microsoft.graph.callRecords

Representa informações sobre a rede usada em uma chamada.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|bandwidthLowEventRatio|Duplo|Fração da chamada em que o ponto de extremidade de mídia detectou que a política de largura de banda ou largura de banda disponível era baixa o suficiente para causar baixa qualidade do áudio enviado.|
|basicServiceSetIdentifier|String|O identificador do conjunto de serviços básicos de LAN sem fio do ponto de extremidade de mídia usado para se conectar à rede.|
|Connection|Microsoft. Graph. callRecords. networkConnectionType|Tipo de rede usado pelo ponto de extremidade de mídia. Os possíveis valores são: `unknown`, `wired`, `wifi`, `mobile`, `tunnel`, `unknownFutureValue`.|
|delayEventRatio|Duplo|Fração da chamada em que o ponto de extremidade de mídia detectou que o atraso de rede era suficientemente significativo para afetar a capacidade de comunicação bidirecional em tempo real.|
|dnsSuffix|String|Sufixo DNS associado ao adaptador de rede do ponto de extremidade de mídia.|
|ipAddress|Cadeia de caracteres|Endereço IP do ponto de extremidade de mídia.|
|linkSpeed|Int64|Velocidade do link em bits por segundo relatado pelo adaptador de rede usado pelo ponto de extremidade de mídia.|
|macAddress|String|O endereço MAC (controle de acesso de mídia) do dispositivo de rede do ponto de extremidade de mídia.|
|propor|Int32|Número da porta de rede usado pelo ponto de extremidade de mídia.|
|receivedQualityEventRatio|Duplo|Fração da chamada em que o ponto de extremidade de mídia detectou que a rede estava causando baixa qualidade do áudio recebido.|
|reflexiveIPAddress|String|Endereço IP do ponto de extremidade de mídia conforme visto pelo servidor de Media Relay. Em geral, esse é o endereço IP público da Internet associado ao ponto de extremidade.|
|relayIPAddress|String|Endereço IP do servidor de Media Relay alocado pelo ponto de extremidade de mídia.|
|relayPort|Int32|Número de porta de rede alocado no servidor de Media Relay pelo ponto de extremidade de mídia.|
|sentQualityEventRatio|Duplo|Fração da chamada em que o ponto de extremidade de mídia detectou que a rede estava causando baixa qualidade do áudio enviado.|
|-|String|Sub-rede usada para fluxo de mídia pelo ponto de extremidade de mídia.|
|wifiBand|Microsoft. Graph. callRecords. wifiBand|Banda WiFi usada pelo ponto de extremidade de mídia. Os valores possíveis são: `unknown`, `frequency24GHz`, `frequency50GHz`, `frequency60GHz`, `unknownFutureValue`.|
|wifiBatteryCharge|Int32|Carga da bateria restante estimada em porcentagem relatada pelo ponto de extremidade de mídia.|
|wifiChannel|Int32|O canal WiFi usado pelo ponto de extremidade de mídia.|
|wifiMicrosoftDriver|String|Nome do driver do Microsoft WiFi usado pelo ponto de extremidade de mídia. O valor pode ser localizado com base no idioma usado pelo ponto de extremidade.|
|wifiMicrosoftDriverVersion|String|Versão do driver do Microsoft WiFi usado pelo ponto de extremidade de mídia.|
|wifiRadioType|Microsoft. Graph. callRecords. wifiRadioType|Tipo de rádio WiFi usado pelo ponto de extremidade de mídia. Os valores possíveis são: `unknown`, `wifi80211a`, `wifi80211b`, `wifi80211g`, `wifi80211n`, `wifi80211ac`, `wifi80211ax`, `unknownFutureValue`.|
|wifiSignalStrength|Int32|Intensidade do sinal WiFi em porcentagem reportada pelo ponto de extremidade de mídia.|
|wifiVendorDriver|String|Nome do driver WiFi usado pelo ponto de extremidade de mídia. O valor pode ser localizado com base no idioma usado pelo ponto de extremidade.|
|wifiVendorDriverVersion|String|Versão do driver WiFi usado pelo ponto de extremidade de mídia.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.networkInfo",
  "baseType": null
}-->

```json
{
  "bandwidthLowEventRatio": "Double",
  "basicServiceSetIdentifier": "String",
  "connectionType": "String",
  "delayEventRatio": "Double",
  "dnsSuffix": "String",
  "ipAddress": "String",
  "linkSpeed": 1024,
  "macAddress": "String",
  "port": 1024,
  "receivedQualityEventRatio": "Double",
  "reflexiveIPAddress": "String",
  "relayIPAddress": "String",
  "relayPort": 1024,
  "sentQualityEventRatio": "Double",
  "subnet": "String",
  "wifiBand": "String",
  "wifiBatteryCharge": 1024,
  "wifiChannel": 1024,
  "wifiMicrosoftDriver": "String",
  "wifiMicrosoftDriverVersion": "String",
  "wifiRadioType": "String",
  "wifiSignalStrength": 1024,
  "wifiVendorDriver": "String",
  "wifiVendorDriverVersion": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->