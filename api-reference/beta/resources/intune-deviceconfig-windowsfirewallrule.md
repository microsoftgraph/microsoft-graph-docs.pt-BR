---
title: Tipo de recurso windowsFirewallRule
description: Uma regra que controla o tráfego por meio Windows Firewall.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1c34a3d9a9b5d0b4078256fdd16e8f0a9ae833c6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58821652"
---
# <a name="windowsfirewallrule-resource-type"></a>Tipo de recurso windowsFirewallRule

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma regra que controla o tráfego por meio Windows Firewall.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|O nome de exibição da regra. Não precisa ser exclusivo.|
|description|Cadeia de caracteres|A descrição da regra.|
|packageFamilyName|Cadeia de caracteres|O nome da família de pacotes de Microsoft Store aplicativo que é afetado pela regra de firewall.|
|filePath|Cadeia de caracteres|O caminho completo do arquivo de um aplicativo afetado pela regra de firewall.|
|serviceName|Cadeia de caracteres|O nome usado nos casos em que um serviço, não um aplicativo, está enviando ou recebendo tráfego.|
|protocol|Int32|0-255 número representando o protocolo IP (TCP = 6, UDP = 17). Se não for especificado, o padrão será All. Valores válidos de 0 a 255|
|localPortRanges|Coleção de cadeias de caracteres|Lista de intervalos de portas locais. Por exemplo, "100-120", "200", "300-320". Se não for especificado, o padrão será All.|
|remotePortRanges|Coleção String|Lista de intervalos de portas remotas. Por exemplo, "100-120", "200", "300-320". Se não for especificado, o padrão será All.|
|localAddressRanges|Coleção String|Lista de endereços locais abordados pela regra. Padrão é qualquer endereço. Os tokens válidos incluem:<ul><li>"*" indica qualquer endereço local. Se presente, esse deve ser o único token incluído.</li><li>Uma sub-rede pode ser especificada usando a notação de prefixo de rede ou máscara de sub-rede. Se nem uma máscara de sub-rede nem um prefixo de rede for especificado, a máscara de sub-rede será padrão para 255.255.255.255.</li><li>Um endereço IPv6 válido.</li><li>Um intervalo de endereços IPv4 no formato "endereço inicial - endereço final" sem espaços incluídos.</li><li>Um intervalo de endereços IPv6 no formato "endereço inicial - endereço final" sem espaços incluídos.</li></ul>|
|remoteAddressRanges|Coleção de cadeias de caracteres|Lista de tokens que especificam os endereços remotos cobertos pela regra. Tokens não são maiúsculas de minúsculas. Padrão é qualquer endereço. Os tokens válidos incluem:<ul><li>"*" indica qualquer endereço remoto. Se presente, esse deve ser o único token incluído.</li><li>"Defaultgateway"</li><li>"DHCP"</li><li>"DNS"</li><li>"WINS"</li><li>"Intranet" (com suporte Windows versões 1809+)</li><li>"RmtIntranet" (com suporte Windows versões 1809+)</li><li>"Internet" (com suporte em Windows versões 1809+)</li><li>"Ply2Renders" (com suporte Windows versões 1809+)</li><li>"LocalSubnet" indica qualquer endereço local na sub-rede local.</li><li>Uma sub-rede pode ser especificada usando a notação de prefixo de rede ou máscara de sub-rede. Se nem uma máscara de sub-rede nem um prefixo de rede for especificado, a máscara de sub-rede será padrão para 255.255.255.255.</li><li>Um endereço IPv6 válido.</li><li>Um intervalo de endereços IPv4 no formato "endereço inicial - endereço final" sem espaços incluídos.</li><li>Um intervalo de endereços IPv6 no formato "endereço inicial - endereço final" sem espaços incluídos.</li></ul>|
|profileTypes|[windowsFirewallRuleNetworkProfileTypes](../resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes.md)|Especifica os perfis aos quais a regra pertence. Se não for especificado, o padrão será All. Os valores possíveis são: `notConfigured`, `domain`, `private`, `public`.|
|ação|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|A ação que a regra impõe. Se não for especificado, o padrão será Allowed. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|trafficDirection|[windowsFirewallRuleTrafficDirectionType](../resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype.md)|A direção de tráfego para a qual a regra está habilitada. Se não for especificado, o padrão será Out. Os valores possíveis são: `notConfigured` , `out` , `in` .|
|interfaceTypes|[windowsFirewallRuleInterfaceTypes](../resources/intune-deviceconfig-windowsfirewallruleinterfacetypes.md)|Os tipos de interface da regra. Os valores possíveis são: `notConfigured`, `remoteAccess`, `wireless`, `lan`.|
|edgeTraversal|[stateManagementSetting](../resources/intune-deviceconfig-statemanagementsetting.md)|Indica se a rotação de borda está habilitada ou desabilitada para essa regra. A configuração EdgeTraversal indica que o tráfego de entrada específico pode ser túnel através de NATs e outros dispositivos de borda usando a tecnologia de túnel teredo. Para que essa configuração funcione corretamente, o aplicativo ou serviço com a regra de firewall de entrada precisa dar suporte a IPv6. O aplicativo principal dessa configuração permite que os ouvintes no host sejam globalmente abordadas por meio de um endereço IPv6 de Teredo. As novas regras têm a propriedade EdgeTraversal desabilitada por padrão. Os valores possíveis são: `notConfigured`, `blocked`, `allowed`.|
|localUserAuthorizations|Cadeia de caracteres|Especifica a lista de usuários locais autorizados para o contêiner do aplicativo. Esta é uma cadeia de caracteres no formato SDDL (Linguagem de Definição do Descritor de Segurança).|

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



