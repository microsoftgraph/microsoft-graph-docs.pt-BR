# <a name="update-androidgeneraldeviceconfiguration"></a>Atualizar androidGeneralDeviceConfiguration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Atualizar as propriedades de um objeto [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md).
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|Token&gt; de portador obrigatório.&lt;|
|Aceitar|aplicativo/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md).

A tabela a seguir mostra as propriedades que são necessárias ao criar [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|appsBlockClipboardSharing|Booleano|Indica se a função de copiar e colar entre aplicativos será bloqueada ou não no compartilhamento de área de transferência.|
|appsBlockCopyPaste|Booleano|Indica se a função de copiar e colar dentro de aplicativos será bloqueada ou não.|
|appsBlockYouTube|Booleano|Indica se o aplicativo YouTube deve ou não ser bloqueado.|
|bluetoothBlocked|Booleano|Indica se o Bluetooth deve ou não ser bloqueado.|
|cameraBlocked|Booleano|Indica se o uso da câmera deve ou não ser bloqueado.|
|cellularBlockDataRoaming|Booleano|Indica se o roaming de dados deve ou não ser bloqueado.|
|cellularBlockMessaging|Booleano|Indica se as mensagens SMS/MMS devem ou não ser bloqueadas.|
|cellularBlockVoiceRoaming|Booleano|Indica se o roaming de voz deve ou não ser bloqueado.|
|cellularBlockWiFiTethering|Booleano|Indica se a sincronização de compartilhamento de Internet por Wi-Fi deve ou não ser bloqueada.|
|compliantAppsList|Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)|Lista de aplicativos em conformidade (lista de permissões ou lista de bloqueios, controladas por CompliantAppListType). Essa coleção pode conter um máximo de 10.000 elementos.|
|compliantAppListType|[appListType](../resources/intune_deviceconfig_applisttype.md)|Tipo de lista que está na CompliantAppsList. Os valores possíveis são: `none`, `appsInListCompliant`, `appsNotInListCompliant`.|
|diagnosticDataBlockSubmission|Booleano|Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.|
|locationServicesBlocked|Booleano|Indica se os serviços de localização devem ou não ser bloqueados.|
|googleAccountBlockAutoSync|Booleano|Indica se a sincronização automática da conta do Google deve ou não ser bloqueada.|
|googlePlayStoreBlocked|Booleano|Indica se a Google Play Store deve ou não ser bloqueada.|
|kioskModeBlockSleepButton|Booleano|Indica se o botão de suspensão de tela deve ou não ser bloqueado no modo quiosque.|
|kioskModeBlockVolumeButtons|Booleano|Indica se os botões de volume devem ou não ser bloqueados no modo quiosque.|
|kioskModeApps|Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)|Uma lista de aplicativos que poderão ser executados quando o dispositivo estiver no modo quiosque. Esta coleção pode conter um máximo de 500 elementos.|
|nfcBlocked|Booleano|Indica se a comunicação a curta distância deve ou não ser bloqueada.|
|passwordBlockFingerprintUnlock|Booleano|Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.|
|passwordBlockTrustAgents|Booleano|Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.|
|passwordExpirationDays|Int32|Número de dias antes da expiração da senha. Valores válidos de 1 a 365|
|passwordMinimumLength|Int32|Comprimento mínimo das senhas. Valores válidos de 4 a 16|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Minutos de inatividade antes que a tela atinja o tempo limite.|
|passwordPreviousPasswordBlockCount|Int32|Número de senhas anteriores para bloquear. Valores válidos de 0 a 24|
|passwordSignInFailureCountBeforeFactoryReset|Int32|Número permitido de falhas de entrada antes da redefinição de fábrica. Valores válidos de 4 a 11|
|passwordRequiredType|[androidRequiredPasswordType](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|Tipo de senha que é necessário. Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.|
|passwordRequired|Booleano|Indica se uma senha deve ou não ser exigida.|
|powerOffBlocked|Booleano|Indica se o desligamento do dispositivo deve ou não ser bloqueado.|
|factoryResetBlocked|Booleano|Indica se o usuário será ou não impedido de executar uma restauração de fábrica.|
|screenCaptureBlocked|Booleano|Indica se capturas de tela devem ou não ser bloqueadas.|
|deviceSharingAllowed|Booleano|Indica se o modo de compartilhamento do dispositivo deve ou não ser permitido.|
|storageBlockGoogleBackup|Booleano|Indica se o Backup do Google deve ou não ser bloqueado.|
|storageBlockRemovableStorage|Booleano|Indica se o uso do armazenamento removível deve ou não ser bloqueado.|
|storageRequireDeviceEncryption|Booleano|Indica se a criptografia do dispositivo é ou não necessária.|
|storageRequireRemovableStorageEncryption|Booleano|Indica se a criptografia do armazenamento removível é ou não necessária.|
|voiceAssistantBlocked|Booleano|Indica se o uso do Assistente de voz será ou não bloqueado.|
|voiceDialingBlocked|Booleano|Indica se a discagem de voz deve ou não ser bloqueada.|
|webBrowserBlockPopups|Booleano|Indica se os pop-ups dentro do navegador da Web devem ou não ser bloqueados.|
|webBrowserBlockAutofill|Booleano|Indica se o recurso de preenchimento automático do navegador da Web deve ou não ser bloqueado.|
|webBrowserBlockJavaScript|Booleano|Indica se o JavaScript dentro do navegador da Web deve ou não ser bloqueado.|
|webBrowserBlocked|Booleano|Indica se o navegador da Web deve ou não ser bloqueado.|
|webBrowserCookieSettings|[webBrowserCookieSettings](../resources/intune_deviceconfig_webbrowsercookiesettings.md)|Configurações de cookie dentro do navegador da Web. Os valores possíveis são:`browserDefault` , `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.|
|wiFiBlocked|Booleano|Indica se a sincronização de Wi-Fi deve ou não ser bloqueada.|
|appsInstallAllowList|Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)|Lista de aplicativos que podem ser instalados no dispositivo KNOX. Esta coleção pode conter um máximo de 500 elementos.|
|appsLaunchBlockList|Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)|Lista de aplicativos que não podem ser abertos no dispositivo KNOX. Esta coleção pode conter um máximo de 500 elementos.|
|appsHideList|Coleção [appListItem](../resources/intune_deviceconfig_applistitem.md)|Lista de aplicativos que devem ficar ocultos no dispositivo KNOX. Esta coleção pode conter um máximo de 500 elementos.|
|securityRequireVerifyApps|Booleano|Exige que o recurso de verificação de aplicativos Android esteja ativado.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [androidGeneralDeviceConfiguration](../resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3025

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
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
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
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
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3205

{
  "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
  "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
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
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "diagnosticDataBlockSubmission": true,
  "locationServicesBlocked": true,
  "googleAccountBlockAutoSync": true,
  "googlePlayStoreBlocked": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "nfcBlocked": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphabetic",
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
  "webBrowserCookieSettings": "blockAlways",
  "wiFiBlocked": true,
  "appsInstallAllowList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsLaunchBlockList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsHideList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "securityRequireVerifyApps": true
}
```








