# <a name="androidgeneraldeviceconfiguration-resource-type"></a>Tipo de recurso androidGeneralDeviceConfiguration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso androidGeneralDeviceConfiguration.

Herda de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidGeneralDeviceConfigurations](../api/intune_deviceconfig_androidgeneraldeviceconfiguration_list.md)|Coleção [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md)|Listar propriedades e relações dos objetos [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md).|
|[Obter androidGeneralDeviceConfiguration](../api/intune_deviceconfig_androidgeneraldeviceconfiguration_get.md)|[androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md)|Ler propriedades e relações do objeto [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md).|
|[Criar androidGeneralDeviceConfiguration](../api/intune_deviceconfig_androidgeneraldeviceconfiguration_create.md)|[androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md)|Criar um novo objeto [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md).|
|[Excluir androidGeneralDeviceConfiguration](../api/intune_deviceconfig_androidgeneraldeviceconfiguration_delete.md)|Nenhum|Excluir um [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md).|
|[Atualizar androidGeneralDeviceConfiguration](../api/intune_deviceconfig_androidgeneraldeviceconfiguration_update.md)|[androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md)|Atualizar as propriedades de um objeto [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|appsBlockClipboardSharing|Booliano|Indica se a função de copiar e colar entre aplicativos será bloqueada ou não no compartilhamento de área de transferência.|
|appsBlockCopyPaste|Booliano|Indica se a função de copiar e colar dentro de aplicativos será bloqueada ou não.|
|appsBlockYouTube|Booliano|Indica se o aplicativo YouTube deve ou não ser bloqueado.|
|bluetoothBlocked|Booliano|Indica se o Bluetooth deve ou não ser bloqueado.|
|cameraBlocked|Booliano|Indica se o uso da câmera deve ou não ser bloqueado.|
|cellularBlockDataRoaming|Booliano|Indica se o roaming de dados deve ou não ser bloqueado.|
|cellularBlockMessaging|Booliano|Indica se as mensagens SMS/MMS devem ou não ser bloqueadas.|
|cellularBlockVoiceRoaming|Booliano|Indica se o roaming de voz deve ou não ser bloqueado.|
|cellularBlockWiFiTethering|Booliano|Indica se a sincronização de compartilhamento de Internet por Wi-Fi deve ou não ser bloqueada.|
|compliantAppsList|Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)|Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType). Essa coleção pode conter um máximo de 10.000 elementos.|
|compliantAppListType|[appListType](../resources/intune_deviceconfig_applisttype.md)|Tipo de lista que está em CompliantAppsList. Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|diagnosticDataBlockSubmission|Booliano|Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.|
|locationServicesBlocked|Booliano|Indica se os serviços de localização devem ou não ser bloqueados.|
|googleAccountBlockAutoSync|Booliano|Indica se a sincronização automática do Google deve ou não ser bloqueada.|
|googlePlayStoreBlocked|Booliano|Indica se a Google Play Store deve ou não ser bloqueada.|
|kioskModeBlockSleepButton|Booliano|Indica se o botão de suspensão de tela deve ou não ser bloqueado no modo quiosque.|
|kioskModeBlockVolumeButtons|Booliano|Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.|
|kioskModeApps|Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)|Uma lista de aplicativos que poderão ser executados quando o dispositivo estiver no modo quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|nfcBlocked|Booliano|Indica se a comunicação a curta distância deve ou não ser bloqueada.|
|passwordBlockFingerprintUnlock|Booliano|Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.|
|passwordBlockTrustAgents|Booliano|Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.|
|passwordExpirationDays|Int32|Número de dias antes da expiração da senha. Valores válidos de 1 a 365|
|passwordMinimumLength|Int32|Comprimento mínimo das senhas. Valores válidos de 4 a 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Minutos de inatividade antes que a tela atinja o tempo limite.|
|passwordPreviousPasswordBlockCount|Int32|Número de senhas anteriores para bloquear. Valores válidos de 0 a 24|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Número permitido de falhas de entrada antes da redefinição de fábrica. Valores válidos de 4 a 11|
|passwordRequiredType|[androidRequiredPasswordType](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|Tipo de senha necessário. Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.|
|passwordRequired|Booliano|Indica se uma senha deve ou não ser exigida.|
|powerOffBlocked|Booliano|Indica se o desligamento do dispositivo deve ou não ser bloqueado.|
|factoryResetBlocked|Booliano|Indica se o usuário será ou não impedido de executar uma restauração de fábrica.|
|screenCaptureBlocked|Booliano|Indica se capturas de tela devem ou não ser bloqueadas.|
|deviceSharingAllowed|Booliano|Indica se o modo de compartilhamento do dispositivo deve ou não ser permitido.|
|storageBlockGoogleBackup|Booliano|Indica se o Backup do Google deve ou não ser bloqueado.|
|storageBlockRemovableStorage|Booliano|Indica se o uso do armazenamento removível deve ou não ser bloqueado.|
|storageRequireDeviceEncryption|Booliano|Indica se a criptografia do dispositivo é ou não necessária.|
|storageRequireRemovableStorageEncryption|Booliano|Indica se a criptografia do armazenamento removível é ou não necessária.|
|voiceAssistantBlocked|Booliano|Indica se o uso do Assistente de voz será ou não bloqueado.|
|voiceDialingBlocked|Booliano|Indica se a discagem de voz deve ou não ser bloqueada.|
|webBrowserBlockPopups|Booliano|Indica se as pop-ups dentro do navegador da Web devem ou não ser bloqueadas.|
|webBrowserBlockAutofill|Booliano|Indica se o recurso de preenchimento automático do navegador da Web deve ou não ser bloqueado.|
|webBrowserBlockJavaScript|Booliano|Indica se o JavaScript dentro do navegador da Web deve ou não ser bloqueado.|
|webBrowserBlocked|Booliano|Indica se o navegador da Web deve ou não ser bloqueado.|
|webBrowserCookieSettings|[webBrowserCookieSettings](../resources/intune_deviceconfig_webbrowsercookiesettings.md)|Configuração de cookies do navegador da Web. Os valores possíveis são: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.|
|wiFiBlocked|Booliano|Indica se a sincronização de Wi-Fi deve ou não ser bloqueada.|
|appsInstallAllowList|Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)|Lista de aplicativos que podem ser instalados no dispositivo KNOX. Esta coleção pode conter um máximo de 500 elementos.|
|appsLaunchBlockList|Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)|Lista de aplicativos que não podem ser abertos no dispositivo KNOX. Esta coleção pode conter um máximo de 500 elementos.|
|appsHideList|Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)|Lista de aplicativos que devem ficar ocultos no dispositivo KNOX. Esta coleção pode conter um máximo de 500 elementos.|
|securityRequireVerifyApps|Booliano|Exige que o recurso de verificação de aplicativos Android esteja ativado.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Status de instalação da configuração de dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidGeneralDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "appsBlockClipboardSharing": true,
  "appsBlockCopyPaste": true,
  "appsBlockYouTube": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockMessaging": true,
  "cellularBlockVoiceRoaming": true,
  "cellularBlockWiFiTethering": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "compliantAppListType": "String",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "passwordRequiredType": "String",
  "passwordRequired": true,
  "powerOffBlocked": true,
  "factoryResetBlocked": true,
  "screenCaptureBlocked": true,
  "deviceSharingAllowed": true,
  "storageBlockGoogleBackup": true,
  "storageBlockRemovableStorage": true,
  "storageRequireDeviceEncryption": true,
  "storageRequireRemovableStorageEncryption": true,
  "voiceAssistantBlocked": true,
  "voiceDialingBlocked": true,
  "webBrowserBlockPopups": true,
  "webBrowserBlockAutofill": true,
  "webBrowserBlockJavaScript": true,
  "webBrowserBlocked": true,
  "webBrowserCookieSettings": "String",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "securityRequireVerifyApps": true
}
```



