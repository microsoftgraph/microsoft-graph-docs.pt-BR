---
title: enumeração securityNetworkProtocol
description: Valores possíveis para o protocolo de rede.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: b9b4d29bb3af7e52665c00801e5e38e9b208455b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511468"
---
# <a name="securitynetworkprotocol-enum"></a>enumeração securityNetworkProtocol

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Valores possíveis para o protocolo de rede.

## <a name="members"></a>Membros

|Membro|Valor|Descrição|
|:---|:---|:---|
|unknown|-1|Protocolo desconhecido.|
|IP|.0|Protocolo de Internet.|
|ICMP|-1| Protocolo de mensagem de controle de Internet.|
|IGMP|-2| Protocolo de gerenciamento de grupos da Internet.|
|ggp|-3| Protocolo de gateway a Gateway.|
|IPv4|4*| Internet Protocol versão 4.|
|TCP|-6| Protocolo de controle de transmissão.|
|PUP|1.2| Protocolo de pacote Universal PARC.|
|UDP|1.7| Protocolo de datagrama de usuário.|
|IDP|2.2| Protocolo de datagrama de Internet.|
|IPv6|4.1| Protocolo IP versão 6 (ipv6).|
|ipv6RoutingHeader|4.3| cabeçalho de roteamento IPv6.|
|ipv6FragmentHeader|4.4| cabeçalho de fragmento IPv6.|
|ipSecEncapsulatingSecurityPayload|50%| cabeçalho de carga de segurança de encapsulamento IPv6.|
|ipSecAuthenticationHeader|5.1| cabeçalho de autenticação de IPv6.|
|icmpV6|5.8| Protocolo de mensagem de controle da Internet para ipv6.|
|ipv6NoNextHeader|5.9| IPv6 não próximo cabeçalho.|
|ipv6DestinationOptions|-60| cabeçalho de opções de destino de IPv6.|
|término|7.7| NET protocolo de disco (não oficiais).|
|Raw|255| Protocolo de pacote IP bruto.|
|protocolo IPX|-1000| Protocolo do Exchange de pacotes de Internet.|
|SPX|1256| Protocolo de intercâmbio de pacote sequenciado.|
|spxII|1257| Protocolo de versão 2 Exchange pacote sequenciado.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/securitynetworkprotocolenumtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
