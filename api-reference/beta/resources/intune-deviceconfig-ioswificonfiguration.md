---
title: tipo de recurso de iosWiFiConfiguration
description: Fornecendo as configurações neste perfil, você poderá instruir o dispositivo iOS para se conectar ao ponto de extremidade Wi-Fi desejado. Especificando os tipos de segurança e o método de autenticação esperado pelo ponto de extremidade Wi-Fi que você pode fazer a conexão Wi-Fi perfeita para usuário final. Esse perfil fornece tipos de segurança limitado e mais simples que perfil corporativa Wi-Fi.
ms.openlocfilehash: 549f8154e6dc8eee87c7dc324177decf84463740
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039651"
---
# <a name="ioswificonfiguration-resource-type"></a>tipo de recurso de iosWiFiConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Fornecendo as configurações neste perfil, você poderá instruir o dispositivo iOS para se conectar ao ponto de extremidade Wi-Fi desejado. Especificando os tipos de segurança e o método de autenticação esperado pelo ponto de extremidade Wi-Fi que você pode fazer a conexão Wi-Fi perfeita para usuário final. Esse perfil fornece tipos de segurança limitado e mais simples que perfil corporativa Wi-Fi.

Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista iosWiFiConfigurations](../api/intune-deviceconfig-ioswificonfiguration-list.md)|coleção [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|Lista as propriedades e os relacionamentos dos objetos [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .|
|[Obter iosWiFiConfiguration](../api/intune-deviceconfig-ioswificonfiguration-get.md)|[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|Leia as propriedades e os relacionamentos do objeto [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .|
|[Criar iosWiFiConfiguration](../api/intune-deviceconfig-ioswificonfiguration-create.md)|[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|Crie um novo objeto de [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .|
|[Excluir iosWiFiConfiguration](../api/intune-deviceconfig-ioswificonfiguration-delete.md)|Nenhum|Exclui um [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md).|
|[Atualizar iosWiFiConfiguration](../api/intune-deviceconfig-ioswificonfiguration-update.md)|[iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md)|Atualize as propriedades de um objeto [iosWiFiConfiguration](../resources/intune-deviceconfig-ioswificonfiguration.md) .|

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
|networkName|String|Nome da rede|
|SSID|String|Este é o nome da rede Wi-Fi que é difundido para todos os dispositivos.|
|connectAutomatically|Booliano|Conecte automaticamente quando esta rede estiver no intervalo. Essa configuração como true ignorar o prompt do usuário e se conecte automaticamente o dispositivo à rede Wi-Fi.|
|connectWhenNetworkNameIsHidden|Booliano|Conecte-se quando a rede não está transmitindo seu nome (SSID). Quando definido como true, esse perfil força o dispositivo para se conectar a uma rede que não transmite seu SSID para todos os dispositivos.|
|wiFiSecurityType|[wiFiSecurityType](../resources/intune-deviceconfig-wifisecuritytype.md)|Indica se o ponto de extremidade Wi-Fi usa um tipo de segurança baseada em EAP. Os possíveis valores são: `open`, `wpaPersonal`, `wpaEnterprise`, `wep`, `wpa2Personal`, `wpa2Enterprise`.|
|proxySettings|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Tipo de proxy para esta conexão Wi-Fi. Os valores possíveis são: `none`, `manual`, `automatic`.|
|proxyManualAddress|String|Nome de host DNS ou endereço IP do servidor proxy quando a configuração manual está selecionada.|
|proxyManualPort|Int32|Porta do servidor proxy quando a configuração manual está selecionada.|
|proxyAutomaticConfigurationUrl|String|URL do script de configuração automática do servidor proxy quando a configuração automática é selecionada. Essa URL normalmente é o local do arquivo PAC (configuração automática de Proxy).|
|preSharedKey|String|Esta é a chave pré compartilhada para rede Wi-Fi WPA Pessoal.|

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
  "@odata.type": "microsoft.graph.iosWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWiFiConfiguration",
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
  "networkName": "String",
  "ssid": "String",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "String",
  "proxySettings": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "preSharedKey": "String"
}
```





