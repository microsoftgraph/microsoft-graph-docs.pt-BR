---
title: tipo de recurso appleVpnAlwaysOnConfiguration
description: Configuração de VPN AlwaysOn para MacOS e iOS IKEv2
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 10facf24c8fd56786c2706e1fa8ee999f48e2ed7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796065"
---
# <a name="applevpnalwaysonconfiguration-resource-type"></a>tipo de recurso appleVpnAlwaysOnConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configuração de VPN AlwaysOn para MacOS e iOS IKEv2

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|tunnelConfiguration|[vpnTunnelConfigurationType](../resources/intune-deviceconfig-vpntunnelconfigurationtype.md)|Determina a quais conexões a configuração de túnel específica se aplica. Os valores possíveis são: `wifiAndCellular`, `cellular`, `wifi`.|
|userToggleEnabled|Boolean|Permitir que o usuário alterne a configuração VPN usando a interface do usuário|
|voicemailExceptionAction|[vpnServiceExceptionAction](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|Determine se o serviço de caixa postal será isento da conexão VPN sempre ativa. Os valores possíveis são: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|airPrintExceptionAction|[vpnServiceExceptionAction](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|Determine se o serviço de impressão do servidor será isento da conexão VPN sempre ativa. Os valores possíveis são: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|cellularExceptionAction|[vpnServiceExceptionAction](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|Determine se o serviço celular será isento da conexão VPN sempre ativa. Os valores possíveis são: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|allowAllCaptiveNetworkPlugins|Boolean|Especifica se o tráfego de todos os plugins de rede prisioneiros deve ser permitido fora da VPN|
|allowedCaptiveNetworkPlugins|[specifiedCaptiveNetworkPlugins](../resources/intune-deviceconfig-specifiedcaptivenetworkplugins.md)|Determina se todos, alguns ou nenhum aplicativo de rede cativo não nativo são permitidos|
|allowCaptiveWebSheet|Boolean|Determina se o tráfego do aplicativo Websheet é permitido fora da VPN|
|natKeepAliveIntervalInSeconds|Int32|Especifica com que frequência, em segundos, enviar um pacote de KeepAlive de conversão de endereços de rede através da VPN|
|natKeepAliveOffloadEnable|Boolean|Habilitar descarregamento de hardware de sinais de KeepAlive de NAT quando o dispositivo estiver suspenso|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleVpnAlwaysOnConfiguration",
  "tunnelConfiguration": "String",
  "userToggleEnabled": true,
  "voicemailExceptionAction": "String",
  "airPrintExceptionAction": "String",
  "cellularExceptionAction": "String",
  "allowAllCaptiveNetworkPlugins": true,
  "allowedCaptiveNetworkPlugins": {
    "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
    "allowedBundleIdentifiers": [
      "String"
    ]
  },
  "allowCaptiveWebSheet": true,
  "natKeepAliveIntervalInSeconds": 1024,
  "natKeepAliveOffloadEnable": true
}
```



