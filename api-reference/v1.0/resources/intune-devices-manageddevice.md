---
title: Tipo de recurso managedDevice
description: Dispositivos gerenciados ou pré-registrados pelo Intune
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 11c403f1d64d6cb13684952b93c28d495c5bcf9b563acda42a4859d10322fedf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246763"
---
# <a name="manageddevice-resource-type"></a>Tipo de recurso managedDevice

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Dispositivos gerenciados ou pré-registrados pelo Intune

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedDevices](../api/intune-devices-manageddevice-list.md)|Conjunto [managedDevice](../resources/intune-devices-manageddevice.md)|Listar propriedades e relações dos objetos [managedDevice](../resources/intune-devices-manageddevice.md).|
|[Obter managedDevice](../api/intune-devices-manageddevice-get.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|Ler propriedades e relações de objetos de [managedDevice](../resources/intune-devices-manageddevice.md).|
|[Criar managedDevice](../api/intune-devices-manageddevice-create.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|Criar um novo objeto [managedDevice](../resources/intune-devices-manageddevice.md).|
|[Excluir managedDevice](../api/intune-devices-manageddevice-delete.md)|Nenhum|Excluir um [managedDevice](../resources/intune-devices-manageddevice.md)|
|[Atualizar managedDevice](../api/intune-devices-manageddevice-update.md)|[managedDevice](../resources/intune-devices-manageddevice.md)|Atualizar as propriedades de um objeto [managedDevice](../resources/intune-devices-manageddevice.md).|
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

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do dispositivo. Essa propriedade é somente leitura.|
|userId|Cadeia de caracteres|Identificador exclusivo do usuário associado ao dispositivo. Essa propriedade é somente leitura.|
|deviceName|String|Nome do dispositivo. Essa propriedade é somente leitura.|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-devices-manageddeviceownertype.md)|Propriedade do dispositivo. Pode ser "empresa" ou "pessoal". Os valores possíveis são: `unknown`, `company`, `personal`.|
|deviceActionResults|Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|Lista de objetos ComplexType deviceActionResult. Essa propriedade é somente leitura.|
|enrolledDateTime|DateTimeOffset|Hora de registro do dispositivo. Essa propriedade é somente leitura.|
|lastSyncDateTime|DateTimeOffset|A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune. Essa propriedade é somente leitura.|
|operatingSystem|String|Sistema operacional do dispositivo. Windows, iOS, etc. Essa propriedade é somente leitura.|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|Estado de conformidade do dispositivo. Essa propriedade é somente leitura. Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|jailBroken|String|se o dispositivo está desbloqueado ou modificado. Essa propriedade é somente leitura.|
|managementAgent|[managementAgentType](../resources/intune-devices-managementagenttype.md)|Canal de gerenciamento do dispositivo. Intune, EAS, etc. Essa propriedade é somente leitura. Os valores possíveis são: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.|
|osVersion|String|A versão do sistema operacional do dispositivo. Essa propriedade é somente leitura.|
|easActivated|Boolean|Se o dispositivo está ativado para Exchange ActiveSync. Essa propriedade é somente leitura.|
|easDeviceId|String|ID do Exchange ActiveSync do dispositivo. Essa propriedade é somente leitura.|
|easActivationDateTime|DateTimeOffset|Hora de ativação do Exchange ActiveSync do dispositivo. Essa propriedade é somente leitura.|
|azureADRegistered|Boolean|Se o dispositivo é registrado no Azure Active Directory. Essa propriedade é somente leitura.|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-devices-deviceenrollmenttype.md)|Tipo de registro do dispositivo. Essa propriedade é somente leitura. Os valores possíveis são: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment` e `appleUserEnrollmentWithServiceAccount`.|
|activationLockBypassCode|String|Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado. Essa propriedade é somente leitura.|
|emailAddress|String|Email(s) para o usuário associado ao dispositivo. Essa propriedade é somente leitura.|
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
|userPrincipalName|Cadeia de caracteres|Nome principal do usuário do dispositivo. Essa propriedade é somente leitura.|
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
|iccid|Cadeia de caracteres|Identificador integrado de cartão de circuito, é o número de identificação exclusivo de um cartão SIM. Essa propriedade é somente leitura.|
|udid|String|Identificador de dispositivo exclusivo para dispositivos iOS e macOS. Essa propriedade é somente leitura.|
|notes|String|Observações sobre o dispositivo criado pelo administrador de IT|
|ethernetMacAddress|Cadeia de caracteres|Ethernet MAC. Essa propriedade é somente leitura.|
|physicalMemoryInBytes|Int64|Memória total em bytes. Essa propriedade é somente leitura.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|deviceCategory|[deviceCategory](../resources/intune-devices-devicecategory.md)|Categoria do dispositivo|

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
  "partnerReportedThreatState": "String",
  "iccid": "String",
  "udid": "String",
  "notes": "String",
  "ethernetMacAddress": "String",
  "physicalMemoryInBytes": 1024
}
```




