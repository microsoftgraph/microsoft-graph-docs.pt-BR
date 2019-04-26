---
title: Enumeração securityNetworkProtocol
description: Valores possíveis para o protocolo de rede.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: b9b4d29bb3af7e52665c00801e5e38e9b208455b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572448"
---
# <a name="securitynetworkprotocol-enum"></a>Enumeração securityNetworkProtocol

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Valores possíveis para o protocolo de rede.

## <a name="members"></a>Membros

|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|-1|Protocolo desconhecido.|
|IP|,0|Protocolo de Internet.|
|ICMP|1 | Protocolo de mensagens de controle da Internet.|
|IGMP|2 | Protocolo de gerenciamento de grupos da Internet.|
|GGP|3 | Gateway para protocolo gateway.|
|IPv4|4 | Protocolo IP versão 4.|
|tcp|6 | Protocolo de controle de transmissão.|
|confiável|12 | Protocolo de pacote universal do PARC.|
|via|17 | Protocolo de dataGrama de usuário.|
|IDP|22| Protocolo de dataGrama da Internet.|
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/securitynetworkprotocolenumtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
