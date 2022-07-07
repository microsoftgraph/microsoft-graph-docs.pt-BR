---
title: Tipo de recurso windows10DeviceFirmwareConfigurationInterface
description: 'Propriedades do grafo para a Interface de Configuração do Firmware do Dispositivo '
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: db2c0e1b9a9815fd5882bd51364cbc2f285d37a7
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668395"
---
# <a name="windows10devicefirmwareconfigurationinterface-resource-type"></a>Tipo de recurso windows10DeviceFirmwareConfigurationInterface

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Propriedades do grafo para a Interface de Configuração do Firmware do Dispositivo 


Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windows10DeviceFirmwareConfigurationInterfaces](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-list.md)|[Coleção windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)|Listar propriedades e relações dos [objetos windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .|
|[Obter windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-get.md)|[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)|Ler propriedades e relações do [objeto windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .|
|[Criar windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-create.md)|[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)|Crie um novo [objeto windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .|
|[Excluir windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-delete.md)|Nenhum|Exclui um [windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md).|
|[Atualizar windows10DeviceFirmwareConfigurationInterface](../api/intune-deviceconfig-windows10devicefirmwareconfigurationinterface-update.md)|[windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md)|Atualize as propriedades de um [objeto windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de marcas de escopo para esta instância de entidade. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Booleano|Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo. A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure. Essa propriedade é somente leitura. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|A aplicabilidade da edição do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|A regra de aplicabilidade da versão do sistema operacional para esta Política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|A regra de aplicabilidade do modo de dispositivo para esta Política. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|descrição|String|O administrador forneceu a descrição da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|changeUefiSettingsPermission|[changeUefiSettingsPermission](../resources/intune-deviceconfig-changeuefisettingspermission.md)|Define o nível de permissão concedido aos usuários para alterar as configurações da UEFI. Os valores possíveis são: `notConfiguredOnly` e `none`.|
|virtualizationOfCpuAndIO|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se a virtualização de CPU e E/S está habilitada. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|Câmeras|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se as câmeras internas estão habilitadas. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|microphonesAndSpeakers|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se microfones ou alto-falantes internos estão habilitados. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|Rádios|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se os rádios internos, por exemplo, WIFI, NFC, Bluetooth, estão habilitados. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|bootFromExternalMedia|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se um usuário tem permissão para inicializar de mídia externa. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|bootFromBuiltInNetworkAdapters|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se um usuário tem permissão para inicializar de adaptadores de rede internos. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|windowsPlatformBinaryTable|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se um usuário tem permissão para habilitar a Tabela Binária da Plataforma Windows. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|simultaneousMultiThreading|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se um usuário tem permissão para habilitar MultiThreading Simultâneo. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|frontCamera|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se um usuário tem permissão para habilitar a Câmera Frontal. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|rearCamera|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se um usuário tem permissão para habilitar a câmera traseira. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|infravermelhaCamera|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se um usuário tem permissão para habilitar a câmera infravermelha. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|Microfone|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se um usuário tem permissão para habilitar o Microfone. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|Bluetooth|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se um usuário tem permissão para habilitar o Bluetooth. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|wirelessWideAreaNetwork|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se um usuário tem permissão para habilitar a Rede de Área Larga Sem Fio. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|nearFieldCommunication|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se um usuário tem permissão para habilitar a Comunicação em Campo Próximo. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|Wifi|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se um usuário tem permissão para habilitar o WiFi. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|usbTypeAPort|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se um usuário tem permissão para habilitar a Porta USB tipo A. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|Sdcard|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se um usuário tem permissão para habilitar a Porta do Cartão SD. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|wakeOnLAN|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se um usuário tem permissão para habilitar o Wake on LAN. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|wakeOnPower|[Capacitação](../resources/intune-deviceconfig-enablement.md)|Define se um usuário tem permissão para habilitar o Wake On Power. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|groupAssignments|[Coleção deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)|A lista de atribuições de grupo para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md)|Status da instalação da configuração de dispositivo por dispositivo. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|Visão geral de status de dispositivos para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|Visão geral de status de usuários para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md)|Visão geral de dispositivos de configuração para Configuração de Dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10DeviceFirmwareConfigurationInterface"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10DeviceFirmwareConfigurationInterface",
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
  "changeUefiSettingsPermission": "String",
  "virtualizationOfCpuAndIO": "String",
  "cameras": "String",
  "microphonesAndSpeakers": "String",
  "radios": "String",
  "bootFromExternalMedia": "String",
  "bootFromBuiltInNetworkAdapters": "String",
  "windowsPlatformBinaryTable": "String",
  "simultaneousMultiThreading": "String",
  "frontCamera": "String",
  "rearCamera": "String",
  "infraredCamera": "String",
  "microphone": "String",
  "bluetooth": "String",
  "wirelessWideAreaNetwork": "String",
  "nearFieldCommunication": "String",
  "wiFi": "String",
  "usbTypeAPort": "String",
  "sdCard": "String",
  "wakeOnLAN": "String",
  "wakeOnPower": "String"
}
```




