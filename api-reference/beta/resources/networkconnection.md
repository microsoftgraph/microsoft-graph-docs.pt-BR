---
title: tipo de recurso networkConnection
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: a20520a729076c7e63079c6dfc803659ace45b9d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880056"
---
# <a name="networkconnection-resource-type"></a>tipo de recurso networkConnection

 > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Contém informações com informações de estado sobre a conexão de rede relacionado ao alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|applicationName|Cadeia de caracteres|Nome do aplicativo de gerenciamento de conexão de rede (por exemplo, Facebook, SMTP, etc.).|
|destinationAddress|Cadeia de caracteres|Endereço IP de destino (da conexão de rede).|
|destinationDomain|Cadeia de caracteres|Parte do domínio de destino da URL de destino. (por exemplo 'www.contoso.com').|
|destinationPort|Cadeia de caracteres|Porta de destino (da conexão de rede).|
|destinationUrl|Cadeia de caracteres|Cadeia de caracteres de URL/URI de conexão - excluindo os parâmetros de rede. (por exemplo, 'www.contoso.com/products/default.html')|
|direção|connectionDirection|Direção da conexão de rede. Os valores possíveis são: `unknown`, `inbound`, `outbound`.|
|domainRegisteredDateTime|DateTimeOffset|Data quando o domínio de destino foi registrado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|localDnsName|Cadeia de caracteres|O local a resolução de nomes DNS como ele aparece no cache DNS local do host (por exemplo, caso o arquivo 'hosts' foi violado).|
|natDestinationAddress|Cadeia de caracteres|Endereço IP de destino de conversão de endereço de rede.|
|natDestinationPort|Cadeia de caracteres|Porta de destino de conversão de endereço de rede.|
|natSourceAddress|Cadeia de caracteres|Endereço IP de origem de conversão de endereço de rede.|
|natSourcePort|Cadeia de caracteres|Porta de origem da conversão de endereço de rede.|
|protocolo|[securityNetworkProtocol](securitynetworkprotocolenumtype.md)|Protocolo de rede. Os valores possíveis são: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd` , `raw`, `ipx`, `spx`, `spxII`.|
|riskScore|Cadeia de caracteres|Provedor gerado/calculado o risco de pontuação de conexão de rede. Valor recomendado o intervalo de 0-1, que é igual a um percentual.|
|Endereço_da_origem|Cadeia de caracteres|Endereço IP de origem (isto é, origem) (da conexão de rede).|
|Porta_da_origem|Cadeia de caracteres|Porta de IP de origem (isto é, origem) (da conexão de rede).|
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
