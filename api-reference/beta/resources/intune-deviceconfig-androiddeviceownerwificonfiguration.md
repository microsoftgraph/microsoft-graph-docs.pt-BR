---
title: Tipo de recurso androidDeviceOwnerWiFiConfiguration
description: Ao fornecer as configurações nesse perfil, você pode instruir o dispositivo Android se conectar ao ponto de extremidade Wi-Fi desejado. Especificando o método de autenticação e os tipos de segurança esperados Wi-Fi ponto de extremidade, você pode tornar a conexão Wi-Fi perfeita para o usuário final. Esse perfil fornece tipos de segurança limitados e mais simples do que Enterprise Wi-Fi perfil.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0be04023333876fcbee23e7f55a627b26b78d725
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858293"
---
# <a name="androiddeviceownerwificonfiguration-resource-type"></a>Tipo de recurso androidDeviceOwnerWiFiConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ao fornecer as configurações nesse perfil, você pode instruir o dispositivo Android se conectar ao ponto de extremidade Wi-Fi desejado. Especificando o método de autenticação e os tipos de segurança esperados Wi-Fi ponto de extremidade, você pode tornar a conexão Wi-Fi perfeita para o usuário final. Esse perfil fornece tipos de segurança limitados e mais simples do que Enterprise Wi-Fi perfil.


Herda de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidDeviceOwnerWiFiConfigurations](../api/intune-deviceconfig-androiddeviceownerwificonfiguration-list.md)|[coleção androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|Listar propriedades e relações dos objetos [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) .|
|[Obter androidDeviceOwnerWiFiConfiguration](../api/intune-deviceconfig-androiddeviceownerwificonfiguration-get.md)|[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|Ler propriedades e relações do objeto [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) .|
|[Criar androidDeviceOwnerWiFiConfiguration](../api/intune-deviceconfig-androiddeviceownerwificonfiguration-create.md)|[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|Crie um novo [objeto androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) .|
|[Excluir androidDeviceOwnerWiFiConfiguration](../api/intune-deviceconfig-androiddeviceownerwificonfiguration-delete.md)|Nenhum|Exclui um [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md).|
|[Atualizar androidDeviceOwnerWiFiConfiguration](../api/intune-deviceconfig-androiddeviceownerwificonfiguration-update.md)|[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)|Atualize as propriedades de um [objeto androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|roleScopeTagIds|Coleção String|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|description|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|networkName|String|Nome da Rede|
|Ssid|String|Esse é o nome da rede Wi-Fi que é transmitida para todos os dispositivos.|
|connectAutomatically|Booliano|Conexão automaticamente quando essa rede estiver no intervalo. Definir isso como true ignorará o prompt do usuário e conectará automaticamente o dispositivo Wi-Fi rede.|
|connectWhenNetworkNameIsHidden|Booliano|Quando definido como true, esse perfil força o dispositivo a se conectar a uma rede que não transmite seu SSID para todos os dispositivos.|
|wiFiSecurityType|[androidDeviceOwnerWiFiSecurityType](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|Indica se o Wi-Fi de extremidade usa um tipo de segurança baseado em EAP. Os valores possíveis são: `open`, `wep`, `wpaPersonal`, `wpaEnterprise`.|
|preSharedKey|String|Essa é a chave pré-compartilhada para a rede de Wi-Fi WPA Personal.|
|preSharedKeyIsSet|Booliano|Essa é a chave pré-compartilhada para a rede de Wi-Fi WPA Personal.|
|proxySettings|[wiFiProxySetting](../resources/intune-deviceconfig-wifiproxysetting.md)|Especifique a configuração de proxy Wi-Fi configuração. Os valores possíveis incluem nenhum, manual e automático. Os valores possíveis são: `none`, `manual`, `automatic`.|
|proxyManualAddress|String|Especifique o endereço IP do servidor proxy. Android documentação não especifica IPv4 ou IPv6. Por exemplo: 192.168.1.1.|
|proxyManualPort|Int32|Especifique a porta do servidor proxy.|
|proxyAutomaticConfigurationUrl|String|Especifique a URL de script de configuração do servidor proxy.|
|proxyExclusionList|String|Lista de hosts a serem excluídos usando o proxy em conexões. Esses hosts podem usar caracteres curinga, como *.example.com.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|[Coleção deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status da instalação da configuração de dispositivo por dispositivo. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidDeviceOwnerWiFiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "networkName": "String",
  "ssid": "String",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "String",
  "preSharedKey": "String",
  "preSharedKeyIsSet": true,
  "proxySettings": "String",
  "proxyManualAddress": "String",
  "proxyManualPort": 1024,
  "proxyAutomaticConfigurationUrl": "String",
  "proxyExclusionList": "String"
}
```




