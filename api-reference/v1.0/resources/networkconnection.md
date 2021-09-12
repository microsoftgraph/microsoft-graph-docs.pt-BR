---
title: Tipo de recurso networkConnection
description: Contém informações de estado sobre a conexão de rede relacionada ao alerta.
ms.localizationpriority: medium
author: chinguyen1
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: edddb2f14458a0c4afd60465c687f618937f43e8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59006911"
---
# <a name="networkconnection-resource-type"></a>Tipo de recurso networkConnection

Namespace: microsoft.graph

Contém informações de estado sobre a conexão de rede relacionada ao alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|applicationName|Cadeia de caracteres|Nome do aplicativo que gerencia a conexão de rede (por exemplo, Facebook ou SMTP).|
|destinationAddress|Cadeia de caracteres|Endereço IP de destino (da conexão de rede).|
|destinationLocation|String|Local (por mapeamento de endereço IP) associado ao destino de uma conexão de rede.|
|destinationDomain|Cadeia de caracteres|Parte do domínio de destino da URL de destino. (por exemplo, 'www.contoso.com').|
|destinationPort|Cadeia de caracteres|Porta de destino (da conexão de rede).|
|destinationUrl|Cadeia de caracteres|Cadeia de caracteres url/URI de conexão de rede - excluindo parâmetros. (por exemplo, 'www.contoso.com/products/default.html')|
|direction|connectionDirection|Direção da conexão de rede. Os valores possíveis são: `unknown`, `inbound`, `outbound`.|
|domainRegisteredDateTime|DateTimeOffset|Data em que o domínio de destino foi registrado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|localDnsName|String|A resolução de nome DNS local como ela aparece no cache DNS local do host (por exemplo, caso o arquivo 'hosts' tenha sido adulterado).|
|natDestinationAddress|String|Endereço de rede Endereço endereço endereço IP de destino.|
|natDestinationPort|String|Porta de destino de conversão de endereço de rede.|
|natSourceAddress|Cadeia de caracteres|Endereço de rede Endereço endereço IP de origem.|
|natSourcePort|String|Porta de origem de conversão de endereço de rede.|
|protocol|[securityNetworkProtocol](securitynetworkprotocol.md)|Protocolo de rede. Os valores possíveis são: `unknown` , , , , , , , , `ip` `icmp` , `igmp` `ggp` , `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` , `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII`|
|riskScore|Cadeia de caracteres|Pontuação de risco gerada/calculada do provedor da conexão de rede. Intervalo de valores recomendado de 0 a 1, que equivale a uma porcentagem.|
|sourceAddress|String|Endereço IP de origem (ou seja, origem) (da conexão de rede).|
|sourceLocation|String|Local (por mapeamento de endereço IP) associado à origem de uma conexão de rede.|
|sourcePort|String|Porta IP de origem (ou seja, origem) (da conexão de rede).|
|status|connectionStatus|Status da conexão de rede. Os valores possíveis são: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.|
|urlParameters|Cadeia de caracteres|Parâmetros (sufixo) da URL de destino.|

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
  "destinationLocation": "String",
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
  "sourceLocation": "String",
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

