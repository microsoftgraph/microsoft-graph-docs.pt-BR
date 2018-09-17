# <a name="manageddevice-resource-type"></a>Tipo de recurso managedDevice

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Dispositivos gerenciados ou pré-registrados pelo Intune
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedDevices](../api/intune_devices_manageddevice_list.md)|Coleção [managedDevice](../resources/intune_devices_manageddevice.md)|Listar propriedades e relações dos objetos [managedDevice](../resources/intune_devices_manageddevice.md).|
|[Obter managedDevice](../api/intune_devices_manageddevice_get.md)|[managedDevice](../resources/intune_devices_manageddevice.md)|Ler propriedades e relações de objetos de [managedDevice](../resources/intune_devices_manageddevice.md).|
|[Criar managedDevice](../api/intune_devices_manageddevice_create.md)|[managedDevice](../resources/intune_devices_manageddevice.md)|Criar um novo objeto [managedDevice](../resources/intune_devices_manageddevice.md).|
|[Excluir managedDevice](../api/intune_devices_manageddevice_delete.md)|Nenhum|Excluir um [managedDevice](../resources/intune_devices_manageddevice.md)|
|[Atualizar managedDevice](../api/intune_devices_manageddevice_update.md)|[managedDevice](../resources/intune_devices_manageddevice.md)|Atualizar as propriedades de um objeto [managedDevice](../resources/intune_devices_manageddevice.md).|
|[Ação retire](../api/intune_devices_manageddevice_retire.md)|Nenhum|Desativar um dispositivo|
|[Ação wipe](../api/intune_devices_manageddevice_wipe.md)|Nenhum|Apagar um dispositivo|
|[Ação resetPasscode](../api/intune_devices_manageddevice_resetpasscode.md)|Nenhum|Redefinir senha|
|[Ação remoteLock](../api/intune_devices_manageddevice_remotelock.md)|Nenhum|Bloqueio remoto|
|[Ação requestRemoteAssistance](../api/intune_devices_manageddevice_requestremoteassistance.md)|Nenhum|Solicitar assistência remota|
|[Ação disableLostMode](../api/intune_devices_manageddevice_disablelostmode.md)|Nenhum|Desabilitar o modo perdido|
|[Ação locateDevice](../api/intune_devices_manageddevice_locatedevice.md)|Nenhum|Localizar um dispositivo|
|[Ação bypassActivationLock](../api/intune_devices_manageddevice_bypassactivationlock.md)|Nenhum|Ignorar bloqueio de ativação|
|[Ação rebootNow](../api/intune_devices_manageddevice_rebootnow.md)|Nenhum|Reiniciar dispositivo|
|[Ação shutDown](../api/intune_devices_manageddevice_shutdown.md)|Nenhum|Desligar dispositivo|
|[Ação recoverPasscode](../api/intune_devices_manageddevice_recoverpasscode.md)|Nenhum|Recuperar senha|
|[Ação cleanWindowsDevice](../api/intune_devices_manageddevice_cleanwindowsdevice.md)|Nenhum|Limpar dispositivo Windows|
|[Ação logoutSharedAppleDeviceActiveUser](../api/intune_devices_manageddevice_logoutsharedappledeviceactiveuser.md)|Nenhum|Sair do usuário ativo no dispositivo Apple compartilhado|
|[Ação deleteUserFromSharedAppleDevice](../api/intune_devices_manageddevice_deleteuserfromsharedappledevice.md)|Nenhum|Excluir o usuário do dispositivo compartilhado da Apple|
|[Ação syncDevice](../api/intune_devices_manageddevice_syncdevice.md)|Nenhum|Ainda não documentado|
|[Ação windowsDefenderScan](../api/intune_devices_manageddevice_windowsdefenderscan.md)|Nenhum|Ainda não documentado|
|[Ação windowsDefenderUpdateSignatures](../api/intune_devices_manageddevice_windowsdefenderupdatesignatures.md)|Nenhum|Ainda não documentado|
|[Ação updateWindowsDeviceAccount](../api/intune_devices_manageddevice_updatewindowsdeviceaccount.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do dispositivo|
|userId|Cadeia de caracteres|O identificador exclusivo do usuário associado ao dispositivo|
|deviceName|Cadeia de caracteres|Nome do dispositivo|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune_devices_manageddeviceownertype.md)|Propriedade do dispositivo. Pode ser 'empresa' ou 'pessoal'. Os valores possíveis são: , , .`unknown` `company` `personal`|
|deviceActionResults|Coleção [deviceActionResult](../resources/intune_devices_deviceactionresult.md)|Lista de objetos ComplexType deviceActionResult.|
|enrolledDateTime|DateTimeOffset|Hora de registro do dispositivo.|
|lastSyncDateTime|DateTimeOffset|A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.|
|operatingSystem|Cadeia de caracteres|Sistema operacional do dispositivo. Windows, iOS, etc.|
|complianceState|[complianceState](../resources/intune_devices_compliancestate.md)|Estado de conformidade do dispositivo. Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|jailBroken|Cadeia de caracteres|se o dispositivo está desbloqueado ou modificado.|
|managementAgent|[managementAgentType](../resources/intune_devices_managementagenttype.md)|Canal de gerenciamento do dispositivo. Intune, EAS, etc. Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.|
|osVersion|Cadeia de caracteres|A versão do sistema operacional do dispositivo.|
|easActivated|Booleano|Se o dispositivo está ativado para Exchange ActiveSync.|
|easDeviceId|Cadeia de caracteres|ID do Exchange ActiveSync do dispositivo.|
|easActivationDateTime|DateTimeOffset|Hora de ativação do Exchange ActiveSync do dispositivo.|
|azureADRegistered|Booleano|Se o dispositivo é registrado no Azure Active Directory.|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune_shared_deviceenrollmenttype.md)|Tipo de registro do dispositivo. Os valores possíveis são:  `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|activationLockBypassCode|Cadeia de caracteres|Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.|
|emailAddress|Cadeia de caracteres|Email(s) do usuário associado ao dispositivo|
|azureADDeviceId|Cadeia de caracteres|O identificador exclusivo do dispositivo do Azure Active Directory. Somente leitura.|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune_devices_deviceregistrationstate.md)|Estado do registro do dispositivo. Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|Cadeia de caracteres|Nome de exibição da categoria do dispositivo|
|isSupervised|Booleano|Status supervisionado do dispositivo|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Última vez em que o dispositivo entrou em contato com o Exchange.|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune_devices_devicemanagementexchangeaccessstate.md)|O estado de acesso do dispositivo no Exchange. Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune_devices_devicemanagementexchangeaccessstatereason.md)|O motivo do estado de acesso do dispositivo no Exchange. Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|Cadeia de caracteres|A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.|
|remoteAssistanceSessionErrorDetails|Cadeia de caracteres|Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.|
|isEncrypted|Booleano|Status da criptografia de dispositivo|
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário do dispositivo|
|modelo|Cadeia de caracteres|Modelo do dispositivo|
|fabricante|Cadeia de caracteres|Fabricante do dispositivo|
|imei|Cadeia de caracteres|IMEI|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|DateTime em que o período de cortesia de conformidade do dispositivo termina|
|serialNumber|Cadeia de caracteres|SerialNumber|
|phoneNumber|Cadeia de caracteres|Número de telefone do dispositivo|
|androidSecurityPatchLevel|Cadeia de caracteres|Nível do patch de segurança Android|
|userDisplayName|Cadeia de caracteres|Nome de exibição do usuário|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune_devices_configurationmanagerclientenabledfeatures.md)|Recursos habilitados pelo cliente do ConfigrMgr|
|wiFiMacAddress|Cadeia de caracteres|MAC Wi-Fi|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune_devices_devicehealthattestationstate.md)|O estado do atestado de integridade do dispositivo.|
|subscriberCarrier|Cadeia de caracteres|Operadora do assinante|
|meid|Cadeia de caracteres|MEID|
|totalStorageSpaceInBytes|Int64|Total de armazenamento em bytes|
|freeStorageSpaceInBytes|Int64|Armazenamento gratuito em bytes|
|managedDeviceName|Cadeia de caracteres|Nome gerado automaticamente para identificar um dispositivo. Pode ser substituído por um nome amigável ao usuário.|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune_devices_manageddevicepartnerreportedhealthstate.md)|Indica o estado de ameaça de um dispositivo quando um parceiro do Mobile Threat Defense está em uso pela conta e pelo dispositivo. Somente leitura. Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceCategory|[deviceCategory](../resources/intune_shared_devicecategory.md)|Categoria do dispositivo|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)",
  "userId": "String",
  "deviceName": "String",
  "managedDeviceOwnerType": "String",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ],
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "operatingSystem": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureADDeviceId": "String",
  "deviceRegistrationState": "String",
  "deviceCategoryDisplayName": "String",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "String (timestamp)",
  "exchangeAccessState": "String",
  "exchangeAccessStateReason": "String",
  "remoteAssistanceSessionUrl": "String",
  "remoteAssistanceSessionErrorDetails": "String",
  "isEncrypted": true,
  "userPrincipalName": "String",
  "model": "String",
  "manufacturer": "String",
  "imei": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "serialNumber": "String",
  "phoneNumber": "String",
  "androidSecurityPatchLevel": "String",
  "userDisplayName": "String",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "String",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "String",
    "contentNamespaceUrl": "String",
    "deviceHealthAttestationStatus": "String",
    "contentVersion": "String",
    "issuedDateTime": "String (timestamp)",
    "attestationIdentityKey": "String",
    "resetCount": 1024,
    "restartCount": 1024,
    "dataExcutionPolicy": "String",
    "bitLockerStatus": "String",
    "bootManagerVersion": "String",
    "codeIntegrityCheckVersion": "String",
    "secureBoot": "String",
    "bootDebugging": "String",
    "operatingSystemKernelDebugging": "String",
    "codeIntegrity": "String",
    "testSigning": "String",
    "safeMode": "String",
    "windowsPE": "String",
    "earlyLaunchAntiMalwareDriverProtection": "String",
    "virtualSecureMode": "String",
    "pcrHashAlgorithm": "String",
    "bootAppSecurityVersion": "String",
    "bootManagerSecurityVersion": "String",
    "tpmVersion": "String",
    "pcr0": "String",
    "secureBootConfigurationPolicyFingerPrint": "String",
    "codeIntegrityPolicy": "String",
    "bootRevisionListInfo": "String",
    "operatingSystemRevListInfo": "String",
    "healthStatusMismatchInfo": "String",
    "healthAttestationSupportedStatus": "String"
  },
  "subscriberCarrier": "String",
  "meid": "String",
  "totalStorageSpaceInBytes": 1024,
  "freeStorageSpaceInBytes": 1024,
  "managedDeviceName": "String",
  "partnerReportedThreatState": "String"
}
```








