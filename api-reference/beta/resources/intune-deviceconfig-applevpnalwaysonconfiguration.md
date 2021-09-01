---
title: Tipo de recurso appleVpnAlwaysOnConfiguration
description: Configuração VPN Always On para MacOS e iOS IKEv2
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 38b574bd07e4797a14de2e6061cf45e638ca2b98
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787003"
---
# <a name="applevpnalwaysonconfiguration-resource-type"></a>Tipo de recurso appleVpnAlwaysOnConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Configuração VPN Always On para MacOS e iOS IKEv2

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|tunnelConfiguration|[vpnTunnelConfigurationType](../resources/intune-deviceconfig-vpntunnelconfigurationtype.md)|Determina a que conexões a configuração de túnel específica se aplica. Os valores possíveis são: `wifiAndCellular`, `cellular`, `wifi`.|
|userToggleEnabled|Boleano|Permitir que o usuário alterne a configuração vpn usando a interface do usuário|
|voicemailExceptionAction|[vpnServiceExceptionAction](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|Determine se o serviço de caixa postal será isento da conexão VPN sempre on. Os valores possíveis são: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|airPrintExceptionAction|[vpnServiceExceptionAction](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|Determine se o serviço AirPrint estará isento da conexão VPN always-on. Os valores possíveis são: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|cellularExceptionAction|[vpnServiceExceptionAction](../resources/intune-deviceconfig-vpnserviceexceptionaction.md)|Determine se o serviço Celular será isento da conexão VPN sempre on. Os valores possíveis são: `forceTrafficViaVPN`, `allowTrafficOutside`, `dropTraffic`.|
|allowAllCaptiveNetworkPlugins|Boleano|Especifica se o tráfego de todos os plug-ins de rede cativos deve ser permitido fora da vpn|
|allowedCaptiveNetworkPlugins|[specifiedCaptiveNetworkPlugins](../resources/intune-deviceconfig-specifiedcaptivenetworkplugins.md)|Determina se todos, alguns ou nenhum aplicativo de rede cativo não nativo são permitidos|
|allowCaptiveWebSheet|Boleano|Determina se o tráfego do aplicativo Websheet é permitido fora da VPN|
|natKeepAliveIntervalInSeconds|Int32|Especifica com que frequência, em segundos, enviar um pacote de conversão de endereço de rede continuado por meio da VPN|
|natKeepAliveOffloadEnable|Boleano|Habilitar o descarregamento de hardware de sinais manter-se nat quando o dispositivo estiver inodornado|

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



