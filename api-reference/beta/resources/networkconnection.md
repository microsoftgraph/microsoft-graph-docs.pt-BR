---
title: tipo de recurso networkConnection
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 9d25d78d51a39d3240d0d7566b7037f55e379fe1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811109"
---
# <a name="networkconnection-resource-type"></a>tipo de recurso networkConnection

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações de estado sobre a conexão de rede relacionada ao alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|applicationName|Cadeia de caracteres|Nome do aplicativo que gerencia a conexão de rede (por exemplo, Facebook, SMTP, etc.).|
|destinationAddress|String|Endereço IP de destino (da conexão de rede).|
|destinationDomain|String|Parte do domínio de destino da URL de destino. (por exemplo, ' www.contoso.com ').|
|destinationLocation|String|Local (por mapeamento de endereço IP) associado ao destino de uma conexão de rede.|
|destinationPort|String|Porta de destino (da conexão de rede).|
|destinationUrl|String|URL de conexão de rede/cadeia de caracteres URI-excluindo parâmetros. (por exemplo, ' www.contoso.com/products/default.htmL')|
|direction|connectionDirection|Direção da conexão de rede. Os valores possíveis são: `unknown`, `inbound`, `outbound`.|
|domainRegisteredDateTime|DateTimeOffset|Data em que o domínio de destino foi registrado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|localDnsName|String|A resolução de nome DNS local da forma como aparece no cache de DNS local do host (por exemplo, caso o arquivo "hosts" tenha sido adulterado).|
|natDestinationAddress|String|Endereço IP de destino de conversão de endereço de rede.|
|natDestinationPort|String|Porta de destino de conversão de endereço de rede.|
|natSourceAddress|String|Endereço IP de origem de conversão de endereço de rede.|
|natSourcePort|String|Porta de origem de conversão de endereço de rede.|
|RDP|securityNetworkProtocol|Protocolo de rede. Os valores possíveis são:,,,,,,,,,,,,,,,,,,,, `unknown` `ip` `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader` , `ipSecEncapsulatingSecurityPayload` , `ipSecAuthenticationHeader` ,, `icmpV6` `ipv6NoNextHeader` , `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII` ,,,,,.|
|riskScore|String|Provedor gerado/Pontuação de risco calculado da conexão de rede. O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.|
|sourceAddress|String|Endereço IP de origem (ou seja, origem) (da conexão de rede).|
|sourceLocation|String|Local (por mapeamento de endereço IP) associado à origem de uma conexão de rede.|
|sourcePort|String|Porta IP de origem (ou seja, origem) (da conexão de rede).|
|status|connectionStatus|Status da conexão de rede. Os valores possíveis são: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.|
|urlParameters|String|Parâmetros (sufixo) da URL de destino.|

### <a name="securitynetworkprotocol-values"></a>valores de securityNetworkProtocol

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|-1|Protocolo desconhecido.|
|IP|,0|Protocolo de Internet.|
|ICMP|1| Protocolo de mensagens de controle da Internet.|
|IGMP|duas| Protocolo de gerenciamento de grupos da Internet.|
|ggp|3D| Gateway para protocolo gateway.|
|IPv4|4 | Protocolo IP versão 4.|
|tcp|6 | Protocolo de controle de transmissão.|
|confiável|12 | Protocolo de pacote universal do PARC.|
|via|17 | Protocolo de datagrama de usuário.|
|IDP|22| Protocolo de datagrama da Internet.|
|IPv6|41| Protocolo IP versão 6 (IPv6).|
|ipv6RoutingHeader|43| cabeçalho de roteamento IPv6.|
|ipv6FragmentHeader|44| cabeçalho de fragmento IPv6.|
|ipSecEncapsulatingSecurityPayload|50| cabeçalho de carga de segurança de encapsulamento IPv6.|
|ipSecAuthenticationHeader|51| cabeçalho de autenticação IPv6.|
|icmpV6|58| Protocolo de mensagens de controle da Internet para IPv6.|
|ipv6NoNextHeader|59| IPv6 sem cabeçalho seguinte.|
|ipv6DestinationOptions|60| cabeçalho de opções de destino IPv6.|
|término|77| Protocolo de disco de rede (não oficial).|
|-|255| Protocolo de pacote IP bruto.|
|roteador|1000| Protocolo Internet Packet Exchange.|
|SPX|1256| Protocolo de troca de pacotes sequenciado.|
|spxII|1257| Protocolo de troca de pacotes de versão 2.|

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
  "destinationLocation": "String",
  "destinationPort": "String",
  "destinationUrl": "String",
  "direction": "String",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "string",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourceLocation": "String",
  "sourcePort": "String",
  "status": "String",
  "urlParameters": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
