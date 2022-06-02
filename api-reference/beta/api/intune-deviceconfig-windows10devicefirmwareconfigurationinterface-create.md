---
title: Criar windows10DeviceFirmwareConfigurationInterface
description: Crie um novo objeto windows10DeviceFirmwareConfigurationInterface.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1ef1042b4942160c2491760ccbfc33358c772e8d
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857887"
---
# <a name="create-windows10devicefirmwareconfigurationinterface"></a>Criar windows10DeviceFirmwareConfigurationInterface

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto windows10DeviceFirmwareConfigurationInterface.

A tabela a seguir mostra as propriedades que são necessárias ao criar o windows10DeviceFirmwareConfigurationInterface.

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
|changeUefiSettingsPermission|[changeUefiSettingsPermission](../resources/intune-deviceconfig-changeuefisettingspermission.md)|Define o nível de permissão concedido aos usuários para alterar as configurações da UEFI. Os valores possíveis são: `notConfiguredOnly` e `none`.|
|virtualizationOfCpuAndIO|[Capacitação](../resources/intune-shared-enablement.md)|Define se a virtualização de CPU e E/S está habilitada. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|Câmeras|[Capacitação](../resources/intune-shared-enablement.md)|Define se as câmeras internas estão habilitadas. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|microphonesAndSpeakers|[Capacitação](../resources/intune-shared-enablement.md)|Define se microfones ou alto-falantes internos estão habilitados. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|Rádios|[Capacitação](../resources/intune-shared-enablement.md)|Define se rádios internos, por exemplo, WIFI, NFC, Bluetooth, estão habilitados. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|bootFromExternalMedia|[Capacitação](../resources/intune-shared-enablement.md)|Define se um usuário tem permissão para inicializar de mídia externa. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|bootFromBuiltInNetworkAdapters|[Capacitação](../resources/intune-shared-enablement.md)|Define se um usuário tem permissão para inicializar de adaptadores de rede internos. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|windowsPlatformBinaryTable|[Capacitação](../resources/intune-shared-enablement.md)|Define se um usuário tem permissão para habilitar Windows Tabela Binária da Plataforma. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|simultaneousMultiThreading|[Capacitação](../resources/intune-shared-enablement.md)|Define se um usuário tem permissão para habilitar MultiThreading Simultâneo. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|frontCamera|[Capacitação](../resources/intune-shared-enablement.md)|Define se um usuário tem permissão para habilitar o Front Câmera. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|rearCamera|[Capacitação](../resources/intune-shared-enablement.md)|Define se um usuário tem permissão para habilitar a câmera traseira. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|infravermelhaCamera|[Capacitação](../resources/intune-shared-enablement.md)|Define se um usuário tem permissão para habilitar a câmera infravermelha. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|Microfone|[Capacitação](../resources/intune-shared-enablement.md)|Define se um usuário tem permissão para habilitar o Microfone. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|Bluetooth|[Capacitação](../resources/intune-shared-enablement.md)|Define se um usuário tem permissão para habilitar Bluetooth. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|wirelessWideAreaNetwork|[Capacitação](../resources/intune-shared-enablement.md)|Define se um usuário tem permissão para habilitar a Rede de Área Larga Sem Fio. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|nearFieldCommunication|[Capacitação](../resources/intune-shared-enablement.md)|Define se um usuário tem permissão para habilitar a Comunicação em Campo Próximo. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|Wifi|[Capacitação](../resources/intune-shared-enablement.md)|Define se um usuário tem permissão para habilitar o WiFi. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|usbTypeAPort|[Capacitação](../resources/intune-shared-enablement.md)|Define se um usuário tem permissão para habilitar a Porta USB tipo A. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|Sdcard|[Capacitação](../resources/intune-shared-enablement.md)|Define se um usuário tem permissão para habilitar a Porta do Cartão SD. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|wakeOnLAN|[Capacitação](../resources/intune-shared-enablement.md)|Define se um usuário tem permissão para habilitar o Wake on LAN. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|
|wakeOnPower|[Capacitação](../resources/intune-shared-enablement.md)|Define se um usuário tem permissão para habilitar o Wake On Power. Os valores possíveis são: `notConfigured`, `enabled`, `disabled`.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `201 Created` um código de resposta e um [objeto windows10DeviceFirmwareConfigurationInterface](../resources/intune-deviceconfig-windows10devicefirmwareconfigurationinterface.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1754

{
  "@odata.type": "#microsoft.graph.windows10DeviceFirmwareConfigurationInterface",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "changeUefiSettingsPermission": "none",
  "virtualizationOfCpuAndIO": "enabled",
  "cameras": "enabled",
  "microphonesAndSpeakers": "enabled",
  "radios": "enabled",
  "bootFromExternalMedia": "enabled",
  "bootFromBuiltInNetworkAdapters": "enabled",
  "windowsPlatformBinaryTable": "enabled",
  "simultaneousMultiThreading": "enabled",
  "frontCamera": "enabled",
  "rearCamera": "enabled",
  "infraredCamera": "enabled",
  "microphone": "enabled",
  "bluetooth": "enabled",
  "wirelessWideAreaNetwork": "enabled",
  "nearFieldCommunication": "enabled",
  "wiFi": "enabled",
  "usbTypeAPort": "enabled",
  "sdCard": "enabled",
  "wakeOnLAN": "enabled",
  "wakeOnPower": "enabled"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1926

{
  "@odata.type": "#microsoft.graph.windows10DeviceFirmwareConfigurationInterface",
  "id": "96474363-4363-9647-6343-479663434796",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "changeUefiSettingsPermission": "none",
  "virtualizationOfCpuAndIO": "enabled",
  "cameras": "enabled",
  "microphonesAndSpeakers": "enabled",
  "radios": "enabled",
  "bootFromExternalMedia": "enabled",
  "bootFromBuiltInNetworkAdapters": "enabled",
  "windowsPlatformBinaryTable": "enabled",
  "simultaneousMultiThreading": "enabled",
  "frontCamera": "enabled",
  "rearCamera": "enabled",
  "infraredCamera": "enabled",
  "microphone": "enabled",
  "bluetooth": "enabled",
  "wirelessWideAreaNetwork": "enabled",
  "nearFieldCommunication": "enabled",
  "wiFi": "enabled",
  "usbTypeAPort": "enabled",
  "sdCard": "enabled",
  "wakeOnLAN": "enabled",
  "wakeOnPower": "enabled"
}
```




