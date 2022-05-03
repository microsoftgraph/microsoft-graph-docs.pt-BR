---
title: Tipo de recurso networkConnection
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-pc
ms.technology: microsoft-graph
author: preetikr
ms.openlocfilehash: 4e87cd2019f3dd4eeda73509857d34775017dd1b
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176824"
---
# <a name="networkconnection-resource-type"></a>Tipo de recurso networkConnection

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações com estado sobre a conexão de rede relacionada ao alerta.

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo|Descrição|
|:---------------|:--------|:----------|
|applicationName|Cadeia de caracteres|Nome do aplicativo que gerencia a conexão de rede (por exemplo, Facebook, SMTP etc.).|
|destinationAddress|Cadeia de Caracteres|Endereço IP de destino (da conexão de rede).|
|destinationDomain|Cadeia de Caracteres|Parte do domínio de destino da URL de destino. (por exemplo, 'www.contoso.com').|
|destinationLocation|Cadeia de Caracteres|Local (por mapeamento de endereço IP) associado ao destino de uma conexão de rede.|
|destinationPort|Cadeia de Caracteres|Porta de destino (da conexão de rede).|
|destinationUrl|Cadeia de Caracteres|Cadeia de caracteres de URL/URI de conexão de rede – excluindo parâmetros. (por exemplo, 'www.contoso.com/products/default.html')|
|direction|connectionDirection|Direção da conexão de rede. Os valores possíveis são: `unknown`, `inbound`, `outbound`.|
|domainRegisteredDateTime|DateTimeOffset|Data em que o domínio de destino foi registrado. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|localDnsName|Cadeia de Caracteres|A resolução de nome DNS local como ela aparece no cache DNS local do host (por exemplo, caso o arquivo 'hosts' tenha sido adulterado).|
|natDestinationAddress|Cadeia de Caracteres|Endereço IP de destino da Conversão de Endereços de Rede.|
|natDestinationPort|Cadeia de Caracteres|Porta de destino da Conversão de Endereços de Rede.|
|natSourceAddress|Cadeia de Caracteres|Endereço IP de origem da Conversão de Endereços de Rede.|
|natSourcePort|Cadeia de Caracteres|Porta de origem da Conversão de Endereços de Rede.|
|Protocolo|securityNetworkProtocol|Protocolo de rede. Os valores possíveis são: , , , , , , , , `ipv6``udp``idp``tcp``pup`, . `spxII``spx``ipx``raw``ipSecAuthenticationHeader``ipv6DestinationOptions``ipSecEncapsulatingSecurityPayload``icmpV6``ipv6FragmentHeader``ipv6NoNextHeader``nd``ipv6RoutingHeader``ipv4``ggp``igmp``icmp``ip``unknown`|
|riskScore|Cadeia de Caracteres|Pontuação de risco gerada/calculada pelo provedor da conexão de rede. Intervalo de valor recomendado de 0 a 1, que equivale a um percentual.|
|sourceAddress|Cadeia de Caracteres|Endereço IP de origem (ou seja, origem) (da conexão de rede).|
|Sourcelocation|Cadeia de Caracteres|Local (por mapeamento de endereço IP) associado à origem de uma conexão de rede.|
|sourcePort|Cadeia de Caracteres|Porta IP de origem (ou seja, origem) (da conexão de rede).|
|status|connectionStatus|Status da conexão de rede. Os valores possíveis são: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.|
|urlParameters|Cadeia de Caracteres|Parâmetros (sufixo) da URL de destino.|

### <a name="securitynetworkprotocol-values"></a>valores securityNetworkProtocol

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|-1|Protocolo desconhecido.|
|Ip|0|Protocolo de Internet.|
|Icmp|1| Protocolo de Mensagem de Controle da Internet.|
|Igmp|2| Protocolo de Gerenciamento de Grupo da Internet.|
|Ggp|3| Protocolo gateway para gateway.|
|ipv4|4| Protocolo de Internet versão 4.|
|tcp|6 | Protocolo de Controle de Transmissão.|
|Cachorro|12 | Protocolo parc de pacote universal.|
|Udp|17 | Protocolo de datagrama do usuário.|
|Idp|22| Protocolo de datagrama da Internet.|
|ipv6|41| Protocolo de Internet versão 6 (ipv6).|
|ipv6RoutingHeader|43| Cabeçalho de roteamento ipv6.|
|ipv6FragmentHeader|44| Cabeçalho de fragmento ipv6.|
|ipSecEncapsulatingSecurityPayload|50| ipv6 Encapsulando o cabeçalho de carga de segurança.|
|ipSecAuthenticationHeader|51| Cabeçalho de autenticação ipv6.|
|icmpV6|58| Protocolo de Mensagem de Controle da Internet para ipv6.|
|ipv6NoNextHeader|59| ipv6 Nenhum cabeçalho seguinte.|
|ipv6DestinationOptions|60| Cabeçalho opções de destino ipv6.|
|Nd|77| Net Disk Protocol (não oficial).|
|Raw|255| Protocolo de pacote IP bruto.|
|Ipx|1.000| Protocolo de Exchange Internet.|
|Spx|1256| Protocolo Exchange pacote sequenciado.|
|spxII|1257| Protocolo Exchange versão 2 do Pacote Sequenciado.|

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


