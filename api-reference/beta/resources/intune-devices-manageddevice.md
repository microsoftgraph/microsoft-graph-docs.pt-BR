---
title: Tipo de recurso managedDevice
description: Dispositivos gerenciados ou pré-registrados pelo Intune
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ee7fd96654fe0b6c2a95332b87287d3ebff3ad2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995116"
---
# <a name="manageddevice-resource-type"></a>Tipo de recurso managedDevice

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Dispositivos gerenciados ou pré-registrados pelo Intune

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter managedDevice](../api/intune-devices-manageddevice-get.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|Ler propriedades e relações de objetos de [managedDevice](../resources/intune-devices-manageddevice.md).|
|[Atualizar managedDevice](../api/intune-devices-manageddevice-update.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|Atualizar as propriedades de um objeto [managedDevice](../resources/intune-devices-manageddevice.md).|
|[Ação executeAction](../api/intune-devices-manageddevice-executeaction.md)|[bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md)|Ainda não documentado|
|[Ação enableLostMode](../api/intune-devices-manageddevice-enablelostmode.md)|Nenhum|Habilitar modo perdido|
|[Ação playLostModeSound](../api/intune-devices-manageddevice-playlostmodesound.md)|Nenhum|Bloqueio remoto|
|[Ação setDeviceName](../api/intune-devices-manageddevice-setdevicename.md)|Nenhum|Defina o nome do dispositivo.|
|[ação rotateFileVaultKey](../api/intune-devices-manageddevice-rotatefilevaultkey.md)|Nenhuma|Ainda não documentado|
|[função getFileVaultKey](../api/intune-devices-manageddevice-getfilevaultkey.md)|String|Ainda não documentado|
|[Ação retire](../api/intune-devices-manageddevice-retire.md)|Nenhum|Desativar um dispositivo|
|[Ação wipe](../api/intune-devices-manageddevice-wipe.md)|Nenhum|Apagar um dispositivo|
|[Ação resetPasscode](../api/intune-devices-manageddevice-resetpasscode.md)|Nenhum|Redefinir senha|
|[Ação remoteLock](../api/intune-devices-manageddevice-remotelock.md)|Nenhum|Bloqueio remoto|
|[Ação requestRemoteAssistance](../api/intune-devices-manageddevice-requestremoteassistance.md)|Nenhum|Solicitar assistência remota|
|[Ação disableLostMode](../api/intune-devices-manageddevice-disablelostmode.md)|Nenhum|Desabilitar o modo perdido|
|[Ação locateDevice](../api/intune-devices-manageddevice-locatedevice.md)|Nenhum|Localizar um dispositivo|
|[Ação bypassActivationLock](../api/intune-devices-manageddevice-bypassactivationlock.md)|Nenhum|Ignorar bloqueio de ativação|
|[Ação rebootNow](../api/intune-devices-manageddevice-rebootnow.md)|Nenhum|Reiniciar dispositivo|
|[Ação shutDown](../api/intune-devices-manageddevice-shutdown.md)|Nenhum|Desligar dispositivo|
|[Ação recoverPasscode](../api/intune-devices-manageddevice-recoverpasscode.md)|Nenhum|Recuperar senha|
|[Ação cleanWindowsDevice](../api/intune-devices-manageddevice-cleanwindowsdevice.md)|Nenhum|Limpar dispositivo Windows|
|[Ação logoutSharedAppleDeviceActiveUser](../api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser.md)|Nenhum|Sair do usuário ativo no dispositivo Apple compartilhado|
|[Ação deleteUserFromSharedAppleDevice](../api/intune-devices-manageddevice-deleteuserfromsharedappledevice.md)|Nenhum|Excluir o usuário do dispositivo compartilhado da Apple|
|[Ação syncDevice](../api/intune-devices-manageddevice-syncdevice.md)|Nenhuma|Ainda não documentado|
|[Ação windowsDefenderScan](../api/intune-devices-manageddevice-windowsdefenderscan.md)|Nenhuma|Ainda não documentado|
|[Ação windowsDefenderUpdateSignatures](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|Nenhuma|Ainda não documentado|
|[Ação updateWindowsDeviceAccount](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|Nenhuma|Ainda não documentado|
|[Ação revokeAppleVppLicenses](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|Nenhum|Revogar todas as licenças VPP da Apple para um dispositivo|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do dispositivo|
|userId|Cadeia de caracteres|O identificador exclusivo do usuário associado ao dispositivo|
|deviceName|Cadeia de caracteres|Nome do dispositivo|
|hardwareInformation|[hardwareInformation](../resources/intune-devices-hardwareinformation.md)|Os detalhes do hardward para o dispositivo.  Inclui informações como espaço de armazenamento, fabricante, número de série, etc.|
|ownerType|[ownerType](../resources/intune-devices-ownertype.md)|Propriedade do dispositivo. Pode ser "empresa" ou "pessoal". Os valores possíveis são: `unknown`, `company`, `personal`.|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-devices-manageddeviceownertype.md)|Propriedade do dispositivo. Pode ser "empresa" ou "pessoal". Os valores possíveis são: `unknown`, `company`, `personal`.|
|deviceActionResults|Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|Lista de objetos ComplexType deviceActionResult.|
|ManagementState|[ManagementState](../resources/intune-devices-managementstate.md)|Estado de gerenciamento do dispositivo. Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|enrolledDateTime|DateTimeOffset|Hora de registro do dispositivo.|
|lastSyncDateTime|DateTimeOffset|A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune.|
|chassisType|[chassisType](../resources/intune-devices-chassistype.md)|Tipo de chassi do dispositivo. Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.|
|operatingSystem|Cadeia de caracteres|Sistema operacional do dispositivo. Windows, iOS, etc.|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|Plataforma do dispositivo. Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` ,,,,,,,, , `blackberry`, `palm`, `unknown`.|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|Estado de conformidade do dispositivo. Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|jailBroken|String|se o dispositivo está desbloqueado ou modificado.|
|managementAgent|[managementAgentType](../resources/intune-devices-managementagenttype.md)|Canal de gerenciamento do dispositivo. Intune, EAS, etc. Os valores possíveis são `eas`: `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`,.|
|osVersion|String|A versão do sistema operacional do dispositivo.|
|easActivated|Booliano|Se o dispositivo está ativado para Exchange ActiveSync.|
|easDeviceId|String|ID do Exchange ActiveSync do dispositivo.|
|easActivationDateTime|DateTimeOffset|Hora de ativação do Exchange ActiveSync do dispositivo.|
|aadRegistered|Booliano|Se o dispositivo é registrado no Azure Active Directory.|
|azureADRegistered|Booliano|Se o dispositivo é registrado no Azure Active Directory.|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|Tipo de registro do dispositivo. Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|Indica se o modo perdido está habilitado ou desabilitado. Os valores possíveis são: `disabled` e `enabled`.|
|activationLockBypassCode|String|Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado.|
|emailAddress|String|Email(s) do usuário associado ao dispositivo|
|azureActiveDirectoryDeviceId|String|O identificador exclusivo do dispositivo do Azure Active Directory. Somente leitura.|
|azureADDeviceId|String|O identificador exclusivo do dispositivo do Azure Active Directory. Somente leitura.|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|Estado do registro do dispositivo. Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|String|Nome de exibição da categoria do dispositivo|
|isSupervised|Boolean|Status supervisionado do dispositivo|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Última vez em que o dispositivo entrou em contato com o Exchange.|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|O estado de acesso do dispositivo no Exchange. Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|A razão para o estado de acesso do dispositivo no Exchange. Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|String|A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo.|
|remoteAssistanceSessionErrorDetails|String|Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota.|
|isEncrypted|Boolean|Status da criptografia de dispositivo|
|userPrincipalName|String|Nome principal do usuário do dispositivo|
|modelo|String|Modelo do dispositivo|
|fabricante|String|Fabricante do dispositivo|
|imei|String|IMEI|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|DateTime em que o período de cortesia de conformidade do dispositivo termina|
|serialNumber|Cadeia de caracteres|SerialNumber|
|phoneNumber|String|Número de telefone do dispositivo|
|androidSecurityPatchLevel|String|Nível do patch de segurança Android|
|userDisplayName|String|Nome de exibição do usuário|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|Recursos habilitados pelo cliente do ConfigrMgr|
|wiFiMacAddress|String|MAC Wi-Fi|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|O estado do atestado de integridade do dispositivo.|
|subscriberCarrier|String|Operadora do assinante|
|meid|String|MEID|
|totalStorageSpaceInBytes|Int64|Total de armazenamento em bytes|
|freeStorageSpaceInBytes|Int64|Armazenamento gratuito em bytes|
|managedDeviceName|String|Nome gerado automaticamente para identificar um dispositivo. Pode ser substituído por um nome amigável ao usuário.|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo. Somente leitura. Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|retireAfterDateTime|DateTimeOffset|Indica o horário após o momento em que um dispositivo será desativado automaticamente devido à ação agendada.|
|usersLoggedOn|coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)|Indica o último usuário conectado de um dispositivo|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.  Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito. Somente leitura.|
|autopilotEnrolled|Booliano|Relata se o dispositivo gerenciado está inscrito via piloto automático.|
|requireUserEnrollmentApproval|Booliano|Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário.|
|managementCertificateExpirationDate|DateTimeOffset|Relatórios da data de expiração do certificado de gerenciamento de dispositivos|
|iccid|String|Identificador de cartão de circuito integrado, é o número de identificação exclusivo de um cartão SIM.|
|udid|String|Identificador de dispositivo exclusivo para dispositivos iOS e macOS.|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de IDs de marca de escopo para esta instância de dispositivo.|
|windowsActiveMalwareCount|Int32|Contagem de malwares ativos para este dispositivo Windows|
|windowsRemediatedMalwareCount|Int32|Contagem de malware corrigido para este dispositivo Windows|
|notes|String|Observações sobre o dispositivo criado pelo administrador de ti|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|detectedApps|Conjunto [detectedApp](../resources/intune-devices-detectedapp.md)|Todos os aplicativos atualmente instalados no dispositivo|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|Categoria do dispositivo|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|O status de proteção do dispositivo.|
|usuários|Coleção [usuário](../resources/intune-shared-user.md)|Os usuários primários associados ao dispositivo gerenciado.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "String (identifier)",
  "userId": "String",
  "deviceName": "String",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "String",
    "totalStorageSpace": 1024,
    "freeStorageSpace": 1024,
    "imei": "String",
    "meid": "String",
    "manufacturer": "String",
    "model": "String",
    "phoneNumber": "String",
    "subscriberCarrier": "String",
    "cellularTechnology": "String",
    "wifiMac": "String",
    "operatingSystemLanguage": "String",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "String",
        "dataToSync": true,
        "dataQuota": 1024,
        "dataUsed": 1024
      }
    ],
    "tpmSpecificationVersion": "String",
    "operatingSystemEdition": "String",
    "deviceFullQualifiedDomainName": "String",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
    "deviceGuardVirtualizationBasedSecurityState": "String",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
  },
  "ownerType": "String",
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
  "managementState": "String",
  "enrolledDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "chassisType": "String",
  "operatingSystem": "String",
  "deviceType": "String",
  "complianceState": "String",
  "jailBroken": "String",
  "managementAgent": "String",
  "osVersion": "String",
  "easActivated": true,
  "easDeviceId": "String",
  "easActivationDateTime": "String (timestamp)",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "String",
  "lostModeState": "String",
  "activationLockBypassCode": "String",
  "emailAddress": "String",
  "azureActiveDirectoryDeviceId": "String",
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
    "windowsUpdateForBusiness": true,
    "endpointProtection": true,
    "officeApps": true
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
  "partnerReportedThreatState": "String",
  "retireAfterDateTime": "String (timestamp)",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "String",
      "lastLogOnDateTime": "String (timestamp)"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "String (timestamp)",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "String (timestamp)",
  "iccid": "String",
  "udid": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "windowsActiveMalwareCount": 1024,
  "windowsRemediatedMalwareCount": 1024,
  "notes": "String",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "String",
    "errorCode": 1024,
    "lastSyncDateTime": "String (timestamp)"
  }
}
```





