---
title: tipo de recurso windowsFirewallRule
description: Uma regra que controla o tráfego por meio do firewall do Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2f4191edfee5148094f10b7a57bb50844d3bfcca
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994115"
---
# <a name="windowsfirewallrule-resource-type"></a>tipo de recurso windowsFirewallRule

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma regra que controla o tráfego por meio do firewall do Windows.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição da regra. Não precisa ser exclusivo.|
|descrição|String|A descrição da regra.|
|packageFamilyName|String|O nome da família de pacotes de um aplicativo da Microsoft Store que é afetado pela regra de firewall.|
|filePath|String|O caminho completo do arquivo de um aplicativo afetado pela regra de firewall.|
|serviceName|String|O nome usado em casos em que um serviço, não um aplicativo, está enviando ou recebendo tráfego.|
|RDP|Int32|0-255 número que representa o protocolo IP (TCP = 6, UDP = 17). Se não for especificado, o padrão é ALL. Valores válidos de 0 a 255|
|localPortRanges|Coleção de cadeias de caracteres|Lista de intervalos de porta locais. Por exemplo, "100-120", "200", "300-320". Se não for especificado, o padrão é ALL.|
|remotePortRanges|Coleção de cadeias de caracteres|Lista de intervalos de portas remotas. Por exemplo, "100-120", "200", "300-320". Se não for especificado, o padrão é ALL.|
|localAddressRanges|Coleção de cadeias de caracteres|Lista de endereços locais cobertos pela regra. Os tokens válidos incluem:
- "*" indica qualquer endereço local. Se presente, este deve ser o único token incluído.
- Uma sub-rede pode ser especificada usando a máscara de sub-rede ou a notação de prefixo de rede. Se nenhuma máscara de sub-rede ou prefixo de rede for especificado, a máscara de sub-rede padrão será 255.255.255.255.
- Um endereço IPv6 válido.
- Um intervalo de endereços IPv4 no formato "Iniciar endereço-end endereço" sem espaços incluídos.
- Um intervalo de endereços IPv6 no formato "Iniciar endereço-end endereço" sem espaços incluídos.
O padrão é qualquer endereço. | | remoteAddressRanges | Conjunto de cadeias de caracteres | Lista de tokens que especifica os endereços remotos cobertos pela regra. Tokens não diferenciam maiúsculas de minúsculas. Os tokens válidos incluem:
- "*" indica qualquer endereço remoto. Se presente, este deve ser o único token incluído.
- "DefaultGateway"
- ESCOPO
- DNS
- WINS
- "Intranet" (compatível com as versões do Windows 1809 +)
- "RmtIntranet" (suportado nas versões do Windows 1809 +)
- "Internet" (suportado nas versões do Windows 1809 +)
- "Ply2Renders" (suportado nas versões do Windows 1809 +)
- "LocalSubnet" indica qualquer endereço local na sub-rede local.
- Uma sub-rede pode ser especificada usando a máscara de sub-rede ou a notação de prefixo de rede. Se nenhuma máscara de sub-rede ou prefixo de rede for especificado, a máscara de sub-rede padrão será 255.255.255.255.
- Um endereço IPv6 válido.
- Um intervalo de endereços IPv4 no formato "Iniciar endereço-end endereço" sem espaços incluídos.
- Um intervalo de endereços IPv6 no formato "Iniciar endereço-end endereço" sem espaços incluídos.
O padrão é qualquer endereço. | | profiletypes | [windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)| Especifica os perfis aos quais a regra pertence. Se não for especificado, o padrão é ALL. Os valores possíveis são `notConfigured`: `domain`, `private`, `public`,. | | ação | [stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)| A ação que a regra impõe. Se não for especificado, o padrão será permitido. Os valores possíveis são `notConfigured`: `blocked`, `allowed`,. | | trafficDirection | [windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)| A direção de tráfego para a qual a regra está habilitada. Se não for especificado, o padrão será out. Os valores possíveis são `notConfigured`: `out`, `in`,. | | Interfaces | [windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)| Os tipos de interface da regra. Os valores possíveis são `notConfigured`: `remoteAccess`, `wireless`, `lan`,. | | localUserAuthorizations | Cadeia de caracteres | Especifica a lista de usuários locais autorizados para o contêiner de aplicativos. Esta é uma cadeia de caracteres no formato SDDL (Security Descriptor Definition Language). |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsFirewallRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsFirewallRule",
  "displayName": "String",
  "description": "String",
  "packageFamilyName": "String",
  "filePath": "String",
  "serviceName": "String",
  "protocol": 1024,
  "localPortRanges": [
    "String"
  ],
  "remotePortRanges": [
    "String"
  ],
  "localAddressRanges": [
    "String"
  ],
  "remoteAddressRanges": [
    "String"
  ],
  "profileTypes": "String",
  "action": "String",
  "trafficDirection": "String",
  "interfaceTypes": "String",
  "localUserAuthorizations": "String"
}
```





