---
title: tipo de recurso networkConnection
description: Contém informações de estado sobre a conexão de rede relacionada ao alerta.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 86986178bc7104118dfb4db83ae43f7780307fe6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447364"
---
# <a name="networkconnection-resource-type"></a>tipo de recurso networkConnection

Namespace: Microsoft. Graph

Contém informações de estado sobre a conexão de rede relacionada ao alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|applicationName|Cadeia de caracteres|Nome do aplicativo que gerencia a conexão de rede (por exemplo, Facebook, SMTP, etc.).|
|destinationAddress|String|Endereço IP de destino (da conexão de rede).|
|destinationDomain|String|Parte do domínio de destino da URL de destino. (por exemplo, ' www.contoso.com ').|
|destinationPort|String|Porta de destino (da conexão de rede).|
|destinationUrl|String|URL de conexão de rede/cadeia de caracteres URI-excluindo parâmetros. (por exemplo, ' www.contoso.com/products/default.html ')|
|direction|connectionDirection|Direção da conexão de rede. Os valores possíveis são: `unknown`, `inbound`, `outbound`.|
|domainRegisteredDateTime|DateTimeOffset|Data em que o domínio de destino foi registrado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|localDnsName|String|A resolução de nome DNS local da forma como aparece no cache de DNS local do host (por exemplo, caso o arquivo "hosts" tenha sido adulterado).|
|natDestinationAddress|String|Endereço IP de destino de conversão de endereço de rede.|
|natDestinationPort|String|Porta de destino de conversão de endereço de rede.|
|natSourceAddress|String|Endereço IP de origem de conversão de endereço de rede.|
|natSourcePort|String|Porta de origem de conversão de endereço de rede.|
|RDP|[securityNetworkProtocol](securitynetworkprotocol.md)|Protocolo de rede. Os valores possíveis são `unknown`: `ip`, `icmp`, `igmp`, `ggp` `ipv4` `tcp`,,, `pup`, `udp`, `idp` `ipv6` `ipv6RoutingHeader`,,, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd` `raw` `ipx` `spx`,,,, `spxII`,,,,,,,,,.|
|riskScore|String|Provedor gerado/Pontuação de risco calculado da conexão de rede. O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.|
|sourceAddress|String|Endereço IP de origem (ou seja, origem) (da conexão de rede).|
|sourcePort|String|Porta IP de origem (ou seja, origem) (da conexão de rede).|
|status|connectionStatus|Status da conexão de rede. Os valores possíveis são: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.|
|urlParameters|String|Parâmetros (sufixo) da URL de destino.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkConnection"
}-->

```json
{
  "applicationName": "String",
  "destinationAddress": "String",
  "destinationDomain": "String",
  "destinationPort": "String",
  "destinationUrl": "String",
  "direction": "@odata.type: microsoft.graph.connectionDirection",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "@odata.type: microsoft.graph.securityNetworkProtocol",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourcePort": "String",
  "status": "@odata.type: microsoft.graph.connectionStatus",
  "urlParameters": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
