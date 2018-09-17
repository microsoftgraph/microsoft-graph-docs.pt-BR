# <a name="create-androidworkprofilecompliancepolicy"></a>Criar androidWorkProfileCompliancePolicy

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Criar um novo objeto [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) .
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
POST /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|Token&gt; de portador obrigatório.&lt;|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto androidWorkProfileCompliancePolicy.

A tabela a seguir mostra as propriedades que são necessárias ao criar o androidWorkProfileCompliancePolicy.

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



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidWorkProfileCompliancePolicy](../resources/intune_deviceconfig_androidworkprofilecompliancepolicy.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
Content-type: application/json
Content-length: 1234

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1342

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCompliancePolicy",
  "id": "4e385271-5271-4e38-7152-384e7152384e",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordMinimumLength": 5,
  "passwordRequiredType": "alphabetic",
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordExpirationDays": 6,
  "passwordPreviousPasswordBlockCount": 2,
  "securityPreventInstallAppsFromUnknownSources": true,
  "securityDisableUsbDebugging": true,
  "securityRequireVerifyApps": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "securityBlockJailbrokenDevices": true,
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
  "storageRequireEncryption": true,
  "securityRequireSafetyNetAttestationBasicIntegrity": true,
  "securityRequireSafetyNetAttestationCertifiedDevice": true,
  "securityRequireGooglePlayServices": true,
  "securityRequireUpToDateSecurityProviders": true,
  "securityRequireCompanyPortalAppIntegrity": true
}
```








