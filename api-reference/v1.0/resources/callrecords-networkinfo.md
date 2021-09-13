---
title: Tipo de recurso networkInfo
description: O tipo networkInfo
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e5f3115b5f450c3998ffb93f8b843dcc80e9f6d9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59029154"
---
# <a name="networkinfo-resource-type"></a>Tipo de recurso networkInfo

Namespace: microsoft.graph.callRecords

Representa informações sobre a rede usada em uma chamada.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|bandwidthLowEventRatio|Duplo|Fração da chamada que o ponto de extremidade de mídia detectou a largura de banda ou a política de largura de banda disponível foi baixa o suficiente para causar má qualidade do áudio enviado.|
|basicServiceSetIdentifier|Cadeia de caracteres|O identificador do conjunto de serviços básicos de LAN sem fio do ponto de extremidade de mídia usado para se conectar à rede.|
|connectionType|microsoft.graph.callRecords.networkConnectionType|Tipo de rede usada pelo ponto de extremidade de mídia. Os possíveis valores são: `unknown`, `wired`, `wifi`, `mobile`, `tunnel`, `unknownFutureValue`.|
|delayEventRatio|Duplo|Fração da chamada que o ponto de extremidade de mídia detectou o atraso da rede foi significativa o suficiente para afetar a capacidade de ter uma comunicação de duas vias em tempo real.|
|dnsSuffix|Cadeia de caracteres|Sufixo DNS associado ao adaptador de rede do ponto de extremidade de mídia.|
|ipAddress|Cadeia de caracteres|Endereço IP do ponto de extremidade de mídia.|
|linkSpeed|Int64|Velocidade do link em bits por segundo relatado pelo adaptador de rede usado pelo ponto de extremidade de mídia.|
|macAddress|String|O endereço MAC (controle de acesso de mídia) do dispositivo de rede do ponto de extremidade de mídia.|
|port|Int32|Número da porta de rede usado pelo ponto de extremidade de mídia.|
|receivedQualityEventRatio|Duplo|Fração da chamada que o ponto de extremidade de mídia detectou na rede estava causando má qualidade do áudio recebido.|
|reflexiveIPAddress|Cadeia de caracteres|Endereço IP do ponto de extremidade de mídia, conforme visto pelo servidor de retransmissão de mídia. Normalmente, esse é o endereço IP da Internet público associado ao ponto de extremidade.|
|relayIPAddress|String|Endereço IP do servidor de retransmissão de mídia alocado pelo ponto de extremidade de mídia.|
|relayPort|Int32|Número da porta de rede alocado no servidor de retransmissão de mídia pelo ponto de extremidade de mídia.|
|sentQualityEventRatio|Duplo|Fração da chamada que o ponto de extremidade de mídia detectou na rede estava causando má qualidade do áudio enviado.|
|sub-rede|String|Sub-rede usada para fluxo de mídia pelo ponto de extremidade de mídia.|
|wifiBand|microsoft.graph.callRecords.wifiBand|Banda WiFi usada pelo ponto de extremidade de mídia. Os valores possíveis são: `unknown`, `frequency24GHz`, `frequency50GHz`, `frequency60GHz`, `unknownFutureValue`.|
|wifiBatteryCharge|Int32|Carga de bateria restante estimada em porcentagem relatada pelo ponto de extremidade de mídia.|
|wifiChannel|Int32|Canal WiFi usado pelo ponto de extremidade de mídia.|
|wifiMicrosoftDriver|String|Nome do driver Do Microsoft WiFi usado pelo ponto de extremidade de mídia. O valor pode ser localizado com base no idioma usado pelo ponto de extremidade.|
|wifiMicrosoftDriverVersion|Cadeia de caracteres|Versão do driver Do Microsoft WiFi usado pelo ponto de extremidade de mídia.|
|wifiRadioType|microsoft.graph.callRecords.wifiRadioType|Tipo de rádio WiFi usado pelo ponto de extremidade de mídia. Os valores possíveis são: `unknown`, `wifi80211a`, `wifi80211b`, `wifi80211g`, `wifi80211n`, `wifi80211ac`, `wifi80211ax`, `unknownFutureValue`.|
|wifiSignalStrength|Int32|Força do sinal WiFi em porcentagem relatada pelo ponto de extremidade de mídia.|
|wifiVendorDriver|Cadeia de caracteres|Nome do driver WiFi usado pelo ponto de extremidade de mídia. O valor pode ser localizado com base no idioma usado pelo ponto de extremidade.|
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
