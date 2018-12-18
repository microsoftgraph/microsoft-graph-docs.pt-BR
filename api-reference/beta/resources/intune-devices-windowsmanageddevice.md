---
title: tipo de recurso de windowsManagedDevice
description: Dispositivos do Windows que são gerenciados ou pre-enrolled por meio de Intune
author: tfitzmac
ms.openlocfilehash: d432e4cdc4552117de56362df0fd632f6bc1719e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328935"
---
# <a name="windowsmanageddevice-resource-type"></a>tipo de recurso de windowsManagedDevice

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Dispositivos do Windows que são gerenciados ou pre-enrolled por meio de Intune

Herda de [managedDevice](../resources/intune-devices-manageddevice.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista windowsManagedDevices](../api/intune-devices-windowsmanageddevice-list.md)|coleção [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Lista as propriedades e os relacionamentos dos objetos [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .|
|[Obter windowsManagedDevice](../api/intune-devices-windowsmanageddevice-get.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Leia as propriedades e os relacionamentos do objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .|
|[Criar windowsManagedDevice](../api/intune-devices-windowsmanageddevice-create.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Crie um novo objeto de [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .|
|[Excluir windowsManagedDevice](../api/intune-devices-windowsmanageddevice-delete.md)|Nenhum|Exclui um [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).|
|[Atualizar windowsManagedDevice](../api/intune-devices-windowsmanageddevice-update.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Atualize as propriedades de um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)|
|userId|String|Identificador exclusivo para o usuário associado ao dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceName|String|Nome do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)|
|hardwareInformation|[hardwareInformation](../resources/intune-devices-hardwareinformation.md)|Os detalhes de hardware do dispositivo.  Inclui informações como o espaço de armazenamento, fabricante, número de série, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|ownerType|[ownerType](../resources/intune-devices-ownertype.md)|Propriedade do dispositivo. Pode ser 'empresa' ou 'pessoal' herdar de [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `company`, `personal`.|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-devices-manageddeviceownertype.md)|Propriedade do dispositivo. Pode ser 'empresa' ou 'pessoal' herdar de [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `company`, `personal`.|
|deviceActionResults|Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|Lista de objetos ComplexType deviceActionResult. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|Estado de gerenciamento do dispositivo. Herdada do [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|enrolledDateTime|DateTimeOffset|Hora de registro do dispositivo. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|lastSyncDateTime|DateTimeOffset|A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|chassisType|[chassisType](../resources/intune-devices-chassistype.md)|Tipo de chassi do dispositivo. Herdada do [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.|
|operatingSystem|String|Sistema operacional do dispositivo. Windows, iOS, etc. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|Plataforma do dispositivo. Herdada do [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` , `blackberry`, `palm`, `unknown`.|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|Estado de conformidade do dispositivo. Herdada do [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|jailBroken|String|se o dispositivo está desbloqueado ou modificado. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementAgent|[managementAgentType](../resources/intune-devices-managementagenttype.md)|Canal de gerenciamento do dispositivo. Intune, EAS, etc. Herdada do [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`.|
|osVersion|String|A versão do sistema operacional do dispositivo. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivated|Boolean|Se o dispositivo está ativado para Exchange ActiveSync. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|easDeviceId|String|ID do Exchange ActiveSync do dispositivo. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivationDateTime|DateTimeOffset|Hora de ativação do Exchange ActiveSync do dispositivo. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|aadRegistered|Boolean|Se o dispositivo é registrado no Azure Active Directory. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADRegistered|Boolean|Se o dispositivo é registrado no Azure Active Directory. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|Tipo de registro do dispositivo. Herdada do [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|Indica se o modo perdido está habilitado ou desabilitada Inherited em [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `disabled` e `enabled`.|
|activationLockBypassCode|String|Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|emailAddress|String|O usuário associado ao dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md) email(s)|
|azureActiveDirectoryDeviceId|String|O identificador exclusivo do dispositivo do Azure Active Directory. Somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADDeviceId|String|O identificador exclusivo do dispositivo do Azure Active Directory. Somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|Estado do registro do dispositivo. Herdada do [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|String|Nome de exibição de categoria dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)|
|isSupervised|Boolean|Status do dispositivo supervisionado Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Última vez em que o dispositivo entrou em contato com o Exchange. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|O estado de acesso do dispositivo no Exchange. Herdada do [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|A razão para o estado de acesso do dispositivo no Exchange. Herdada do [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|String|A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|remoteAssistanceSessionErrorDetails|String|Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|isEncrypted|Boolean|Status de criptografia do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)|
|userPrincipalName|String|Dispositivo nome principal de usuário Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)|
|modelo|String|Modelo do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)|
|fabricante|String|Fabricante do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)|
|imei|String|IMEI herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|A data e hora quando o período de carência de conformidade do dispositivo expiram Inherited do [managedDevice](../resources/intune-devices-manageddevice.md)|
|serialNumber|String|SerialNumber herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|phoneNumber|String|Número de telefone do dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)|
|androidSecurityPatchLevel|String|Nível de patch de segurança Android Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)|
|userDisplayName|String|Nome de exibição do usuário Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|Cliente de ConfigrMgr habilitado recursos Inherited do [managedDevice](../resources/intune-devices-manageddevice.md)|
|wiFiMacAddress|String|Wi-Fi MAC herdada do [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|O estado do atestado de integridade do dispositivo. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|subscriberCarrier|String|Herdado de operadora de assinante de [managedDevice](../resources/intune-devices-manageddevice.md)|
|meid|String|MEID herdados de [managedDevice](../resources/intune-devices-manageddevice.md)|
|totalStorageSpaceInBytes|Int64|Armazenamento total em Bytes herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|freeStorageSpaceInBytes|Int64|Armazenamento gratuito em Bytes herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|managedDeviceName|String|Nome gerado automaticamente para identificar um dispositivo. Pode ser substituído por um nome amigável ao usuário. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo. Somente leitura. Herdada do [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|usersLoggedOn|coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)|Indica o último logon usuários de um dispositivo Inherited da [managedDevice](../resources/intune-devices-manageddevice.md)|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|Relatórios de DateTime que a configuração preferMdmOverGroupPolicy foi definida.  Quando definido, as configurações de Intune MDM substituirão as configurações de diretiva de grupo se não houver um conflito. Somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|autopilotEnrolled|Boolean|Relata se o dispositivo gerenciado está inscrito via piloto automático. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|requireUserEnrollmentApproval|Boolean|Relata se o dispositivo de iOS gerenciado é o registro de aprovação do usuário. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementCertificateExpirationDate|DateTimeOffset|Relatórios de dispositivo gerenciamento data de validade certificado Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)|
|iccid|String|Identificador de cartão de circuito integrado, é o número de identificação exclusiva do cartão de uma SIM. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|UDID|String|Identificador exclusivo do dispositivo para dispositivos iOS e macOS. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|roleScopeTagIds|String collection|Lista de IDs de marca de escopo para essa instância do dispositivo. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsActiveMalwareCount|Int32|Contagem de malware ativos para este dispositivo windows Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsRemediatedMalwareCount|Int32|Contagem de malware remediados por teste para este dispositivo windows Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)|
|Observações|String|Anotações no dispositivo criados pelo administrador de TI herdadas a partir do [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|Configuration manager cliente estado de integridade, válido somente para dispositivos gerenciados pelo MDM/ConfigMgr herdadas de agente do [managedDevice](../resources/intune-devices-manageddevice.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|detectedApps|Conjunto [detectedApp](../resources/intune-devices-detectedapp.md)|Todos os aplicativos instalados no momento no dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|Categoria de dispositivo Inherited de [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|O status de proteção do dispositivo. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
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
  "partnerReportedThreatState": "String",
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





