---
title: Tipo de recurso networkConnection
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 2221f38c4ba8f8e71030d540985fb93f415bfa19
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722106"
---
# <a name="networkconnection-resource-type"></a>Tipo de recurso networkConnection

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações de estado sobre a conexão de rede relacionada ao alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|applicationName|Cadeia de caracteres|Nome do aplicativo que gerencia a conexão de rede (por exemplo, Facebook, SMTP etc.).|
|destinationAddress|Cadeia de caracteres|Endereço IP de destino (da conexão de rede).|
|destinationDomain|Cadeia de caracteres|Parte do domínio de destino da URL de destino. (por exemplo, 'www.contoso.com').|
|destinationLocation|Cadeia de caracteres|Local (por mapeamento de endereço IP) associado ao destino de uma conexão de rede.|
|destinationPort|Cadeia de caracteres|Porta de destino (da conexão de rede).|
|destinationUrl|Cadeia de caracteres|Cadeia de caracteres url/URI de conexão de rede - excluindo parâmetros. (por exemplo, 'www.contoso.com/products/default.html')|
|direction|connectionDirection|Direção da conexão de rede. Os valores possíveis são: `unknown`, `inbound`, `outbound`.|
|domainRegisteredDateTime|DateTimeOffset|Data em que o domínio de destino foi registrado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|localDnsName|Cadeia de caracteres|A resolução de nome DNS local como ela aparece no cache DNS local do host (por exemplo, caso o arquivo 'hosts' tenha sido adulterado).|
|natDestinationAddress|Cadeia de caracteres|Endereço de rede Endereço endereço endereço IP de destino.|
|natDestinationPort|Cadeia de caracteres|Porta de destino de conversão de endereço de rede.|
|natSourceAddress|Cadeia de caracteres|Endereço de rede Endereço endereço IP de origem.|
|natSourcePort|Cadeia de caracteres|Porta de origem de conversão de endereço de rede.|
|protocol|securityNetworkProtocol|Protocolo de rede. Os valores possíveis são: `unknown` , , , , , , , , `ip` `icmp` , `igmp` `ggp` , `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` , `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII`|
|riskScore|Cadeia de caracteres|Pontuação de risco gerada/calculada do provedor da conexão de rede. Intervalo de valores recomendado de 0 a 1, que equivale a uma porcentagem.|
|sourceAddress|Cadeia de caracteres|Endereço IP de origem (ou seja, origem) (da conexão de rede).|
|sourceLocation|Cadeia de caracteres|Local (por mapeamento de endereço IP) associado à origem de uma conexão de rede.|
|sourcePort|Cadeia de caracteres|Porta IP de origem (ou seja, origem) (da conexão de rede).|
|status|connectionStatus|Status da conexão de rede. Os valores possíveis são: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.|
|urlParameters|Cadeia de caracteres|Parâmetros (sufixo) da URL de destino.|

### <a name="securitynetworkprotocol-values"></a>valores securityNetworkProtocol

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|-1|Protocolo desconhecido.|
|ip|0|Protocolo Internet.|
|icmp|1| Protocolo de Mensagem de Controle da Internet.|
|igmp|2 | Protocolo de Gerenciamento de Grupo da Internet.|
|ggp|3 | Protocolo gateway para gateway.|
|ipv4|4 | Protocolo internet versão 4.|
|tcp|6 | Protocolo de Controle de Transmissão.|
|cachorro-do-cachorro|12 | Protocolo de Pacote Universal do PARC.|
|udp|17 | Protocolo datagram do usuário.|
|idp|22| Protocolo Datagram da Internet.|
|ipv6|41| Protocolo internet versão 6 (ipv6).|
|ipv6RoutingHeader|43| Header de roteamento ipv6.|
|ipv6FragmentHeader|44| Header de fragmento ipv6.|
|ipSecEncapsulatingSecurityPayload|50| ipv6 Encapsulando o header de Carga de Segurança.|
|ipSecAuthenticationHeader|51| Header de autenticação ipv6.|
|icmpV6|58| Protocolo de Mensagem de Controle da Internet para ipv6.|
|ipv6NoNextHeader|59| ipv6 Nenhum próximo header.|
|ipv6DestinationOptions|60| Header de Opções de Destino ipv6.|
|nd|77| Protocolo De Disco Líquido (não oficial).|
|raw|255| Protocolo de pacote IP bruto.|
|ipx|1000| Protocolo Exchange de Pacotes da Internet.|
|spx|1256| Protocolo de Exchange de Pacotes Sequenciados.|
|spxII|1257| Protocolo sequenced Packet Exchange versão 2.|

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


