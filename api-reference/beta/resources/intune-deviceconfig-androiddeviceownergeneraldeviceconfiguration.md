---
title: tipo de recurso androidDeviceOwnerGeneralDeviceConfiguration
description: Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso androidDeviceOwnerGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fee3354cc66bb90a51874986ed46b80b4a8c9d8c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156200"
---
# <a name="androiddeviceownergeneraldeviceconfiguration-resource-type"></a>tipo de recurso androidDeviceOwnerGeneralDeviceConfiguration

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso androidDeviceOwnerGeneralDeviceConfiguration.


Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidDeviceOwnerGeneralDeviceConfigurations](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-list.md)|coleção [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Listar Propriedades e relações dos objetos [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|
|[Obter androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-get.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Leia as propriedades e as relações do objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|
|[Criar androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-create.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Criar um novo objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|
|[Excluir androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-delete.md)|Nenhum|Exclui [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).|
|[Atualizar androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-update.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Atualiza as propriedades de um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|

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
|accountsBlockModification|Boolean|Indica se a adição ou a remoção de contas está desabilitada.|
|appsAllowInstallFromUnknownSources|Boolean|Indica se o usuário tem permissão para habilitar a configuração de fontes desconhecidas.|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|Indica o valor da política de atualização automática do aplicativo. Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|Indica a política de permissão para solicitações de permissões de tempo de execução se uma não estiver definida para o aplicativo especificamente. Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|appsRecommendSkippingFirstUseHints|Boolean|Se todos os aplicativos devem ou não ser recomendados, pule qualquer dica de primeira vez que ele possa ter adicionado.|
|bluetoothBlockConfiguration|Boolean|Indica se um usuário será ou não impedido de configurar o Bluetooth.|
|bluetoothBlockContactSharing|Boolean|Indica se um usuário será ou não impedido de compartilhar contatos via Bluetooth.|
|cameraBlocked|Boolean|Indica se o uso da câmera deve ou não ser desativado.|
|cellularBlockWiFiTethering|Boolean|Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.|
|dataRoamingBlocked|Boolean|Indica se um usuário será ou não bloqueado de roaming de dados.|
|dateTimeConfigurationBlocked|Boolean|Indica se o usuário será ou não impedido de alterar manualmente a data ou a hora no dispositivo|
|factoryResetDeviceAdministratorEmails|Coleção de cadeias de caracteres|Lista de emails de conta do Google que serão necessários para autenticar após a redefinição de fábrica de um dispositivo antes que ele possa ser configurado.|
|factoryResetBlocked|Boolean|Indica se a opção de redefinição de fábrica em configurações está desabilitada.|
|kioskModeApps|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Uma lista de aplicativos gerenciados que serão mostrados quando o dispositivo estiver no modo quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|kioskModeWallpaperUrl|String|URL para uma imagem publicamente acessível a ser usada para o papel de parede quando o dispositivo estiver no modo quiosque.|
|kioskModeExitCode|String|Código de saída para permitir que um usuário saia do modo quiosque quando o dispositivo estiver no modo quiosque.|
|kioskModeVirtualHomeButtonEnabled|Boolean|Se um botão de Home virtual será exibido ou não quando o dispositivo estiver no modo quiosque.|
|microphoneForceMute|Boolean|Indica se a desativação do microfone no dispositivo deve ou não ser bloqueada.|
|networkEscapeHatchAllowed|Boolean|Indica se o dispositivo permitirá ou não conexão com uma conexão de rede temporária no momento da inicialização.|
|nfcBlockOutgoingBeam|Boolean|Indica se o feixe de saída NFC deve ou não ser bloqueado.|
|passwordBlockKeyguard|Boolean|Indica se o keyguard está desabilitado ou não.|
|passwordBlockKeyguardFeatures|coleção [androidKeyguardFeature](../resources/intune-deviceconfig-androidkeyguardfeature.md)|Lista de recursos de keyguard de dispositivo para bloquear. Essa coleção pode conter um máximo de 7 elementos.|
|passwordExpirationDays|Int32|Indica a quantidade de tempo, em segundos, que uma senha pode ser definida para antes de expirar e uma nova senha será necessária. Valores válidos de 1 a 365|
|passwordMinimumLength|Int32|Indica o comprimento mínimo da senha necessária no dispositivo. Valores válidos de 4 a 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Milissegundos de inatividade antes da tela expirar.|
|passwordPreviousPasswordCountToBlock|Int32|Indica o comprimento do histórico de senhas, onde o usuário não poderá inserir uma nova senha que seja igual a qualquer senha no histórico. Valores válidos de 0 a 24|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Indica a qualidade mínima da senha necessária no dispositivo. Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Indica o número de vezes que um usuário pode inserir uma senha incorreta antes que o dispositivo seja apagado. Valores válidos de 4 a 11|
|safeBootBlocked|Boolean|Indica se o dispositivo será reinicializado na inicialização segura está desabilitado.|
|screenCaptureBlocked|Boolean|Indica se a capacidade de realizar capturas de tela deve ou não ser desabilitada.|
|securityAllowDebuggingFeatures|Boolean|Indica se o usuário será ou não impedido de habilitar recursos de depuração no dispositivo.|
|securityRequireVerifyApps|Boolean|Indica se os aplicativos devem ou não ser verificados.|
|statusBarBlocked|Boolean|Indica se a barra de status está desabilitada, incluindo notificações, configurações rápidas e outras sobreposições de tela.|
|stayOnModes|coleção [androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)|Lista de modos em que a exibição do dispositivo permanecerá ligada. Essa coleção pode conter um máximo de 4 elementos.|
|storageAllowUsb|Boolean|Indica se o armazenamento em massa USB deve ou não ser permitido.|
|storageBlockExternalMedia|Boolean|Indica se a mídia externa deve ou não ser bloqueada.|
|storageBlockUsbFileTransfer|Boolean|Indica se a transferência de arquivos USB deve ou não ser bloqueada.|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|Indica o número de minutos após a meia-noite que a janela de atualização do sistema é iniciada. Valores válidos de 0 a 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|Indica o número de minutos após a meia-noite que a janela de atualização do sistema termina. Valores válidos de 0 a 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|O tipo de configuração de atualização do sistema. Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.|
|systemWindowsBlocked|Boolean|Se as janelas de prompt do sistema Android serão bloqueadas ou não, como notificações, atividades de telefone e alertas de sistema.|
|usersBlockAdd|Boolean|Indica se os usuários e perfis serão ou não desabilitados.|
|usersBlockRemove|Boolean|Indica se a remoção de outros usuários do dispositivo deve ou não ser desabilitada.|
|volumeBlockAdjustment|Boolean|Indica se o ajuste do volume mestre está ou não desabilitado.|
|vpnAlwaysOnPackageIdentifier|String|Nome do pacote do aplicativo Android para o aplicativo que manipulará uma conexão VPN sempre ativa.|
|vpnAlwaysOnLockdownMode|Boolean|Se um nome de pacote VPN Always on for especificado, se o tráfego de rede será ou não bloqueado quando essa VPN for desconectada.|
|wifiBlockEditConfigurations|Boolean|Indica se o usuário será ou não impedido de editar as configurações de conexão WiFi.|
|wifiBlockEditPolicyDefinedConfigurations|Boolean|Indica se o usuário será ou não impedido de editar apenas as redes definidas pela política.|

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
  "@odata.type": "microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
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
  "accountsBlockModification": true,
  "appsAllowInstallFromUnknownSources": true,
  "appsAutoUpdatePolicy": "String",
  "appsDefaultPermissionPolicy": "String",
  "appsRecommendSkippingFirstUseHints": true,
  "bluetoothBlockConfiguration": true,
  "bluetoothBlockContactSharing": true,
  "cameraBlocked": true,
  "cellularBlockWiFiTethering": true,
  "dataRoamingBlocked": true,
  "dateTimeConfigurationBlocked": true,
  "factoryResetDeviceAdministratorEmails": [
    "String"
  ],
  "factoryResetBlocked": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "kioskModeWallpaperUrl": "String",
  "kioskModeExitCode": "String",
  "kioskModeVirtualHomeButtonEnabled": true,
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
  "passwordBlockKeyguardFeatures": [
    "String"
  ],
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordCountToBlock": 1024,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "safeBootBlocked": true,
  "screenCaptureBlocked": true,
  "securityAllowDebuggingFeatures": true,
  "securityRequireVerifyApps": true,
  "statusBarBlocked": true,
  "stayOnModes": [
    "String"
  ],
  "storageAllowUsb": true,
  "storageBlockExternalMedia": true,
  "storageBlockUsbFileTransfer": true,
  "systemUpdateWindowStartMinutesAfterMidnight": 1024,
  "systemUpdateWindowEndMinutesAfterMidnight": 1024,
  "systemUpdateInstallType": "String",
  "systemWindowsBlocked": true,
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "vpnAlwaysOnPackageIdentifier": "String",
  "vpnAlwaysOnLockdownMode": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```




