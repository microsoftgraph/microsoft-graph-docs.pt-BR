# <a name="create-windows81generalconfiguration"></a>Criar windows81GeneralConfiguration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Criar um novo objeto [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).
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
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|Token&gt; de portador obrigatório.&lt;|
|Aceitar|aplicativo/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto windows81GeneralConfiguration.

A tabela a seguir mostra as propriedades que são necessárias ao criar windows81GeneralConfiguration.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|description|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|accountsBlockAddingNonMicrosoftAccountEmail|Booleano|Indica se o usuário será impedido ou não de adicionar ao dispositivo contas de email não associadas a uma conta da Microsoft.|
|applyOnlyToWindows81|Booleano|Valor que indica se esta política se aplica somente ao Windows 8.1. Essa propriedade é somente leitura.|
|browserBlockAutofill|Booleano|Indica se o preenchimento automático deve ou não ser bloqueado.|
|browserBlockAutomaticDetectionOfIntranetSites|Booleano|Indica se a detecção automática de sites da Intranet deve ou não ser bloqueada.|
|browserBlockEnterpriseModeAccess|Booleano|Indica se o acesso ao modo Empresarial deve ou não ser bloqueado.|
|browserBlockJavaScript|Booleano|Indica se o usuário será ou não impedido de usar JavaScript.|
|browserBlockPlugins|Booleano|Indica se os plug-ins devem ou não ser bloqueados.|
|browserBlockPopups|Booleano|Indica se janelas pop-ups devem ou não ser bloqueadas.|
|browserBlockSendingDoNotTrackHeader|Booleano|Indica se o usuário será ou não impedido de enviar o cabeçalho Do Not Track.|
|browserBlockSingleWordEntryOnIntranetSites|Booleano|Indica se a entrada de palavra única em sites da Intranet deve ou não ser bloqueada.|
|browserRequireSmartScreen|Booleano|Indica se o usuário deverá ou não usar o Filtro SmartScreen.|
|browserEnterpriseModeSiteListLocation|Cadeia de caracteres|O local da lista de sites do modo Empresarial. Pode ser um arquivo local, rede local ou local http.|
|browserInternetSecurityLevel|[internetSiteSecurityLevel](../resources/intune_deviceconfig_internetsitesecuritylevel.md)|O nível de segurança da internet. Os valores possíveis são: `userDefined`, `medium`, `mediumHigh`, `high`.|
|browserIntranetSecurityLevel|[siteSecurityLevel](../resources/intune_deviceconfig_sitesecuritylevel.md)|O nível de segurança de Intranet. Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.|
|browserLoggingReportLocation|Cadeia de caracteres|O local do relatório de registro em log.|
|browserRequireHighSecurityForRestrictedSites|Booleano|Indica se a alta segurança para sites restritos deve ou não ser exigida.|
|browserRequireFirewall|Booleano|Indica se um firewall deve ou não ser exigido.|
|browserRequireFraudWarning|Booleano|Indica se um aviso de fraude deve ou não ser exigido.|
|browserTrustedSitesSecurityLevel|[siteSecurityLevel](../resources/intune_deviceconfig_sitesecuritylevel.md)|O nível de segurança de sites confiáveis. Os valores possíveis são: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.|
|cellularBlockDataRoaming|Booleano|Indica se o roaming de dados deve ou não ser bloqueado.|
|diagnosticsBlockDataSubmission|Booleano|Indica se o envio de dados de diagnóstico deve ou não ser bloqueado.|
|passwordBlockPicturePasswordAndPin|Booleano|Indica se o usuário será ou não impedido de usar senha com imagens ou pin.|
|passwordExpirationDays|Int32|Expiração da senha em dias.|
|passwordMinimumLength|Int32|O comprimento mínimo da senha.|
|passwordMinutesOfInactivityBeforeScreenTimeout|Int32|Os minutos de inatividade antes que a tela atinja o tempo limite.|
|passwordMinimumCharacterSetCount|Int32|O número de conjuntos de caracteres necessários na senha.|
|passwordPreviousPasswordBlockCount|Int32|O número de senhas anteriores cujo uso deve ser evitado. Valores válidos de 0 a 24|
|passwordRequiredType|[requiredPasswordType](../resources/intune_deviceconfig_requiredpasswordtype.md)|O tipo de senha necessária. Os valores possíveis são: `deviceDefault`, `alphanumeric`, `numeric`.|
|passwordSignInFailureCountBeforeFactoryReset|Int32|O número de falhas de entrada antes da redefinição de fábrica.|
|storageRequireDeviceEncryption|Booleano|Indica se a criptografia é ou não necessária em um dispositivo móvel.|
|updatesRequireAutomaticUpdates|Booleano|Indica se as atualizações automáticas devem ou não ser exigidas.|
|userAccountControlSettings|[windowsUserAccountControlSettings](../resources/intune_deviceconfig_windowsuseraccountcontrolsettings.md)|As configurações de controle de conta de usuário. Os valores possíveis são: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.|
|workFoldersUrl|Cadeia de caracteres|A URL das pastas de trabalho|



## <a name="response"></a>Resposta
Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1757

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1865

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```








