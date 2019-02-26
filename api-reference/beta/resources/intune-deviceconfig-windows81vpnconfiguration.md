---
title: tipo de recurso windows81VpnConfiguration
description: Ao fornecer as configurações neste perfil, você pode instruir os dispositivos Windows 8,1 (e posteriores) para se conectarem ao ponto de extremidade VPN desejado. Especificando o método de autenticação e os tipos de segurança esperados pelo ponto de extremidade da VPN, você pode tornar a conexão VPN perfeita para o usuário final.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef93e3207fbd7d9171d7d9d28d20f8b07936517a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161597"
---
# <a name="windows81vpnconfiguration-resource-type"></a>tipo de recurso windows81VpnConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ao fornecer as configurações neste perfil, você pode instruir os dispositivos Windows 8,1 (e posteriores) para se conectarem ao ponto de extremidade VPN desejado. Especificando o método de autenticação e os tipos de segurança esperados pelo ponto de extremidade da VPN, você pode tornar a conexão VPN perfeita para o usuário final.


Herda de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windows81VpnConfigurations](../api/intune-deviceconfig-windows81vpnconfiguration-list.md)|coleção [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)|Listar Propriedades e relações dos objetos [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .|
|[Obter windows81VpnConfiguration](../api/intune-deviceconfig-windows81vpnconfiguration-get.md)|[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)|Leia as propriedades e as relações do objeto [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .|
|[Criar windows81VpnConfiguration](../api/intune-deviceconfig-windows81vpnconfiguration-create.md)|[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)|Criar um novo objeto [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .|
|[Excluir windows81VpnConfiguration](../api/intune-deviceconfig-windows81vpnconfiguration-delete.md)|Nenhum|Exclui [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md).|
|[Atualizar windows81VpnConfiguration](../api/intune-deviceconfig-windows81vpnconfiguration-update.md)|[windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md)|Atualiza as propriedades de um objeto [windows81VpnConfiguration](../resources/intune-deviceconfig-windows81vpnconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure. Esta propriedade é somente leitura. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|ConnectionName|String|Nome da conexão exibido para o usuário. Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|servidores|coleção [vpnServer](../resources/intune-deviceconfig-vpnserver.md)|Lista de servidores VPN na rede. Verifique se os usuários finais podem acessar esses locais de rede. Esta coleção pode conter um máximo de 500 elementos. Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|customXml|Binária|Comandos XML personalizados que configura a conexão VPN. (Matriz de bytes codificados por UTF8) Herdado de [windowsVpnConfiguration](../resources/intune-deviceconfig-windowsvpnconfiguration.md)|
|applyOnlyToWindows81|Boolean|Valor que indica se esta política se aplica somente ao Windows 8.1. Essa propriedade é somente leitura.|
|Connection|[windowsVpnConnectionType](../resources/intune-deviceconfig-windowsvpnconnectiontype.md)|Tipo de conexão. Os valores possíveis são: `pulseSecure`, `f5EdgeClient`, `dellSonicWallMobileConnect`, `checkPointCapsuleVpn`.|
|loginGroupOrDomain|String|Domínio ou grupo de logon quando o tipo de conexão é definido como Dell SonicWALL Mobile Connection.|
|enableSplitTunneling|Boolean|Habilitar o tunelamento dividido para a VPN.|
|proxyServer|[windows81VpnProxyServer](../resources/intune-deviceconfig-windows81vpnproxyserver.md)|Servidor proxy.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|coleção [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows81VpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81VpnConfiguration",
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
  "connectionName": "String",
  "servers": [
    {
      "@odata.type": "microsoft.graph.vpnServer",
      "description": "String",
      "address": "String",
      "isDefaultServer": true
    }
  ],
  "customXml": "binary",
  "applyOnlyToWindows81": true,
  "connectionType": "String",
  "loginGroupOrDomain": "String",
  "enableSplitTunneling": true,
  "proxyServer": {
    "@odata.type": "microsoft.graph.windows81VpnProxyServer",
    "automaticConfigurationScriptUrl": "String",
    "address": "String",
    "port": 1024,
    "automaticallyDetectProxySettings": true,
    "bypassProxyServerForLocalAddress": true
  }
}
```




