---
title: Tipo de recurso windowsManagedDevice
description: Dispositivos Windows gerenciados ou pré-registrados por meio do Intune
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1451a701fd50a8c277905b55f0f1e58c521fc88e
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66667401"
---
# <a name="windowsmanageddevice-resource-type"></a>Tipo de recurso windowsManagedDevice

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Dispositivos Windows gerenciados ou pré-registrados por meio do Intune


Herda de [managedDevice](../resources/intune-devices-manageddevice.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windowsManagedDevices](../api/intune-devices-windowsmanageddevice-list.md)|[coleção windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Listar propriedades e relações dos [objetos windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .|
|[Obter windowsManagedDevice](../api/intune-devices-windowsmanageddevice-get.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Ler propriedades e relações do objeto [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .|
|[Criar windowsManagedDevice](../api/intune-devices-windowsmanageddevice-create.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Crie um novo [objeto windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .|
|[Excluir windowsManagedDevice](../api/intune-devices-windowsmanageddevice-delete.md)|Nenhum|Exclui um [windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md).|
|[Atualizar windowsManagedDevice](../api/intune-devices-windowsmanageddevice-update.md)|[windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md)|Atualize as propriedades de um [objeto windowsManagedDevice](../resources/intune-devices-windowsmanageddevice.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|userId|Cadeia de caracteres|Identificador Exclusivo para o usuário associado ao dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceName|String|Nome do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|hardwareInformation|[hardwareInformation](../resources/intune-devices-hardwareinformation.md)|Os detalhes rígidos do dispositivo.  Inclui informações como espaço de armazenamento, fabricante, número de série etc. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|Ownertype|[Ownertype](../resources/intune-shared-ownertype.md)|Propriedade do dispositivo. Pode ser "empresa" ou "pessoal" Herdado de [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `company`, `personal`.|
|managedDeviceOwnerType|[managedDeviceOwnerType](../resources/intune-shared-manageddeviceownertype.md)|Propriedade do dispositivo. Pode ser "empresa" ou "pessoal" Herdado de [managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `company`, `personal`.|
|deviceActionResults|Coleção [deviceActionResult](../resources/intune-devices-deviceactionresult.md)|Lista de objetos ComplexType deviceActionResult. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|managementState|[managementState](../resources/intune-devices-managementstate.md)|Estado de gerenciamento do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|enrolledDateTime|DateTimeOffset|Hora de registro do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|lastSyncDateTime|DateTimeOffset|A data e a hora da última vez em que o dispositivo concluiu uma sincronização bem-sucedida com o Intune. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|chassisType|[chassisType](../resources/intune-devices-chassistype.md)|Tipo de chassi do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `desktop`, `laptop`, `worksWorkstation`, `enterpriseServer`, `phone`, `tablet`, `mobileOther`, `mobileUnknown`.|
|operatingSystem|String|Sistema operacional do dispositivo. Windows, iOS, etc. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceType|[Devicetype](../resources/intune-devices-devicetype.md)|Plataforma do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: , , , , , , , `winCE`, `iPod``cloudPC``palm``macMDM``blackberry``unix``linux``iSocConsumer``unknown``windows10x``androidnGMS``iPad``chromeOS``androidEnterprise``androidForWork``surfaceHub``holoLens``android``iPhone``winEmbedded`. `windowsPhone``mac``nokia``winMO6``windowsRT``desktop`|
|complianceState|[complianceState](../resources/intune-devices-compliancestate.md)|Estado de conformidade do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.|
|jailBroken|String|se o dispositivo está desbloqueado ou modificado. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|managementAgent|[managementAgentType](../resources/intune-shared-managementagenttype.md)|Canal de gerenciamento do dispositivo. Intune, EAS, etc. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: , , , , , , , `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, , `googleCloudDevicePolicyController`, `msSense``microsoft365ManagedMdm`, . `intuneAosp``configurationManagerClient``easIntuneClient``intuneClient``easMdm``mdm``eas`|
|osVersion|String|A versão do sistema operacional do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivated|Boolean|Se o dispositivo está ativado para Exchange ActiveSync. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|easDeviceId|String|ID do Exchange ActiveSync do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|easActivationDateTime|DateTimeOffset|Hora de ativação do Exchange ActiveSync do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|aadRegistered|Boolean|Se o dispositivo é registrado no Azure Active Directory. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADRegistered|Boolean|Se o dispositivo é registrado no Azure Active Directory. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceEnrollmentType|[deviceEnrollmentType](../resources/intune-devices-deviceenrollmenttype.md)|Tipo de registro do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: , , , , , , , , `windowsBulkUserless``windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, `windowsAzureADJoinUsingDeviceAuth`, `appleUserEnrollment`, , `appleUserEnrollmentWithServiceAccount`, `azureAdJoinUsingAzureVmExtension`, , `androidEnterpriseDedicatedDevice``androidEnterpriseFullyManaged`. `androidEnterpriseCorporateWorkProfile``windowsAzureADJoin``appleBulkWithUser``appleBulkWithoutUser``deviceEnrollmentManager``userEnrollment``unknown`|
|lostModeState|[lostModeState](../resources/intune-devices-lostmodestate.md)|Indica se o modo Perdido está habilitado ou desabilitado. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `disabled` e `enabled`.|
|activationLockBypassCode|String|Código que permite que o Bloqueio de Ativação em um dispositivo seja ignorado. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|emailAddress|String|Email(s) para o usuário associado ao dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|azureActiveDirectoryDeviceId|String|O identificador exclusivo do dispositivo do Azure Active Directory. Somente leitura. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|azureADDeviceId|String|O identificador exclusivo do dispositivo do Azure Active Directory. Somente leitura. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceRegistrationState|[deviceRegistrationState](../resources/intune-devices-deviceregistrationstate.md)|Estado do registro do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceCategoryDisplayName|String|Nome de exibição da categoria de dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|isSupervised|Boolean|Status supervisionado do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeLastSuccessfulSyncDateTime|DateTimeOffset|Última vez em que o dispositivo entrou em contato com o Exchange. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|exchangeAccessState|[deviceManagementExchangeAccessState](../resources/intune-devices-devicemanagementexchangeaccessstate.md)|O estado de acesso do dispositivo no Exchange. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.|
|exchangeAccessStateReason|[deviceManagementExchangeAccessStateReason](../resources/intune-devices-devicemanagementexchangeaccessstatereason.md)|A razão para o estado de acesso do dispositivo no Exchange. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.|
|remoteAssistanceSessionUrl|String|A URL que permite que uma sessão de assistência remota seja estabelecida com o dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|remoteAssistanceSessionErrorDetails|String|Uma cadeia de caracteres de erro que identifica problemas durante a criação de objetos de sessão de Assistência remota. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|isEncrypted|Boolean|Status de criptografia do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|userPrincipalName|String|Nome principal do usuário do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|modelo|String|Modelo do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|fabricante|String|Fabricante do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|imei|String|IMEI. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|O DateTime quando o período de carência de conformidade do dispositivo expira. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|serialNumber|String|Serialnumber. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|phoneNumber|String|Número de telefone do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|androidSecurityPatchLevel|String|Nível de patch de segurança do Android. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|userDisplayName|Cadeia de caracteres|Nome de exibição do usuário. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientEnabledFeatures|[configurationManagerClientEnabledFeatures](../resources/intune-devices-configurationmanagerclientenabledfeatures.md)|Recursos habilitados para cliente do ConfigrMgr. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|wiFiMacAddress|String|Wi-Fi MAC. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceHealthAttestationState|[deviceHealthAttestationState](../resources/intune-devices-devicehealthattestationstate.md)|O estado do atestado de integridade do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|subscriberCarrier|String|Operadora do Assinante. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|meid|String|MEID. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|totalStorageSpaceInBytes|Int64|Armazenamento total em bytes. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|freeStorageSpaceInBytes|Int64|Armazenamento gratuito em bytes. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|managedDeviceName|String|Nome gerado automaticamente para identificar um dispositivo. Pode ser substituído por um nome amigável ao usuário. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|partnerReportedThreatState|[managedDevicePartnerReportedHealthState](../resources/intune-devices-manageddevicepartnerreportedhealthstate.md)|Indica o estado de ameaças de um dispositivo quando um parceiro de Defesa contra ameaças móveis está em uso pela conta e pelo dispositivo. Somente leitura. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, `compromised`, `misconfigured`.|
|retireAfterDateTime|DateTimeOffset|Indica o tempo após o momento em que um dispositivo será desativado automaticamente devido à ação agendada. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|usersLoggedOn|[coleção loggedOnUser](../resources/intune-devices-loggedonuser.md)|Indica os últimos usuários conectados de um dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|preferMdmOverGroupPolicyAppliedDateTime|DateTimeOffset|Relata o DateTime que a configuração preferMdmOverGroupPolicy foi definida.  Quando definido, as Intune de MDM substituirão Política de Grupo configurações se houver um conflito. Somente leitura. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|autopilotEnrolled|Boolean|Relata se o dispositivo gerenciado está registrado por meio do piloto automático. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|requireUserEnrollmentApproval|Boolean|Relata se o dispositivo iOS gerenciado é o registro de aprovação do usuário. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|managementCertificateExpirationDate|DateTimeOffset|Relata a data de validade do certificado de gerenciamento de dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|iccid|Cadeia de caracteres|Identificador de Placa de Circuito Integrado, é o número de identificação exclusivo de um cartão SIM. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|Udid|Cadeia de caracteres|Identificador de Dispositivo Exclusivo para dispositivos iOS e macOS. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de IDs de marca de escopo para esta instância do dispositivo. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsActiveMalwareCount|Int32|Contagem de malware ativo para este dispositivo Windows. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsRemediatedMalwareCount|Int32|Contagem de malware corrigido para este dispositivo Windows. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|notes|String|Observações sobre o dispositivo criado pela ti Administração herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientHealthState|[configurationManagerClientHealthState](../resources/intune-devices-configurationmanagerclienthealthstate.md)|Estado de integridade do cliente do Configuration Manager, válido somente para dispositivos gerenciados pelo agente MDM/ConfigMgr Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|configurationManagerClientInformation|[configurationManagerClientInformation](../resources/intune-devices-configurationmanagerclientinformation.md)|Informações do cliente do Configuration Manager, válidas somente para dispositivos gerenciados, gerenciados por duelo ou trigerenciados pelo Agente do ConfigMgr Herdado de [managedDevice](../resources/intune-devices-manageddevice.md)|
|ethernetMacAddress|Cadeia de caracteres|Ethernet MAC. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|physicalMemoryInBytes|Int64|Memória total em bytes. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|Processorarchitecture|[managedDeviceArchitecture](../resources/intune-devices-manageddevicearchitecture.md)|Arquitetura do processador. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `x86`, `x64`, `arm`, `arM64`.|
|specificationVersion|Cadeia de caracteres|Versão de especificação. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|joinType|[joinType](../resources/intune-devices-jointype.md)|Tipo de junção de dispositivo [herdado de managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `unknown`, `azureADJoined`, `azureADRegistered`, `hybridAzureADJoined`.|
|skuFamily|Cadeia de caracteres|Família de SKU de dispositivo [herdada de managedDevice](../resources/intune-devices-manageddevice.md)|
|skuNumber|Int32|Número de SKU do dispositivo, consulte também: https://docs.microsoft.com/windows/win32/api/sysinfoapi/nf-sysinfoapi-getproductinfo. Valores válidos de 0 a 2147483647. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|managementFeatures|[managedDeviceManagementFeatures](../resources/intune-devices-manageddevicemanagementfeatures.md)|Recursos de gerenciamento de dispositivo herdados [de managedDevice](../resources/intune-devices-manageddevice.md). Os valores possíveis são: `none` e `microsoftManagedDesktop`.|
|chromeOSDeviceInfo|[Coleção chromeOSDeviceProperty](../resources/intune-devices-chromeosdeviceproperty.md)|Lista de propriedades do dispositivo ChromeOS. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|enrollmentProfileName|Cadeia de caracteres|Nome do perfil de registro atribuído ao dispositivo. O valor padrão é uma cadeia de caracteres vazia, indicando que nenhum perfil de registro foi atribuído. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|bootstrapTokenEscrowed|Boolean|Relata se o dispositivo gerenciado tem um token de inicialização escrotado. Isso é apenas para dispositivos macOS. Se FOR FALSO, nenhum token de inicialização será emitido. Se TRUE, o dispositivo escroou um token de inicialização com Intune. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceFirmwareConfigurationInterfaceManaged|Boolean|Indica se o dispositivo é gerenciado pela DFCI. Quando TRUE, o dispositivo é gerenciado pela DFCI. Quando FALSE, o dispositivo não é gerenciado pela DFCI. O valor padrão é FALSO. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|detectedApps|Conjunto [detectedApp](../resources/intune-devices-detectedapp.md)|Todos os aplicativos atualmente instalados no dispositivo Herdados de [managedDevice](../resources/intune-devices-manageddevice.md)|
|deviceCategory|[deviceCategory](../resources/intune-devices-devicecategory.md)|Categoria de dispositivo Herdada [de managedDevice](../resources/intune-devices-manageddevice.md)|
|windowsProtectionState|[windowsProtectionState](../resources/intune-devices-windowsprotectionstate.md)|O status de proteção do dispositivo. Essa propriedade é somente leitura. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|usuários|Coleção [user](../resources/intune-devices-user.md)|Os usuários primários associados ao dispositivo gerenciado. Herdado [de managedDevice](../resources/intune-devices-manageddevice.md)|
|logCollectionRequests|[Coleção deviceLogCollectionResponse](../resources/intune-devices-devicelogcollectionresponse.md)|Lista de solicitações de coleta de log herdadas [de managedDevice](../resources/intune-devices-manageddevice.md)|

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
    "tpmVersion": "String",
    "wiredIPv4Addresses": [
      "String"
    ],
    "batteryLevelPercentage": "4.2",
    "residentUsersCount": 1024,
    "productName": "String",
    "deviceLicensingStatus": "String",
    "deviceLicensingLastErrorCode": 1024,
    "deviceLicensingLastErrorDescription": "String"
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
  "enrollmentProfileName": "String",
  "bootstrapTokenEscrowed": true,
  "deviceFirmwareConfigurationInterfaceManaged": true
}
```




