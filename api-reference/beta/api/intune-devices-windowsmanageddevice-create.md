---
title: Criar windowsManagedDevice
description: Crie um novo objeto de windowsManagedDevice.
author: tfitzmac
ms.openlocfilehash: 21626854a52ed305dbf237562e151e168330f170
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324441"
---
# <a name="create-windowsmanageddevice"></a>Criar windowsManagedDevice

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Crie um novo objeto de [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .
## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Accept|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto windowsManagedDevice.

A tabela a seguir mostra as propriedades que são necessárias quando você cria o windowsManagedDevice.

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



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) no corpo da resposta.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 7173

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "Serial Number value",
    "totalStorageSpace": 1,
    "freeStorageSpace": 0,
    "imei": "Imei value",
    "meid": "Meid value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "phoneNumber": "Phone Number value",
    "subscriberCarrier": "Subscriber Carrier value",
    "cellularTechnology": "Cellular Technology value",
    "wifiMac": "Wifi Mac value",
    "operatingSystemLanguage": "Operating System Language value",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "User Principal Name value",
        "dataToSync": true,
        "dataQuota": 9,
        "dataUsed": 8
      }
    ],
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "operatingSystemEdition": "Operating System Edition value",
    "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
    "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
  },
  "ownerType": "company",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "managementState": "retirePending",
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "chassisType": "desktop",
  "operatingSystem": "Operating System value",
  "deviceType": "windowsRT",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "lostModeState": "enabled",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "User Id value",
      "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "windowsActiveMalwareCount": 9,
  "windowsRemediatedMalwareCount": 13,
  "notes": "Notes value",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "installed",
    "errorCode": 9,
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  }
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 7222

{
  "@odata.type": "#microsoft.graph.windowsManagedDevice",
  "id": "97842b67-2b67-9784-672b-8497672b8497",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "hardwareInformation": {
    "@odata.type": "microsoft.graph.hardwareInformation",
    "serialNumber": "Serial Number value",
    "totalStorageSpace": 1,
    "freeStorageSpace": 0,
    "imei": "Imei value",
    "meid": "Meid value",
    "manufacturer": "Manufacturer value",
    "model": "Model value",
    "phoneNumber": "Phone Number value",
    "subscriberCarrier": "Subscriber Carrier value",
    "cellularTechnology": "Cellular Technology value",
    "wifiMac": "Wifi Mac value",
    "operatingSystemLanguage": "Operating System Language value",
    "isSupervised": true,
    "isEncrypted": true,
    "isSharedDevice": true,
    "sharedDeviceCachedUsers": [
      {
        "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
        "userPrincipalName": "User Principal Name value",
        "dataToSync": true,
        "dataQuota": 9,
        "dataUsed": 8
      }
    ],
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "operatingSystemEdition": "Operating System Edition value",
    "deviceFullQualifiedDomainName": "Device Full Qualified Domain Name value",
    "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "secureBootRequired",
    "deviceGuardVirtualizationBasedSecurityState": "rebootRequired",
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "rebootRequired"
  },
  "ownerType": "company",
  "managedDeviceOwnerType": "company",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "managementState": "retirePending",
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "chassisType": "desktop",
  "operatingSystem": "Operating System value",
  "deviceType": "windowsRT",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "aadRegistered": true,
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "lostModeState": "enabled",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureActiveDirectoryDeviceId": "Azure Active Directory Device Id value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated",
  "usersLoggedOn": [
    {
      "@odata.type": "microsoft.graph.loggedOnUser",
      "userId": "User Id value",
      "lastLogOnDateTime": "2016-12-31T23:58:37.4262708-08:00"
    }
  ],
  "preferMdmOverGroupPolicyAppliedDateTime": "2016-12-31T23:57:34.4649887-08:00",
  "autopilotEnrolled": true,
  "requireUserEnrollmentApproval": true,
  "managementCertificateExpirationDate": "2016-12-31T23:57:59.9789653-08:00",
  "iccid": "Iccid value",
  "udid": "Udid value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "windowsActiveMalwareCount": 9,
  "windowsRemediatedMalwareCount": 13,
  "notes": "Notes value",
  "configurationManagerClientHealthState": {
    "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
    "state": "installed",
    "errorCode": 9,
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
  }
}
```





