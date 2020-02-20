---
title: tipo de recurso windowsManagedDevice
description: Dispositivos Windows que são gerenciados ou previamente registrados pelo Intune
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f83ef22d7ec1af21c264bfbe30967918051f885c
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160253"
---
# <a name="windowsmanageddevice-resource-type"></a>tipo de recurso windowsManagedDevice

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Dispositivos Windows que são gerenciados ou previamente registrados pelo Intune


Herda de [managedDevice](../resources/intune-devices-manageddevice.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsManagedDevices](../api/intune-devices-windowsmanageddevice-list.md)|coleção [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Listar Propriedades e relações dos objetos [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .|
|[Obter windowsManagedDevice](../api/intune-devices-windowsmanageddevice-get.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Leia as propriedades e as relações do objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .|
|[Criar windowsManagedDevice](../api/intune-devices-windowsmanageddevice-create.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Criar um novo objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .|
|[Excluir windowsManagedDevice](../api/intune-devices-windowsmanageddevice-delete.md)|Nenhum|Exclui [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).|
|[Atualizar windowsManagedDevice](../api/intune-devices-windowsmanageddevice-update.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Atualiza as propriedades de um objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo do dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|userId|Cadeia de caracteres|Identificador exclusivo do usuário associado ao dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceName|String|Nome do dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|hardwareInformation|[hardwareInformation](../resources/intune-devices-hardwareinformation.md)|Os detalhes do hardward para o dispositivo.  Inclui informações como espaço de armazenamento, fabricante, número de série, etc. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|Propriedade do dispositivo. Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `company`, `personal`.|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|Propriedade do dispositivo. Pode ser "Company" ou "Personal" herdado de [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `company`, `personal`.|
|deviceActionResults|Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|Lista de objetos ComplexType deviceActionResult. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|ManagementState|[ManagementState](../resources/intune-devices-managementstate.md)|Estado de gerenciamento do dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|enrolledDateTime|DateTimeOffset|Hora de registro do dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|lastSyncDateTime|DateTimeOffset|A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|chassisType|[chassisType](../resources/intune-devices-chassistype.md)|Tipo de chassi do dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.|
|operatingSystem|Cadeia de caracteres|Sistema operacional do dispositivo. Windows, iOS, etc. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceType|[deviceType](../resources/intune-shared-devicetype.md)|Plataforma do dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são `desktop`: `windowsRT`, `winMO6`, `nokia`, `windowsPhone` `mac` `winCE`,,, `winEmbedded`, `iPhone`, `iPad` `iPod` `android`,,, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise` `windows10x` `blackberry` `palm`,,,, `unknown`,,,,,,,,,.|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|Estado de conformidade do dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|jailBroken|String|se o dispositivo está desbloqueado ou modificado. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementAgent|[managementAgentType](../resources/intune-shared-managementagenttype.md)|Canal de gerenciamento do dispositivo. Intune, EAS, etc. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm` e `windowsManagementCloudApi`.|
|osVersion|Cadeia de caracteres|A versão do sistema operacional do dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivated|Booliano|Se o dispositivo está ativado para Exchange ActiveSync. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|easDeviceId|String|ID do Exchange ActiveSync do dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivationDateTime|DateTimeOffset|Hora de ativação do Exchange ActiveSync do dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|aadRegistered|Boolean|Se o dispositivo é registrado no Azure Active Directory. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADRegistered|Boolean|Se o dispositivo é registrado no Azure Active Directory. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-shared-deviceenrollmenttype.md)|Tipo de registro do dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`.|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|Indica se o modo perdido está habilitado ou desabilitado. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `disabled` e `enabled`.|
|activationLockBypassCode|String|Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|emailAddress|String|Email (s) para o usuário associado ao dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureActiveDirectoryDeviceId|String|O identificador exclusivo do dispositivo do Azure Active Directory. Somente leitura. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADDeviceId|String|O identificador exclusivo do dispositivo do Azure Active Directory. Somente leitura. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|Estado do registro do dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|String|Nome de exibição da categoria do dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|isSupervised|Boolean|Status supervisionado de dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Última vez em que o dispositivo entrou em contato com o Exchange. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|O estado de acesso do dispositivo no Exchange. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|A razão para o estado de acesso do dispositivo no Exchange. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|String|A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|remoteAssistanceSessionErrorDetails|String|Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|isEncrypted|Boolean|Status de criptografia de dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|userPrincipalName|String|Nome principal de usuário de dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|modelo|String|Modelo do dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|fabricante|String|O fabricante do dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|imei|String|IMEI. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|O DateTime quando o período de cortesia de conformidade do dispositivo expira. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|serialNumber|Cadeia de caracteres|Autoridade. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|phoneNumber|String|Número de telefone do dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|androidSecurityPatchLevel|String|Nível de patch de segurança do Android. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|userDisplayName|String|Nome de exibição do usuário. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|Recursos habilitados para cliente do ConfigrMgr. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|wiFiMacAddress|String|MAC Wi-Fi. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|O estado do atestado de integridade do dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|subscriberCarrier|String|Operadora de assinante. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|meid|String|MEID. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|totalStorageSpaceInBytes|Int64|Armazenamento total em bytes. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|freeStorageSpaceInBytes|Int64|Armazenamento gratuito em bytes. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|managedDeviceName|String|Nome gerado automaticamente para identificar um dispositivo. Pode ser substituído por um nome amigável ao usuário. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo. Somente leitura. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|retireAfterDateTime|DateTimeOffset|Indica o horário após o momento em que um dispositivo será desativado automaticamente devido à ação agendada. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|usersLoggedOn|coleção [loggedOnUser](../resources/intune-devices-loggedonuser.md)|Indica o último usuário conectado de um dispositivo. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|Reporta o DateTime que a configuração preferMdmOverGroupPolicy foi definida.  Quando definido, as configurações do MDM do Intune substituirão as configurações da política de grupo, se houver um conflito. Somente leitura. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|autopilotEnrolled|Booliano|Relata se o dispositivo gerenciado está inscrito via piloto automático. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|requireUserEnrollmentApproval|Booliano|Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|managementCertificateExpirationDate|DateTimeOffset|Relata a data de validade do certificado de gerenciamento de dispositivos. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|iccid|String|Identificador de cartão de circuito integrado, é o número de identificação exclusivo de um cartão SIM. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|udid|String|Identificador de dispositivo exclusivo para dispositivos iOS e macOS. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de IDs de marca de escopo para esta instância de dispositivo. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsActiveMalwareCount|Int32|Contagem de malware ativo para este dispositivo Windows. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsRemediatedMalwareCount|Int32|Contagem de malware corrigido para este dispositivo Windows. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|notes|String|Observações sobre o dispositivo criado pelo administrador de ti herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientInformation|[configurationManagerClientInformation](../resources/intune-devices-configurationmanagerclientinformation.md)|Informações do cliente do Configuration Manager, válidas apenas para dispositivos gerenciados, Duel ou tri gerenciados pelo agente do ConfigMgr herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|ethernetMacAddress|String|MAC Ethernet. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|physicalMemoryInBytes|Int64|Memória total em bytes. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|processorArchitecture|[managedDeviceArchitecture](../resources/intune-devices-manageddevicearchitecture.md)|Arquitetura do processador. Essa propriedade é somente leitura. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `x86`, `x64`, `arm`, `arM64`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|detectedApps|Conjunto [detectedApp](../resources/intune-devices-detectedapp.md)|Todos os aplicativos atualmente instalados no dispositivo herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|Categoria do dispositivo herdada de [managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|O status de proteção do dispositivo. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|usuários|Coleção [usuário](../resources/intune-shared-user.md)|Os usuários primários associados ao dispositivo gerenciado. Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|

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
    "deviceGuardLocalSystemAuthorityCredentialGuardState": "String",
    "osBuildNumber": "String"
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
  },
  "configurationManagerClientInformation": {
    "@odata.type": "microsoft.graph.configurationManagerClientInformation",
    "clientIdentifier": "String"
  },
  "ethernetMacAddress": "String",
  "physicalMemoryInBytes": 1024,
  "processorArchitecture": "String"
}
```



