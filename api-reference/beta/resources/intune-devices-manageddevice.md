---
title: Tipo de recurso managedDevice
description: Dispositivos gerenciados ou pré-registrados pelo Intune
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e3634840205a3294519ba65f6f2ecac8d536bf9f
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2022
ms.locfileid: "64630412"
---
# <a name="manageddevice-resource-type"></a>Tipo de recurso managedDevice

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Dispositivos gerenciados ou pré-registrados pelo Intune

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter managedDevice](../api/intune-devices-manageddevice-get.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|Ler propriedades e relações de objetos de [managedDevice](../resources/intune-devices-manageddevice.md).|
|[Atualizar managedDevice](../api/intune-devices-manageddevice-update.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|Atualizar as propriedades de um objeto [managedDevice](../resources/intune-devices-manageddevice.md).|
|[Ação executeAction](../api/intune-devices-manageddevice-executeaction.md)|[bulkManagedDeviceActionResult](../resources/intune-devices-bulkmanageddeviceactionresult.md)|Ainda não documentado|
|[Ação enableLostMode](../api/intune-devices-manageddevice-enablelostmode.md)|Nenhum|Habilitar o modo perdido|
|[Ação playLostModeSound](../api/intune-devices-manageddevice-playlostmodesound.md)|Nenhum|Reproduzir som de modo perdido|
|[Ação setDeviceName](../api/intune-devices-manageddevice-setdevicename.md)|Nenhum|Definir o nome do dispositivo.|
|[Ação activateDeviceEsim](../api/intune-devices-manageddevice-activatedeviceesim.md)|Nenhum|Ative o eSIM no dispositivo.|
|[Ação rotateFileVaultKey](../api/intune-devices-manageddevice-rotatefilevaultkey.md)|Nenhuma|Ainda não documentado|
|[função getFileVaultKey](../api/intune-devices-manageddevice-getfilevaultkey.md)|String|Ainda não documentado|
|[Ação createDeviceLogCollectionRequest](../api/intune-devices-manageddevice-createdevicelogcollectionrequest.md)|[deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Ainda não documentado|
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
|[Ação syncDevice](../api/intune-devices-manageddevice-syncdevice.md)|Nenhum|Ainda não documentado|
|[Ação windowsDefenderScan](../api/intune-devices-manageddevice-windowsdefenderscan.md)|Nenhum|Ainda não documentado|
|[Ação windowsDefenderUpdateSignatures](../api/intune-devices-manageddevice-windowsdefenderupdatesignatures.md)|Nenhum|Ainda não documentado|
|[Ação updateWindowsDeviceAccount](../api/intune-devices-manageddevice-updatewindowsdeviceaccount.md)|Nenhum|Ainda não documentado|
|[Ação revokeAppleVppLicenses](../api/intune-devices-manageddevice-revokeapplevpplicenses.md)|Nenhum|Revogar todas as licenças do Apple Vpp para um dispositivo|
|[Ação rotateBitLockerKeys](../api/intune-devices-manageddevice-rotatebitlockerkeys.md)|Nenhum|Girar BitLockerKeys|
|[ação sendCustomNotificationToCompanyPortal](../api/intune-devices-manageddevice-sendcustomnotificationtocompanyportal.md)|Nenhuma|Ainda não documentado|
|[Ação triggerConfigurationManagerAction](../api/intune-devices-manageddevice-triggerconfigurationmanageraction.md)|Nenhum|Ação de gatilho no cliente ConfigurationManager|
|[Ação de deprovisionamento](../api/intune-devices-manageddevice-deprovision.md)|Nenhuma|Ainda não documentado|
|[desabilitar ação](../api/intune-devices-manageddevice-disable.md)|Nenhuma|Ainda não documentado|
|[Ação reenvelável](../api/intune-devices-manageddevice-reenable.md)|Nenhuma|Ainda não documentado|
|[Ação moveDevicesToOU](../api/intune-devices-manageddevice-movedevicestoou.md)|Nenhuma|Ainda não documentado|
|[função getOemWarranty](../api/intune-devices-manageddevice-getoemwarranty.md)|[oemWarranty](../resources/intune-devices-oemwarranty.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo do dispositivo. Essa propriedade é somente leitura.|
|userId|Cadeia de caracteres|Identificador exclusivo do usuário associado ao dispositivo. Essa propriedade é somente leitura.|
|deviceName|String|Nome do dispositivo. Essa propriedade é somente leitura.|
|hardwareInformation|[hardwareInformation](../resources/intune-devices-hardwareinformation.md)|Os detalhes rígidos do dispositivo.  Inclui informações como espaço de armazenamento, fabricante, número de série etc. Essa propriedade é somente leitura.|
|ownerType|[ownerType](../resources/intune-shared-ownertype.md)|Propriedade do dispositivo. Pode ser "empresa" ou "pessoal". Os valores possíveis são: `unknown`, `company`, `personal`.|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|Propriedade do dispositivo. Pode ser "empresa" ou "pessoal". Os valores possíveis são: `unknown`, `company`, `personal`.|
|deviceActionResults|Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|Lista de objetos ComplexType deviceActionResult. Essa propriedade é somente leitura.|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|Estado de gerenciamento do dispositivo. Essa propriedade é somente leitura. Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|enrolledDateTime|DateTimeOffset|Hora de registro do dispositivo. Essa propriedade é somente leitura.|
|lastSyncDateTime|DateTimeOffset|A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune. Essa propriedade é somente leitura.|
|chassisType|[chassisType](../resources/intune-devices-chassistype.md)|Tipo de chassi do dispositivo. Essa propriedade é somente leitura. Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.|
|operatingSystem|String|Sistema operacional do dispositivo. Windows, iOS, etc. Essa propriedade é somente leitura.|
|deviceType|[deviceType](../resources/intune-devices-devicetype.md)|Plataforma do dispositivo. Essa propriedade é somente leitura. Os valores possíveis são: , , , , `nokia`, `windowsPhone`, `mac`, `iPad`, `linux``cloudPC``macMDM``androidForWork``surfaceHub``palm``androidnGMS``holoLens``chromeOS``windows10x``blackberry``androidEnterprise``unknown``iPod``iSocConsumer``unix``winEmbedded``android``winCE``iPhone``winMO6``windowsRT``desktop`|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|Estado de conformidade do dispositivo. Essa propriedade é somente leitura. Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|jailBroken|String|se o dispositivo está desbloqueado ou modificado. Essa propriedade é somente leitura.|
|managementAgent|[managementAgentType](../resources/intune-devices-managementagenttype.md)|Canal de gerenciamento do dispositivo. Intune, EAS, etc. Essa propriedade é somente leitura. Os valores possíveis são: , , , , , , `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, , `microsoft365ManagedMdm`, `msSense`, `intuneAosp`. `easIntuneClient``intuneClient``easMdm``mdm``eas`|
|osVersion|String|A versão do sistema operacional do dispositivo. Essa propriedade é somente leitura.|
|easActivated|Boolean|Se o dispositivo está ativado para Exchange ActiveSync. Essa propriedade é somente leitura.|
|easDeviceId|String|ID do Exchange ActiveSync do dispositivo. Essa propriedade é somente leitura.|
|easActivationDateTime|DateTimeOffset|Hora de ativação do Exchange ActiveSync do dispositivo. Essa propriedade é somente leitura.|
|aadRegistered|Boolean|Se o dispositivo é registrado no Azure Active Directory. Essa propriedade é somente leitura.|
|azureADRegistered|Boolean|Se o dispositivo é registrado no Azure Active Directory. Essa propriedade é somente leitura.|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-devices-deviceenrollmenttype.md)|Tipo de registro do dispositivo. Essa propriedade é somente leitura. Os valores possíveis são: , , , , , , `windowsAzureADJoin`, , `windowsAutoEnrollment``windowsBulkUserless`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment`, `appleUserEnrollmentWithServiceAccount`, , `azureAdJoinUsingAzureVmExtension`, , `androidEnterpriseFullyManaged``androidEnterpriseCorporateWorkProfile``androidEnterpriseDedicatedDevice`. `appleBulkWithoutUser``appleBulkWithUser``deviceEnrollmentManager``userEnrollment``unknown`|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|Indica se o modo Perdido está habilitado ou desabilitado. Essa propriedade é somente leitura. Os valores possíveis são: `disabled` e `enabled`.|
|activationLockBypassCode|String|Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado. Essa propriedade é somente leitura.|
|emailAddress|String|Email(s) para o usuário associado ao dispositivo. Essa propriedade é somente leitura.|
|azureActiveDirectoryDeviceId|String|O identificador exclusivo do dispositivo do Azure Active Directory. Somente leitura. Essa propriedade é somente leitura.|
|azureADDeviceId|String|O identificador exclusivo do dispositivo do Azure Active Directory. Somente leitura. Essa propriedade é somente leitura.|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|Estado do registro do dispositivo. Essa propriedade é somente leitura. Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|String|Nome de exibição de categoria de dispositivo. Essa propriedade é somente leitura.|
|isSupervised|Boolean|Status supervisionado pelo dispositivo. Essa propriedade é somente leitura.|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Última vez em que o dispositivo entrou em contato com o Exchange. Essa propriedade é somente leitura.|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|O estado de acesso do dispositivo no Exchange. Essa propriedade é somente leitura. Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|A razão para o estado de acesso do dispositivo no Exchange. Essa propriedade é somente leitura. Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|String|A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo. Essa propriedade é somente leitura.|
|remoteAssistanceSessionErrorDetails|String|Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota. Essa propriedade é somente leitura.|
|isEncrypted|Boolean|Status da criptografia do dispositivo. Essa propriedade é somente leitura.|
|userPrincipalName|String|Nome principal do usuário do dispositivo. Essa propriedade é somente leitura.|
|modelo|String|Modelo do dispositivo. Essa propriedade é somente leitura.|
|fabricante|String|Fabricante do dispositivo. Essa propriedade é somente leitura.|
|imei|String|IMEI. Essa propriedade é somente leitura.|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|DateTime quando o período de carência de conformidade do dispositivo expira. Essa propriedade é somente leitura.|
|serialNumber|String|SerialNumber. Essa propriedade é somente leitura.|
|phoneNumber|String|Telefone número do dispositivo. Essa propriedade é somente leitura.|
|androidSecurityPatchLevel|String|Nível de patch de segurança do Android. Essa propriedade é somente leitura.|
|userDisplayName|Cadeia de caracteres|Nome de exibição do usuário. Essa propriedade é somente leitura.|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|Recursos habilitados para cliente ConfigrMgr. Essa propriedade é somente leitura.|
|wiFiMacAddress|String|Wi-Fi MAC. Essa propriedade é somente leitura.|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|O estado do atestado de integridade do dispositivo. Essa propriedade é somente leitura.|
|subscriberCarrier|String|Operadora de Assinantes. Essa propriedade é somente leitura.|
|meid|String|MEID. Essa propriedade é somente leitura.|
|totalStorageSpaceInBytes|Int64|Total Armazenamento em Bytes. Essa propriedade é somente leitura.|
|freeStorageSpaceInBytes|Int64|Free Armazenamento em Bytes. Essa propriedade é somente leitura.|
|managedDeviceName|String|Nome gerado automaticamente para identificar um dispositivo. Pode ser substituído por um nome amigável ao usuário.|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo. Somente leitura. Essa propriedade é somente leitura. Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|retireAfterDateTime|DateTimeOffset|Indica a hora após a resuspensão automática de um dispositivo devido à ação agendada. Essa propriedade é somente leitura.|
|usersLoggedOn|[coleção loggedOnUser](../resources/intune-devices-loggedonuser.md)|Indica o último usuário conectado a um dispositivo. Essa propriedade é somente leitura.|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|Relata que DateTime a configuração preferMdmOverGroupPolicy foi definida.  Quando definido, as configurações Intune MDM substituirão Política de Grupo configurações se houver um conflito. Somente leitura. Essa propriedade é somente leitura.|
|autopilotEnrolled|Booleano|Relata se o dispositivo gerenciado está inscrito por meio de piloto automático. Essa propriedade é somente leitura.|
|requireUserEnrollmentApproval|Boolean|Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário. Essa propriedade é somente leitura.|
|managementCertificateExpirationDate|DateTimeOffset|Relata a data de expiração do certificado de gerenciamento de dispositivo. Essa propriedade é somente leitura.|
|iccid|String|Identificador integrado de cartão de circuito, é o número de identificação exclusivo de um cartão SIM. Essa propriedade é somente leitura.|
|udid|String|Identificador de dispositivo exclusivo para dispositivos iOS e macOS. Essa propriedade é somente leitura.|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de IDs de marca de escopo para esta instância do dispositivo.|
|windowsActiveMalwareCount|Int32|Contagem de malware ativo para este dispositivo windows. Essa propriedade é somente leitura.|
|windowsRemediatedMalwareCount|Int32|Contagem de malwares remediados para este dispositivo windows. Essa propriedade é somente leitura.|
|notes|String|Observações sobre o dispositivo criado pelo administrador de IT|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|Estado de saúde do cliente do gerenciador de configuração, válido somente para dispositivos gerenciados pelo Agente MDM/ConfigMgr|
|configurationManagerClientInformation|[configurationManagerClientInformation](../resources/intune-devices-configurationmanagerclientinformation.md)|Informações do cliente do Gerenciador de Configurações, válidas apenas para dispositivos gerenciados, gerenciados pelo duelar ou gerenciados pelo Agente ConfigMgr|
|ethernetMacAddress|String|Ethernet MAC. Essa propriedade é somente leitura.|
|physicalMemoryInBytes|Int64|Memória total em bytes. Essa propriedade é somente leitura.|
|processorArchitecture|[managedDeviceArchitecture](../resources/intune-devices-manageddevicearchitecture.md)|Arquitetura do processador. Essa propriedade é somente leitura. Os valores possíveis são: `unknown`, `x86`, `x64`, `arm`, `arM64`.|
|specificationVersion|String|Versão de especificação. Essa propriedade é somente leitura.|
|joinType|[joinType](../resources/intune-devices-jointype.md)|Tipo de junção de dispositivo. Os valores possíveis são: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.|
|skuFamily|String|Família sku de dispositivo|
|skuNumber|Int32|Número sku do dispositivo, consulte também: [função GetProductInfo (sysinfoapi.h)](/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo). Valores válidos de 0 a 2147483647. Essa propriedade é somente leitura.|
|managementFeatures|[managedDeviceManagementFeatures](../resources/intune-devices-manageddevicemanagementfeatures.md)|Recursos de gerenciamento de dispositivos. Os valores possíveis são: `none` e `microsoftManagedDesktop`.|
|chromeOSDeviceInfo|[Coleção chromeOSDeviceProperty](../resources/intune-devices-chromeosdeviceproperty.md)|Lista de propriedades do Dispositivo ChromeOS.|
|enrollmentProfileName|String|Nome do perfil de registro atribuído ao dispositivo. O valor padrão é cadeia de caracteres vazia, indicando que nenhum perfil de registro foi assginado. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|detectedApps|Conjunto [detectedApp](../resources/intune-devices-detectedapp.md)|Todos os aplicativos atualmente instalados no dispositivo|
|deviceCategory|[deviceCategory](../resources/intune-shared-devicecategory.md)|Categoria do dispositivo|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|O status de proteção do dispositivo. Essa propriedade é somente leitura.|
|usuários|Coleção [usuário](../resources/intune-shared-user.md)|Os principais usuários associados ao dispositivo gerenciado.|
|logCollectionRequests|[Coleção deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Lista de solicitações de conjunto de log|

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
    "batterySerialNumber": "String",
    "batteryHealthPercentage": 1024,
    "batteryChargeCycles": 1024,
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
    "osBuildNumber": "String",
    "operatingSystemProductType": 1024,
    "ipAddressV4": "String",
    "subnetAddress": "String",
    "esimIdentifier": "String",
    "systemManagementBIOSVersion": "String",
    "tpmManufacturer": "String",
    "tpmVersion": "String"
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
    "clientIdentifier": "String",
    "isBlocked": true
  },
  "ethernetMacAddress": "String",
  "physicalMemoryInBytes": 1024,
  "processorArchitecture": "String",
  "specificationVersion": "String",
  "joinType": "String",
  "skuFamily": "String",
  "skuNumber": 1024,
  "managementFeatures": "String",
  "chromeOSDeviceInfo": [
    {
      "@odata.type": "microsoft.graph.chromeOSDeviceProperty",
      "name": "String",
      "value": "String",
      "valueType": "String",
      "updatable": true
    }
  ],
  "enrollmentProfileName": "String"
}
```




