---
title: tipo de recurso de windowsWifiConfiguration
description: Configuração do dispositivo.
ms.openlocfilehash: 13f2a5819e77c5687c0d4331b19ee6dfc50a1d12
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041028"
---
# <a name="windowswificonfiguration-resource-type"></a>tipo de recurso de windowsWifiConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Configuração do dispositivo.

Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista windowsWifiConfigurations](../api/intune-deviceconfig-windowswificonfiguration-list.md)|coleção [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|Lista as propriedades e os relacionamentos dos objetos [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .|
|[Obter windowsWifiConfiguration](../api/intune-deviceconfig-windowswificonfiguration-get.md)|[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|Leia as propriedades e os relacionamentos do objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .|
|[Criar windowsWifiConfiguration](../api/intune-deviceconfig-windowswificonfiguration-create.md)|[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|Crie um novo objeto de [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .|
|[Excluir windowsWifiConfiguration](../api/intune-deviceconfig-windowswificonfiguration-delete.md)|Nenhum|Exclui um [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md).|
|[Atualizar windowsWifiConfiguration](../api/intune-deviceconfig-windowswificonfiguration-update.md)|[windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md)|Atualize as propriedades de um objeto [windowsWifiConfiguration](../resources/intune-deviceconfig-windowswificonfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String collection|Lista de escopo marcas para essa instância da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo. Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure. Esta propriedade é somente leitura. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|preSharedKey|String|Esta é a chave pré compartilhada para rede Wi-Fi WPA Pessoal.|
|wifiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Especifica o tipo de segurança Wifi. Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.|
|meteredConnectionLimit|[meteredConnectionLimitType](../resources/intune-deviceconfig-meteredconnectionlimittype.md)|Especifica o tipo de limite de conexão monitorados para a conexão wifi. Os valores possíveis são: `unrestricted`, `fixed`, `variable`.|
|SSID|String|Especifique o SSID da conexão wifi.|
|networkName|String|Especifique o nome da configuração de rede.|
|connectAutomatically|Booliano|Especifique se a conexão wifi deve conectar automaticamente quando estiver no intervalo.|
|connectToPreferredNetwork|Booliano|Especifique se a conexão wifi deve se conectar às redes mais preferenciais quando já conectado a este.  Requer ConnectAutomatically seja true.|
|connectWhenNetworkNameIsHidden|Booliano|Especifique se a conexão wifi deve conectar automaticamente mesmo quando o SSID não está transmitindo.|
|proxySetting|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Especifica a configuração para configuração de Wi-Fi do proxy. Os valores possíveis são: `none`, `manual`, `automatic`.|
|proxyManualAddress|String|Especifique o endereço IP do servidor proxy.|
|proxyManualPort|Int32|Especifique a porta para o servidor proxy.|
|proxyAutomaticConfigurationUrl|String|Especifique a URL para o script de configuração do servidor proxy.|
|forceFIPSCompliance|Booliano|Especifique se deseja forçar a conformidade FIPS.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração de dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsWifiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsWifiConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "preSharedKey": "String",
  "wifiSecurityType": "String",
  "meteredConnectionLimit": "String",
  "ssid": "String",
  "networkName": "String",
  "connectAutomatically": true,
  "connectToPreferredNetwork": true,
  "connectWhenNetworkNameIsHidden": true,
  "proxySetting": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "forceFIPSCompliance": true
}
```





