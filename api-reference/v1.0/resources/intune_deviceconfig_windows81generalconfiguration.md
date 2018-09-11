# <a name="windows81generalconfiguration-resource-type"></a>Tipo de recurso windows81GeneralConfiguration

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Este tópico fornece descrições dos métodos declarados, das propriedades e das relações expostos pelo recurso windows81GeneralConfiguration.

Herda de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windows81GeneralConfigurations](../api/intune_deviceconfig_windows81generalconfiguration_list.md)|Coleção [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)|Lista propriedades e relações dos objetos [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).|
|[Obter windows81GeneralConfiguration](../api/intune_deviceconfig_windows81generalconfiguration_get.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)|Ler propriedades e relações do objeto [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).|
|[Criar windows81GeneralConfiguration](../api/intune_deviceconfig_windows81generalconfiguration_create.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)|Criar um novo objeto [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).|
|[Excluir windows81GeneralConfiguration](../api/intune_deviceconfig_windows81generalconfiguration_delete.md)|Nenhum|Excluir um [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)|
|[Atualizar windows81GeneralConfiguration](../api/intune_deviceconfig_windows81generalconfiguration_update.md)|[windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md)|Atualizar as propriedades de um objeto [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md).|

## <a name="properties"></a>Propriedades
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

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|Coleção [deviceConfigurationAssignment](../resources/intune_deviceconfig_deviceconfigurationassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatuses|Coleção [deviceConfigurationDeviceStatus](../resources/intune_deviceconfig_deviceconfigurationdevicestatus.md)|Status de instalação da configuração do dispositivo por dispositivo. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatuses|Coleção [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md)|Status de instalação da configuração do dispositivo por usuário. Herdado de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceStatusOverview|[deviceConfigurationDeviceOverview](../resources/intune_deviceconfig_deviceconfigurationdeviceoverview.md)|Visão geral de status dos dispositivos na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|userStatusOverview|[deviceConfigurationUserOverview](../resources/intune_deviceconfig_deviceconfigurationuseroverview.md)|Visão geral de status dos usuários na Configuração do dispositivo Herdada de [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Resumo de dispositivo de estado de configuração do dispositivo Herdada do [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceConfiguration",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows81GeneralConfiguration"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
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
  "browserEnterpriseModeSiteListLocation": "String",
  "browserInternetSecurityLevel": "String",
  "browserIntranetSecurityLevel": "String",
  "browserLoggingReportLocation": "String",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "String",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 1024,
  "passwordMinimumLength": 1024,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 1024,
  "passwordMinimumCharacterSetCount": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "passwordRequiredType": "String",
  "passwordSignInFailureCountBeforeFactoryReset": 1024,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "String",
  "workFoldersUrl": "String"
}
```








