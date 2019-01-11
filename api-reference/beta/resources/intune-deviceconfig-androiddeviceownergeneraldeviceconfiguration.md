---
title: tipo de recurso de androidDeviceOwnerGeneralDeviceConfiguration
description: Este tópico fornece descrições dos declarado métodos, propriedades e os relacionamentos expostos pelo recurso androidDeviceOwnerGeneralDeviceConfiguration.
localization_priority: Normal
ms.openlocfilehash: 4388c7a79a1db16df92bfa55ec0e205da692fb1a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835452"
---
# <a name="androiddeviceownergeneraldeviceconfiguration-resource-type"></a>tipo de recurso de androidDeviceOwnerGeneralDeviceConfiguration

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Este tópico fornece descrições dos declarado métodos, propriedades e os relacionamentos expostos pelo recurso androidDeviceOwnerGeneralDeviceConfiguration.

Herda de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista androidDeviceOwnerGeneralDeviceConfigurations](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-list.md)|coleção [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Lista as propriedades e os relacionamentos dos objetos [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|
|[Obter androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-get.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Leia as propriedades e os relacionamentos do objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|
|[Criar androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-create.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Crie um novo objeto de [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|
|[Excluir androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-delete.md)|Nenhum|Exclui um [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md).|
|[Atualizar androidDeviceOwnerGeneralDeviceConfiguration](../api/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration-update.md)|[androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md)|Atualize as propriedades de um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|roleScopeTagIds|String collection|Lista de escopo marcas para essa instância da entidade. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|supportsScopeTags|Booliano|Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo. Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo. Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure. Esta propriedade é somente leitura. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)|
|accountsBlockModification|Booliano|Indica se ou não adicionando ou removendo contas está desabilitado.|
|appsAllowInstallFromUnknownSources|Booliano|Indica se o usuário será permitido ou não para habilitar a configuração de fontes desconhecidos.|
|appsAutoUpdatePolicy|[androidDeviceOwnerAppAutoUpdatePolicyType](../resources/intune-deviceconfig-androiddeviceownerappautoupdatepolicytype.md)|Indica o valor da política de atualização automática de app. Os valores possíveis são: `notConfigured`, `userChoice`, `never`, `wiFiOnly`, `always`.|
|appsDefaultPermissionPolicy|[androidDeviceOwnerDefaultAppPermissionPolicyType](../resources/intune-deviceconfig-androiddeviceownerdefaultapppermissionpolicytype.md)|Indica a política de permissão para as solicitações de permissões de tempo de execução se uma não estiver definida para o aplicativo especificamente. Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.|
|bluetoothBlockConfiguration|Booliano|Indica se deve ou não bloquear um usuário configurando bluetooth.|
|bluetoothBlockContactSharing|Booliano|Indica se deve ou não bloquear um usuário compartilhando contatos via bluetooth.|
|cameraBlocked|Booliano|Indica se ou não desabilitar o uso da câmera.|
|cellularBlockWiFiTethering|Booliano|Indica se o compartilhamento de Internet por Wi-Fi deve ou não ser bloqueado.|
|dataRoamingBlocked|Booliano|Indica se deve ou não bloquear um usuário a partir de dados de roaming.|
|dateTimeConfigurationBlocked|Booliano|Indica se ou não impedir que o usuário altere manualmente a data ou hora no dispositivo|
|factoryResetDeviceAdministratorEmails|String collection|Lista de emails de conta do Google que serão necessários para autenticar depois que um dispositivo é redefinida antes que ele pode ser configurado de fábrica.|
|factoryResetBlocked|Booliano|Indica se ou não a opção de redefinição de fábrica nas configurações está desabilitada.|
|kioskModeApps|Coleção [appListItem](../resources/intune-deviceconfig-applistitem.md)|Uma lista de aplicativos gerenciados que será exibido quando o dispositivo estiver no modo de quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|microphoneForceMute|Booliano|Indica se deve ou não bloquear o mudo do microfone no dispositivo.|
|networkEscapeHatchAllowed|Booliano|Indica se ou não o dispositivo permitirá a conexão com uma conexão de rede temporária no momento da inicialização.|
|nfcBlockOutgoingBeam|Booliano|Indica se deve ou não bloquear feixe de saída NFC.|
|passwordBlockKeyguard|Booliano|Indica se ou não o keyguard está desabilitado.|
|passwordExpirationDays|Int32|Indica a quantidade de tempo em segundos que uma senha pode ser definida para antes que ele expire e uma nova senha será necessária. Valores válidos de 1 a 365|
|passwordMinimumLength|Int32|Indica o comprimento mínimo da senha necessário no dispositivo. Valores válidos de 4 a 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Milissegundos de inatividade antes que os tempos de tela check-out.|
|passwordPreviousPasswordCountToBlock|Int32|Indica o tamanho do histórico de senhas, onde o usuário não será capaz de inserir uma nova senha que é o mesmo que qualquer senha no histórico. Valores válidos de 0 a 24|
|passwordRequiredType|[androidDeviceOwnerRequiredPasswordType](../resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype.md)|Indica a qualidade mínimo da senha necessária no dispositivo. Os valores possíveis são: `deviceDefault`, `required`, `numeric`, `numericComplex`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Indica o número de vezes que um usuário pode digitar uma senha incorreta antes que o dispositivo é apagado. Valores válidos de 4 a 11|
|safeBootBlocked|Booliano|Indica se ou não reinicializar que o dispositivo em inicialização segura está desabilitado.|
|screenCaptureBlocked|Booliano|Indica se ou não desabilitar a capacidade de fazer capturas de tela.|
|securityAllowDebuggingFeatures|Booliano|Indica se deve ou não bloquear o usuário desde a habilitação de recursos de depuração no dispositivo.|
|securityRequireVerifyApps|Booliano|Indica se ou não verifique apps é necessário.|
|statusBarBlocked|Booliano|Indica se o status ou barra estiver desabilitada, incluindo notificações, configurações rápidas e outras camadas da tela.|
|stayOnModes|coleção [androidDeviceOwnerBatteryPluggedMode](../resources/intune-deviceconfig-androiddeviceownerbatterypluggedmode.md)|Lista de modos nos quais a exibição do dispositivo permanecerão ativadas. Essa coleção pode conter um máximo de 4 elementos.|
|storageAllowUsb|Booliano|Indica se deve ou não permitir o armazenamento em massa USB.|
|storageBlockExternalMedia|Booliano|Indica se o bloqueio da mídia externa ou não.|
|storageBlockUsbFileTransfer|Booliano|Indica se o bloqueio da transferência de arquivos USB ou não.|
|systemUpdateWindowStartMinutesAfterMidnight|Int32|Indica o número de minutos após a meia-noite que inicia a janela de atualização do sistema. Valores válidos 0 a 1440|
|systemUpdateWindowEndMinutesAfterMidnight|Int32|Indica o número de minutos após a meia-noite que termine a janela de atualização do sistema. Valores válidos 0 a 1440|
|systemUpdateInstallType|[androidDeviceOwnerSystemUpdateInstallType](../resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype.md)|O tipo de configuração de atualização do sistema. Os valores possíveis são: `deviceDefault`, `postpone`, `windowed`, `automatic`.|
|usersBlockAdd|Booliano|Indica se ou não a adição de usuários e perfis está desabilitado.|
|usersBlockRemove|Booliano|Indica se ou não desabilitar a remoção de outros usuários do dispositivo.|
|volumeBlockAdjustment|Booliano|Indica se ou não ajustar que o volume de mestre está desabilitado.|
|wifiBlockEditConfigurations|Booliano|Indica se deve ou não bloquear as configurações de conexão wifi de edição do usuário.|
|wifiBlockEditPolicyDefinedConfigurations|Booliano|Indica se deve ou não bloquear edição apenas as redes definidas pela política do usuário.|

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
  "microphoneForceMute": true,
  "networkEscapeHatchAllowed": true,
  "nfcBlockOutgoingBeam": true,
  "passwordBlockKeyguard": true,
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
  "usersBlockAdd": true,
  "usersBlockRemove": true,
  "volumeBlockAdjustment": true,
  "wifiBlockEditConfigurations": true,
  "wifiBlockEditPolicyDefinedConfigurations": true
}
```





