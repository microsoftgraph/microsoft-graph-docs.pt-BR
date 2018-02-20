# <a name="androidcompliancepolicy-resource-type"></a>androidCompliancePolicy resource type

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Essa classe contém configurações de conformidade para o Android.

Herda de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar androidCompliancePolicies](../api/intune_deviceconfig_androidcompliancepolicy_list.md)|Coleção [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md)|Lista propriedades e relações dos objetos [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md).|
|[Obter androidCompliancePolicy](../api/intune_deviceconfig_androidcompliancepolicy_get.md)|[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md)|Propriedades de leitura e relações do objeto [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md).|
|[Criar androidCompliancePolicy](../api/intune_deviceconfig_androidcompliancepolicy_create.md)|[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md)|Cria um novo objeto [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md).|
|[Excluir androidCompliancePolicy](../api/intune_deviceconfig_androidcompliancepolicy_delete.md)|Nenhum|Exclui um [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md).|
|[Atualizar androidCompliancePolicy](../api/intune_deviceconfig_androidcompliancepolicy_update.md)|[androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md)|Atualiza as propriedades de um objeto [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|createdDateTime|DateTimeOffset|Data e hora em que o objeto foi criado. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|description|Cadeia de caracteres|Descrição fornecida pelo administrador da Configuração do dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|displayName|Cadeia de caracteres|Nome fornecido pelo administrador da configuração do dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|version|Int32|Versão da configuração do dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|passwordRequired|Booliano|Exige uma senha para desbloquear o dispositivo.|
|passwordMinimumLength|Int32|Comprimento mínimo da senha. Valores válidos de 4 a 16|
|passwordRequiredType|Cadeia de caracteres|Tipo de caracteres na senha Os valores possíveis são: `deviceDefault`, `alphabetic`, `alphanumeric`, `alphanumericWithSymbols`, `lowSecurityBiometric`, `numeric`, `numericComplex`, `any`.|
|passwordMinutesOfInactivityBeforeLock|Int32|Minutos de inatividade antes que uma senha seja necessária.|
|passwordExpirationDays|Int32|Número de dias antes da expiração da senha. Valores válidos de 1 a 365|
|passwordPreviousPasswordBlockCount|Int32|Número de senhas anteriores para bloquear.|
|securityPreventInstallAppsFromUnknownSources|Booliano|Exige que os dispositivos não permitam a instalação de aplicativos de origens desconhecidas.|
|securityDisableUsbDebugging|Booliano|Desabilite a depuração USB em dispositivos Android.|
|securityRequireVerifyApps|Booliano|Exige que o recurso de verificação de aplicativos Android esteja ativado.|
|deviceThreatProtectionEnabled|Booliano|Exige que os dispositivos tenham habilitada a proteção contra ameaças.|
|deviceThreatProtectionRequiredSecurityLevel|Cadeia de caracteres|Exige o nível mínimo de risco de Proteção contra Ameaças Móveis para indicar falta de conformidade. Os valores possíveis são: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.|
|securityBlockJailbrokenDevices|Booliano|Os dispositivos não devem ser violados ou com modificações root.|
|osMinimumVersion|Cadeia de caracteres|Versão mínima do Android.|
|osMaximumVersion|Cadeia de caracteres|Versão máxima do Android.|
|minAndroidSecurityPatchLevel|Cadeia de caracteres|Nível mínimo de patch de segurança Android.|
|storageRequireEncryption|Booliano|Exige criptografia em dispositivos Android.|
|securityRequireSafetyNetAttestationBasicIntegrity|Booliano|Exige que o dispositivo passe na verificação de integridade básica SafetyNet.|
|securityRequireSafetyNetAttestationCertifiedDevice|Booliano|Exige que o dispositivo passe na verificação de dispositivo certificado SafetyNet.|
|securityRequireGooglePlayServices|Booliano|Exige que os Google Play Services sejam instalados e habilitados no dispositivo.|
|securityRequireUpToDateSecurityProviders|Booliano|Exige que o dispositivo tenha provedores de segurança atualizados. O dispositivo exigirá que os Google Play Services sejam habilitados e atualizados.|
|securityRequireCompanyPortalAppIntegrity|Booliano|Exige que o dispositivo passe na verificação de integridade de tempo de execução de aplicativo cliente do Portal da Empresa.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|scheduledActionsForRule|Coleção [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md)|A lista de ações agendadas para esta regra. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceStatuses|Coleção [deviceComplianceDeviceStatus](../resources/intune_deviceconfig_devicecompliancedevicestatus.md)|Lista de DeviceComplianceDeviceStatus. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|userStatuses|Coleção [deviceComplianceUserStatus](../resources/intune_deviceconfig_devicecomplianceuserstatus.md)|Lista de DeviceComplianceUserStatus. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceStatusOverview|[deviceComplianceDeviceOverview](../resources/intune_deviceconfig_devicecompliancedeviceoverview.md)|Visão geral de status de dispositivos para Conformidade de dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|userStatusOverview|[deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md)|Visão geral de status de usuários para Conformidade de dispositivo. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|deviceSettingStateSummaries|Coleção [settingStateDeviceSummary](../resources/intune_deviceconfig_settingstatedevicesummary.md)|Visão geral de dispositivos de estado para Configuração de Conformidade. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|
|assignments|Coleção [deviceCompliancePolicyAssignment](../resources/intune_deviceconfig_devicecompliancepolicyassignment.md)|A coleção de atribuições para essa política de conformidade. Herdado de [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidCompliancePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidCompliancePolicy",
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



