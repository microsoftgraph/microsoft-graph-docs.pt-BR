---
title: tipo de recurso windowsFirewallRule
description: Uma regra que controla o tráfego por meio do firewall do Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bf83346e59b15e2394b675744f38d7fbafdb25a4
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692398"
---
# <a name="windowsfirewallrule-resource-type"></a>tipo de recurso windowsFirewallRule

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma regra que controla o tráfego por meio do firewall do Windows.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome de exibição da regra. Não precisa ser exclusivo.|
|description|String|A descrição da regra.|
|packageFamilyName|String|O nome da família de pacotes de um aplicativo da Microsoft Store que é afetado pela regra de firewall.|
|filePath|String|O caminho completo do arquivo de um aplicativo afetado pela regra de firewall.|
|serviceName|String|O nome usado em casos em que um serviço, não um aplicativo, está enviando ou recebendo tráfego.|
|RDP|Int32|0-255 número que representa o protocolo IP (TCP = 6, UDP = 17). Se não for especificado, o padrão é ALL. Valores válidos de 0 a 255|
|localPortRanges|Coleção de cadeias de caracteres|Lista de intervalos de porta locais. Por exemplo, "100-120", "200", "300-320". Se não for especificado, o padrão é ALL.|
|remotePortRanges|Coleção de cadeias de caracteres|Lista de intervalos de portas remotas. Por exemplo, "100-120", "200", "300-320". Se não for especificado, o padrão é ALL.|
|localAddressRanges|Coleção de cadeias de caracteres|Lista de endereços locais cobertos pela regra. O padrão é qualquer endereço. Os tokens válidos incluem:<ul><li>"*" indica qualquer endereço local. Se presente, este deve ser o único token incluído.</li><li>Uma sub-rede pode ser especificada usando a máscara de sub-rede ou a notação de prefixo de rede. Se nenhuma máscara de sub-rede ou prefixo de rede for especificado, a máscara de sub-rede padrão será 255.255.255.255.</li><li>Um endereço IPv6 válido.</li><li>Um intervalo de endereços IPv4 no formato "Iniciar endereço-end endereço" sem espaços incluídos.</li><li>Um intervalo de endereços IPv6 no formato "Iniciar endereço-end endereço" sem espaços incluídos.</li></ul>|
|remoteAddressRanges|Coleção de cadeias de caracteres|Lista de tokens que especifica os endereços remotos cobertos pela regra. Tokens não diferenciam maiúsculas de minúsculas. O padrão é qualquer endereço. Os tokens válidos incluem:<ul><li>"*" indica qualquer endereço remoto. Se presente, este deve ser o único token incluído.</li><li>"DefaultGateway"</li><li>ESCOPO</li><li>DNS</li><li>WINS</li><li>"Intranet" (compatível com as versões do Windows 1809 +)</li><li>"RmtIntranet" (suportado nas versões do Windows 1809 +)</li><li>"Internet" (suportado nas versões do Windows 1809 +)</li><li>"Ply2Renders" (suportado nas versões do Windows 1809 +)</li><li>"LocalSubnet" indica qualquer endereço local na sub-rede local.</li><li>Uma sub-rede pode ser especificada usando a máscara de sub-rede ou a notação de prefixo de rede. Se nenhuma máscara de sub-rede ou prefixo de rede for especificado, a máscara de sub-rede padrão será 255.255.255.255.</li><li>Um endereço IPv6 válido.</li><li>Um intervalo de endereços IPv4 no formato "Iniciar endereço-end endereço" sem espaços incluídos.</li><li>Um intervalo de endereços IPv6 no formato "Iniciar endereço-end endereço" sem espaços incluídos.</li></ul>|
|profiletypes|[windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)|Especifica os perfis aos quais a regra pertence. Se não for especificado, o padrão é ALL. Os valores possíveis são: `notConfigured`, `domain`, `private`, `public`.|
|ação|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|A ação que a regra impõe. Se não for especificado, o padrão será permitido. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|trafficDirection|[windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)|A direção de tráfego para a qual a regra está habilitada. Se não for especificado, o padrão será out. Os valores possíveis são: `notConfigured` , `out` , `in` .|
|Interface de interface|[windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)|Os tipos de interface da regra. Os valores possíveis são: `notConfigured`, `remoteAccess`, `wireless`, `lan`.|
|edgeTraversal|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Indica se a travessia de borda está habilitada ou desabilitada para esta regra. A configuração EdgeTraversal indica que o tráfego de entrada específico tem permissão para fazer o túnel por meio de NATs e outros dispositivos de borda usando a tecnologia de encapsulamento Teredo. Para que essa configuração funcione corretamente, o aplicativo ou serviço com a regra de firewall de entrada precisa dar suporte a IPv6. O aplicativo principal dessa configuração permite que os ouvintes no host sejam endereçados globalmente por meio de um endereço IPv6 Teredo. As novas regras têm a propriedade EdgeTraversal desabilitada por padrão. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|localUserAuthorizations|String|Especifica a lista de usuários locais autorizados para o contêiner de aplicativos. Esta é uma cadeia de caracteres no formato SDDL (Security Descriptor Definition Language).|

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
  "edgeTraversal": "String",
  "localUserAuthorizations": "String"
}
```





