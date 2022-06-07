---
title: Tipo de recurso networkInfo
description: Representa informações sobre a rede usada em uma chamada.
ms.localizationpriority: medium
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d43b60399f1d94266c6d0ab7c2ca9c6ac4484b01
ms.sourcegitcommit: 69b150e408c0b9a0705bf33229269f6e5371bc6c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/07/2022
ms.locfileid: "65924069"
---
# <a name="networkinfo-resource-type"></a>Tipo de recurso networkInfo

Namespace: microsoft.graph.callRecords

Representa informações sobre a rede usada em uma chamada.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|bandwidthLowEventRatio|Duplo|Fração da chamada em que o ponto de extremidade de mídia detectou que a largura de banda ou a política de largura de banda disponível era baixa o suficiente para causar baixa qualidade do áudio enviado.|
|basicServiceSetIdentifier|Cadeia de caracteres|O identificador do conjunto de serviços básico de LAN sem fio do ponto de extremidade de mídia usado para se conectar à rede.|
|Connectiontype|microsoft.graph.callRecords.networkConnectionType|Tipo de rede usado pelo ponto de extremidade de mídia. Os possíveis valores são: `unknown`, `wired`, `wifi`, `mobile`, `tunnel`, `unknownFutureValue`.|
|delayEventRatio|Duplo|Fração da chamada em que o ponto de extremidade de mídia detectou que o atraso de rede foi significativo o suficiente para afetar a capacidade de comunicação bidirecional em tempo real.|
|Dnssuffix|String|Sufixo DNS associado ao adaptador de rede do ponto de extremidade de mídia.|
|ipAddress|Cadeia de caracteres|Endereço IP do ponto de extremidade de mídia.|
|linkSpeed|Int64|Velocidade de vínculo em bits por segundo relatada pelo adaptador de rede usado pelo ponto de extremidade de mídia.|
|macAddress|Cadeia de caracteres|O endereço MAC (controle de acesso de mídia) do dispositivo de rede do ponto de extremidade de mídia.|
|networkTransportProtocol|microsoft.graph.callRecords.networkTransportProtocol|Protocolo de rede usado para a transmissão de fluxo. Os valores possíveis são: `unknown`, `udp`, `tcp`, `unknownFutureValue`.|
|Porta|Int32|Número da porta de rede usado pelo ponto de extremidade de mídia.|
|receivedQualityEventRatio|Duplo|Fração da chamada que o ponto de extremidade de mídia detectou que a rede estava causando baixa qualidade do áudio recebido.|
|reflexiveIPAddress|Cadeia de caracteres|Endereço IP do ponto de extremidade de mídia, conforme visto pelo servidor de retransmissão de mídia. Normalmente, esse é o endereço IP da Internet público associado ao ponto de extremidade.|
|relayIPAddress|Cadeia de caracteres|Endereço IP do servidor de retransmissão de mídia alocado pelo ponto de extremidade de mídia.|
|relayPort|Int32|Número da porta de rede alocada no servidor de retransmissão de mídia pelo ponto de extremidade de mídia.|
|sentQualityEventRatio|Duplo|Fração da chamada que o ponto de extremidade de mídia detectou que a rede estava causando baixa qualidade do áudio enviado.|
|Sub-rede|Cadeia de caracteres|Sub-rede usada para fluxo de mídia pelo ponto de extremidade de mídia.|
|traceRouteHops|[coleção microsoft.graph.callRecords.traceRouteHop](callrecords-traceroutehop.md)|Lista de saltos de rota de rastreamento de rede coletados para esse fluxo de mídia.|
|wifiBand|microsoft.graph.callRecords.wifiBand|Banda WiFi usada pelo ponto de extremidade de mídia. Os valores possíveis são: `unknown`, `frequency24GHz`, `frequency50GHz`, `frequency60GHz`, `unknownFutureValue`.|
|wifiBatteryCharge|Int32|Carga de bateria restante estimada em porcentagem relatada pelo ponto de extremidade de mídia.|
|wifiChannel|Int32|Canal WiFi usado pelo ponto de extremidade de mídia.|
|wifiMicrosoftDriver|Cadeia de caracteres|Nome do driver Do Microsoft WiFi usado pelo ponto de extremidade de mídia. O valor pode ser localizado com base no idioma usado pelo ponto de extremidade.|
|wifiMicrosoftDriverVersion|String|Versão do driver Do Microsoft WiFi usado pelo ponto de extremidade de mídia.|
|wifiRadioType|microsoft.graph.callRecords.wifiRadioType|Tipo de rádio WiFi usado pelo ponto de extremidade de mídia. Os valores possíveis são: `unknown`, `wifi80211a`, `wifi80211b`, `wifi80211g`, `wifi80211n`, `wifi80211ac`, `wifi80211ax`, `unknownFutureValue`.|
|wifiSignalStrength|Int32|Intensidade do sinal WiFi em porcentagem relatada pelo ponto de extremidade de mídia.|
|wifiVendorDriver|Cadeia de caracteres|Nome do driver WiFi usado pelo ponto de extremidade de mídia. O valor pode ser localizado com base no idioma usado pelo ponto de extremidade.|
|wifiVendorDriverVersion|Cadeia de caracteres|Versão do driver WiFi usado pelo ponto de extremidade de mídia.|

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
  "linkSpeed": "Int64",
  "macAddress": "String",
  "networkTransportProtocol": "String",
  "port": "Int32",
  "receivedQualityEventRatio": "Double",
  "reflexiveIPAddress": "String",
  "relayIPAddress": "String",
  "relayPort": "Int32",
  "sentQualityEventRatio": "Double",
  "subnet": "String",
  "traceRouteHops": [{"@odata.type": "microsoft.graph.callRecords.traceRouteHop"}],
  "wifiBand": "String",
  "wifiBatteryCharge": "Int32",
  "wifiChannel": "Int32",
  "wifiMicrosoftDriver": "String",
  "wifiMicrosoftDriverVersion": "String",
  "wifiRadioType": "String",
  "wifiSignalStrength": "Int32",
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
