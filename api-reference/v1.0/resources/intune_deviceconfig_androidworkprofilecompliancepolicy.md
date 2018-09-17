# <a name="androidworkprofilecompliancepolicy-resource-type"></a>Tipo de recurso de androidWorkProfileCompliancePolicy

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Essa classe contém configurações de conformidade para o Perfil de Trabalho do Android.

Herda de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista androidWorkProfileCompliancePolicies](../api/intune_deviceconfig_androidworkprofilecompliancepolicy_list.md)|Coleção [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md)|Lista propriedades e relacionamentos dos objetos [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md).|
|[Obter androidWorkProfileCompliancePolicy](../api/intune_deviceconfig_androidworkprofilecompliancepolicy_get.md)|[androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md)|Leia as propriedades e os relacionamentos do objeto [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) .|
|[Criar androidWorkProfileCompliancePolicy](../api/intune_deviceconfig_androidworkprofilecompliancepolicy_create.md)|[androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md)|Criar um novo objeto [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) .|
|[Excluir androidWorkProfileCompliancePolicy](../api/intune_deviceconfig_androidworkprofilecompliancepolicy_delete.md)|Nenhum|Exclui uma [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md).|
|[Atualizar androidWorkProfileCompliancePolicy](../api/intune_deviceconfig_androidworkprofilecompliancepolicy_update.md)|[androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md)|Atualizar as propriedades de um objeto [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|descrição|Cadeia de caracteres|O administrador forneceu a descrição da Configuração do dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|versão|Int32|Versão da configuração do dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|passwordRequired|Booleano|Exige uma senha para desbloquear o dispositivo.|
|passwordMinimumLength|Int32|Comprimento mínimo da senha. Valores válidos de 4 a 16|
|passwordRequiredType|[androidRequiredPasswordType](../resources/intune_deviceconfig_androidrequiredpasswordtype.md)|Tipo de caracteres da senha. Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.|
|passwordMinutesOfInactivityBeforeLock|Int32|Minutos de inatividade antes que uma senha seja necessária.|
|passwordExpirationDays|Int32|Número de dias antes da expiração da senha. Valores válidos de 1 a 365|
|passwordPreviousPasswordBlockCount|Int32|Número de senhas anteriores para bloquear.|
|securityPreventInstallAppsFromUnknownSources|Booleano|Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.|
|securityDisableUsbDebugging|Booleano|Desabilite a depuração USB em dispositivos Android.|
|securityRequireVerifyApps|Booleano|Exige que o recurso de verificação de aplicativos Android esteja ativado.|
|deviceThreatProtectionEnabled|Booleano|Exige que os dispositivos tenham habilitada a proteção contra ameaças.|
|deviceThreatProtectionRequiredSecurityLevel|[deviceThreatProtectionLevel](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|Exige o nível mínimo de risco de Proteção contra ameaças móveis para relatar a não conformidade. Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.|
|securityBlockJailbrokenDevices|Booleano|Os dispositivos não podem ser desbloqueados ou modificados.|
|osMinimumVersion|Cadeia de caracteres|Versão mínima do Android.|
|osMaximumVersion|Cadeia de caracteres|Versão máxima do Android.|
|minAndroidSecurityPatchLevel|Cadeia de caracteres|Nível mínimo de patch de segurança Android.|
|storageRequireEncryption|Booleano|Exige criptografia em dispositivos Android.|
|securityRequireSafetyNetAttestationBasicIntegrity|Booleano|Exige que o dispositivo passe na verificação de integridade básica SafetyNet.|
|securityRequireSafetyNetAttestationCertifiedDevice|Booleano|Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.|
|securityRequireGooglePlayServices|Booleano|Exige que os Google Play Services sejam instalados e habilitados no dispositivo.|
|securityRequireUpToDateSecurityProviders|Booleano|Exige que o dispositivo tenha provedores de segurança atualizados. O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.|
|securityRequireCompanyPortalAppIntegrity|Booleano|Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|scheduledActionsForRule|Coleção [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|A lista de ações agendadas para esta regra. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceStatuses|Coleção [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md)|Lista de DeviceComplianceDeviceStatus. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|userStatuses|Coleção [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|Lista de DeviceComplianceUserStatus. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|Visão geral de status de dispositivos para Conformidade de dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|Visão geral de status de usuários para Conformidade de dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Visão geral de dispositivos de estado para Configuração de Conformidade. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|atribuições|Coleção [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|A coleção de atribuições para essa política de conformidade. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.deviceCompliancePolicy",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidWorkProfileCompliancePolicy"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024,
  "passwordRequired": true,
  "passwordMinimumLength": 1024,
  "passwordRequiredType": "String",
  "passwordMinutesOfInactivityBeforeLock": 1024,
  "passwordExpirationDays": 1024,
  "passwordPreviousPasswordBlockCount": 1024,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String",
  "minAndroidSecurityPatchLevel": "String",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```








