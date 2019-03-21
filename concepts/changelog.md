---
title: Log de mudanças do Microsoft Graph
description: Esse log de mudanças cobre o que foi alterado no Microsoft Graph, incluindo as APIs do Microsoft Graph para pontos de extremidade v1.0 e beta.
author: jthake-msft
localization_priority: Priority
ms.openlocfilehash: 3b483efe388887b89a12a99ecea27b1f85753efd
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571421"
---
# <a name="changelog-for-microsoft-graph"></a>Log de mudanças do Microsoft Graph

Esse log de mudanças cobre o que foi alterado no Microsoft Graph, incluindo as APIs do Microsoft Graph para pontos de extremidade v1.0 e beta.

Confira os detalhes sobre problemas conhecidos com as APIs do Microsoft Graph em [problemas conhecidos](known-issues.md).

## <a name="march-2019"></a>Março de 2019

### <a name="microsoft-intune-apis"></a>APIs do Microsoft Intune
|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|beta|Foram adicionadas novas entidades:<br/>[windowsHealthMonitoringConfiguration](/graph/api/resources/intune-deviceconfig-windowshealthmonitoringconfiguration?view=graph-rest-beta)<br/>|
|Adição|beta|Foram adicionados novos tipos complexos:<br/>[windowsFirewallRule](/graph/api/resources/intune-deviceconfig-windowsfirewallrule?view=graph-rest-beta)<br/>|
|Adição|Beta|Foram adicionados novos tipos de enumeração:<br/>[androidManagedAppSafetyNetAppsVerificationType](/graph/api/resources/intune-mam-androidmanagedappsafetynetappsverificationtype?view=graph-rest-beta)<br/>[androidManagedAppSafetyNetDeviceAttestationType](/graph/api/resources/intune-mam-androidmanagedappsafetynetdeviceattestationtype?view=graph-rest-beta)<br/>[windowsAutopilotDeviceType](/graph/api/resources/intune-enrollment-windowsautopilotdevicetype?view=graph-rest-beta)<br/>[windowsFirewallRuleInterfaceTypes](/graph/api/resources/intune-deviceconfig-windowsfirewallruleinterfacetypes?view=graph-rest-beta)<br/>[windowsFirewallRuleNetworkProfileTypes](/graph/api/resources/intune-deviceconfig-windowsfirewallrulenetworkprofiletypes?view=graph-rest-beta)<br/>[windowsFirewallRuleTrafficDirectionType](/graph/api/resources/intune-deviceconfig-windowsfirewallruletrafficdirectiontype?view=graph-rest-beta)<br/>[windowsHealthMonitoringScope](/graph/api/resources/intune-deviceconfig-windowshealthmonitoringscope?view=graph-rest-beta)<br/>[windowsUpdateNotificationDisplayOption](/graph/api/resources/intune-deviceconfig-windowsupdatenotificationdisplayoption?view=graph-rest-beta)<br/>|
|Adição|beta|A ação [searchExistingIdentities](o:searchExistingIdentities:Collection(microsoft.graph.importedDeviceIdentity)) foi adicionada à coleção [importedDeviceIdentity](/graph/api/resources/intune-enrollment-importeddeviceidentity?view=graph-rest-beta) |
|Adição|beta|A ação [assignResourceAccountToDevice](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-assignresourceaccounttodevice?view=graph-rest-beta) foi adicionada a [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) |
|Adição|beta|A ação [unassignResourceAccountFromDevice](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-unassignresourceaccountfromdevice?view=graph-rest-beta) foi adicionada a [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) |
|Exclusão|Beta|Foram removidos os seguintes tipos de enumeração:<br/>**defenderScheduleScanDay**<br/>|
|Adição|beta|As propriedades **requiredAndroidSafetyNetDeviceAttestationType**, **appActionIfAndroidSafetyNetDeviceAttestationFailed**, **requiredAndroidSafetyNetAppsVerificationType** e **appActionIfAndroidSafetyNetAppsVerificationFailed** foram adicionadas à entidade [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta)|
|Adição|beta|A propriedade **supportsOemConfig** foi adicionada à entidade [androidManagedStoreApp](/graph/api/resources/intune-apps-androidmanagedstoreapp?view=graph-rest-beta)|
|Adição|beta|A propriedade **appSupportsOemConfig** foi adicionada à entidade [androidManagedStoreAppConfiguration](/graph/api/resources/intune-apps-androidmanagedstoreappconfiguration?view=graph-rest-beta)|
|Adição|beta|As propriedades **requiredAndroidSafetyNetDeviceAttestationType**, **appActionIfAndroidSafetyNetDeviceAttestationFailed**, **requiredAndroidSafetyNetAppsVerificationType** e **appActionIfAndroidSafetyNetAppsVerificationFailed** foram adicionadas à entidade [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)|
|Adição|beta|As propriedades **iCloudStorageDisabled** e **chooseYourLockScreenDisabled** foram adicionadas à entidade [depMacOSEnrollmentProfile](/graph/api/resources/intune-enrollment-depmacosenrollmentprofile?view=graph-rest-beta)|
|Adição|beta|A propriedade **roleScopeTagIds** foi adicionada à entidade [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade **allowedOutboundClipboardSharingExceptionLength** foi adicionada à entidade [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta)|
|Adição|beta|A propriedade **fastFirstSignIn** foi adicionada à entidade [sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade **tpmRequired** foi adicionada à entidade [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta)|
|Adição|beta|A propriedade **firewallRules** foi adicionada à entidade [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Adição|beta|As propriedades **authenticationWebSignIn**, **privacyDisableLaunchExperience** e **appManagementPackageFamilyNamesToLaunchAfterLogOn** foram adicionadas à entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Exclusão|beta|A propriedade **defenderScheduleScanDay** foi removida da entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade **deviceType** foi adicionada à entidade [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta)|
|Adição|beta|As propriedades **resourceName**, **skuNumber**, **systemFamily**, **azureActiveDirectoryDeviceId** e **managedDeviceId** foram adicionadas à entidade [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)|
|Exclusão|beta|A propriedade **edgeKioskResetAfterIdleTimeInMinutes** foi removida da entidade [windowsKioskConfiguration](/graph/api/resources/intune-deviceconfig-windowskioskconfiguration?view=graph-rest-beta)|
|Adição|beta|As propriedades **userWindowsUpdateScanAccess** e **updateNotificationLevel** foram adicionadas à entidade [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade **teams** foi adicionada ao tipo complexo [excludedApps](/graph/api/resources/intune-apps-excludedapps?view=graph-rest-beta)|
|Adição|beta|A propriedade **autoLaunch** foi adicionada ao tipo complexo [windowsKioskAppBase](/graph/api/resources/intune-deviceconfig-windowskioskappbase?view=graph-rest-beta)|
|Adição|beta|A propriedade **allowAccessToDownloadsFolder** foi adicionada ao tipo complexo [windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta)|
|Adição|beta|O membro **lowSecurityBiometric** foi adicionado ao tipo de enumeração [androidDeviceOwnerRequiredPasswordType](/graph/api/resources/intune-deviceconfig-androiddeviceownerrequiredpasswordtype?view=graph-rest-beta)|
|Adição|beta|Os membros **androidBootloaderUnlocked** e **androidFactoryRomModified** foram adicionados ao tipo de enumeração [managedAppFlaggedReason](/graph/api/resources/intune-mam-managedappflaggedreason?view=graph-rest-beta)|

### <a name="directory-apis"></a>APIs de diretório

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição | v1.0 | Adicione as propriedades **passwordNotificationWindowInDays** e **passwordValidityPeriodInDays** ao recurso do [domínio](/graph/api/resources/domain?view=graph-rest-1.0).|
| Adição | beta e v1.0 | Adicione as propriedades **complianceExpirationDateTime**, **profileType** e **systemLabels** ao recurso do [dispositivo](/graph/api/resources/device?view=graph-rest-1.0).|
| Adição | beta e v1.0 | Adicione a propriedade **isResourceAccount** ao recurso do [usuário](/graph/api/resources/user?view=graph-rest-1.0).|

## <a name="february-2019"></a>Fevereiro de 2019

### <a name="dynamics-365-business-central-api"></a>API Central do Dynamics 365 Business

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | Beta          | Adicionadas APIs financeiras para o Dynamics 365 Business Central. Para saber mais, confira o [Referência da API de finanças](/graph/api/resources/dynamics-graph-reference?view=graph-rest-v1.0).|


## <a name="february-2019"></a>Fevereiro de 2019

### <a name="directory-apis"></a>APIs de diretório

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição | v1.0 | Adicionado novo tipo de recurso [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-1.0). |
| Adição | Beta e v1.0 | Adicionar a propriedade **createdDateTime** na [organização](/graph/api/resources/organization?view=graph-rest-1.0). |
| Alteração | Beta e v1.0 | Atualização da propriedade **companyName** no recurso do [usuário](/graph/api/resources/user?view=graph-rest-1.0) para permitir a gravação. |
| Alteração | beta | O tipo [targetResource](/graph/api/resources/targetresource?view=graph-rest-beta) agora inclui propriedades disponíveis anteriormente para tipos derivados que não são mais compatíveis. |
| Exclusão | beta | Os seguintes tipos de derivadas não são mais compatíveis e foram removidos: **targetResourceDevice**, **targetResourceDirectory**, **targetResourceGroup**, **targetResourcePolicy**, **targetResourceRole**, **targetResourceServicePrincipal**, **targetResourceUser** e **targetResourceOther**. |
| Adição |beta | Adicionar as propriedades **passwordNotificationWindowInDays** e **passwordValidityPeriodInDays** no recurso [domain](/graph/api/resources/domain?view=graph-rest-beta).|

### <a name="education-apis"></a>APIs de educação

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Adição |beta|Adicionada nova propriedade relatedContacts em [educationUser](/graph/api/resources/educationUser?view=graph-rest-beta).|
|Adição |v1.0|Adicionada nova propriedade relatedContacts em [educationUser](/graph/api/resources/educationUser?view=graph-rest-v1.0).|

### <a name="microsoft-intune-apis"></a>APIs do Microsoft Intune

|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|beta|Foram adicionadas novas entidades:<br/>[androidOmaCpConfiguration](/graph/api/resources/intune-deviceconfig-androidomacpconfiguration?view=graph-rest-beta)<br/>[managedDeviceEncryptionState](/graph/api/resources/intune-deviceconfig-manageddeviceencryptionstate?view=graph-rest-beta)<br/>|
|Adição|beta|Foram adicionados novos tipos complexos:<br/>[deliveryOptimizationBandwidth](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidth?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthAbsolute](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthabsolute?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthBusinessHoursLimit](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthbusinesshourslimit?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthHoursWithPercentage](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthhourswithpercentage?view=graph-rest-beta)<br/>[deliveryOptimizationBandwidthPercentage](/graph/api/resources/intune-deviceconfig-deliveryoptimizationbandwidthpercentage?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdCustom](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidcustom?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdSource](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidsource?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdSourceOptions](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidsourceoptions?view=graph-rest-beta)<br/>[deliveryOptimizationMaxCacheSize](/graph/api/resources/intune-deviceconfig-deliveryoptimizationmaxcachesize?view=graph-rest-beta)<br/>[deliveryOptimizationMaxCacheSizeAbsolute](/graph/api/resources/intune-deviceconfig-deliveryoptimizationmaxcachesizeabsolute?view=graph-rest-beta)<br/>[deliveryOptimizationMaxCacheSizePercentage](/graph/api/resources/intune-deviceconfig-deliveryoptimizationmaxcachesizepercentage?view=graph-rest-beta)<br/>[encryptionReportPolicyDetails](/graph/api/resources/intune-deviceconfig-encryptionreportpolicydetails?view=graph-rest-beta)<br/>|
|Adição|Beta|Foram adicionados novos tipos de enumeração:<br/>[advancedBitLockerState](/graph/api/resources/intune-deviceconfig-advancedbitlockerstate?view=graph-rest-beta)<br/>[deliveryOptimizationGroupIdOptionsType](/graph/api/resources/intune-deviceconfig-deliveryoptimizationgroupidoptionstype?view=graph-rest-beta)<br/>[deliveryOptimizationRestrictPeerSelectionByOptions](/graph/api/resources/intune-deviceconfig-deliveryoptimizationrestrictpeerselectionbyoptions?view=graph-rest-beta)<br/>[deviceTypes](/graph/api/resources/intune-deviceconfig-devicetypes?view=graph-rest-beta)<br/>[edgeKioskModeRestrictionType](/graph/api/resources/intune-deviceconfig-edgekioskmoderestrictiontype?view=graph-rest-beta)<br/>[encryptionReadinessState](/graph/api/resources/intune-deviceconfig-encryptionreadinessstate?view=graph-rest-beta)<br/>[encryptionState](/graph/api/resources/intune-deviceconfig-encryptionstate?view=graph-rest-beta)<br/>|
|Adição|beta|A propriedade **roleScopeTagIds** foi adicionada à entidade [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta)|
|Adição|beta|As propriedades **autoFillForceAuthentication**, **cellularBlockPlanModification**, **classroomForceAutomaticallyJoinClasses**, **classroomForceUnpromptedAppAndDeviceLock**, **esimBlockModification**, **proximityBlockSetupToNewDevice**, **softwareUpdatesEnforcedDelayInDays** e **softwareUpdatesForceDelayed** foram adicionadas à entidade [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta)|
|Adição|beta|As propriedades **softwareUpdatesEnforcedDelayInDays**, **softwareUpdatesForceDelayed** e **contentCachingBlocked** foram adicionadas à entidade [macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade **licensingType** foi adicionada à entidade [microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-beta)|
|Adição|beta|As propriedades **defenderSecurityCenterDisableClearTpmUI**, **defenderSecurityCenterDisableNotificationAreaUI**, **defenderSecurityCenterDisableVulnerableTpmFirmwareUpdateUI**, **defenderAdobeReaderLaunchChildProcess** e **defenderOfficeCommunicationAppsLaunchChildProcess** foram adicionadas à entidade [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Adição|beta|As propriedades **edgeKioskModeRestriction**, **edgeKioskResetAfterIdleTimeInMinutes**, **defenderScheduleScanEnableLowCpuPriority**, **defenderDisableCatchupQuickScan**, **defenderDisableCatchupFullScan** e **edgeBlockSearchEngineCustomization** foram adicionadas à entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade **enableWhiteGlove** foi adicionada à entidade [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta)|
|Adição|beta|As propriedades **restrictPeerSelectionBy**, **groupIdSource**, **bandwidthMode**, **backgroundDownloadFromHttpDelayInSeconds**, **foregroundDownloadFromHttpDelayInSeconds**, **minimumRamAllowedToPeerInGigabytes**, **minimumDiskSizeAllowedToPeerInGigabytes**, **minimumFileSizeToCacheInMegabytes**, **minimumBatteryPercentageAllowedToUpload**, **modifyCacheLocation**, **maximumCacheAgeInDays**, **maximumCacheSize** e **vpnPeerCaching** foram adicionadas à entidade [windowsDeliveryOptimizationConfiguration](/graph/api/resources/intune-deviceconfig-windowsdeliveryoptimizationconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade **lastCheckInDateTime** foi adicionada à entidade [windowsInformationProtectionWipeAction](/graph/api/resources/intune-mam-windowsinformationprotectionwipeaction?view=graph-rest-beta)|
|Adição|beta|A propriedade de navegação **managedDeviceEncryptionStates** foi adicionada à entidade [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Adição|beta|As propriedades **endpointProtection** e **officeApps** foram adicionadas ao tipo complexo [configurationManagerClientEnabledFeatures](/graph/api/resources/intune-devices-configurationmanagerclientenabledfeatures?view=graph-rest-beta)|
|Adição|beta|As propriedades **productName** e **publisher** foram adicionadas ao tipo complexo [win32LobAppMsiInformation](/graph/api/resources/intune-apps-win32lobappmsiinformation?view=graph-rest-beta)|
|Adição|beta|O membro **warn** foi adicionado ao tipo enumerado [managedAppRemediationAction](/graph/api/resources/intune-mam-managedappremediationaction?view=graph-rest-beta)|

### <a name="microsoft-teams-apis"></a>APIs do Microsoft Teams

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Adição |Beta e v1.0| Adicionada a propriedade **internalId** ao recurso [team](/graph/api/resources/team?view=graph-rest-v1.0).|
|Adição |Beta e v1.0| Adição de suporte para configuração do Word, Excel, PowerPoint, PDF e para as [guias](teams-configuring-builtin-tabs.md) da biblioteca de documentos. |
|Adição |beta| Introdução da API[Enviar uma mensagem para um canal](/graph/api/channel-post-chatmessage?view=graph-rest-beta). |
|Adição |beta| Introdução da API [Responder a uma mensagem em um canal](/graph/api/channel-post-messagereply?view=graph-rest-beta). |
|Exclusão |beta| Remoção da API POST /teams/{id}/channels/{id}/chatThreads. Em lugar dela, use [Criar uma mensagem em um canal](/graph/api/channel-post-chatmessage?view=graph-rest-beta). |
|Adição |beta | Foi adicionado suporte para permissões do aplicativo para o recurso [installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta).|

### <a name="onenote"></a>OneNote

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | Beta e v1.0 | Adicionar o método [getNotebookFromWebUrl](/graph/api/notebook-getnotebookfromweburl?view=graph-rest-1.0). |

### <a name="outlook-calendar"></a>Calendário do Outlook

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Alteração | Beta | Foi alterado o tipo de dados dos seguintes parâmetros de [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-beta): <br>**participantes**: de **attendeeBase** para [attendeeDataModel](/graph/api/resources/attendeedatamodel?view=graph-rest-beta) <br>**locationConstraint**: de **locationConstraint** para [locationConstraints](/graph/api/resources/locationconstraints?view=graph-rest-beta) <br> **timeConstraint**: de **timeConstraint** para [findMeetingTimesTimeConstraints](/graph/api/resources/findmeetingtimestimeconstraints?view=graph-rest-beta)|
|Alteração | Beta | Foi alterado o tipo de retorno de **findMeetingTimes** de **meetingTimeSuggestionsResult** para [findMeetingTimesResponse](/graph/api/resources/findmeetingtimesresponse?view=graph-rest-beta) |
|Alteração | Beta | Foi alterada a carga de resposta de **findMeetingTimes** para excluir o **tipo** de cada participante que identifica se o participante é obrigatório, opcional ou é um recurso |
|Alteração | Beta | Foi alterado o tipo de base de [locationConstraintItem](/graph/api/resources/locationconstraintitem?view=graph-rest-beta) de [location](/graph/api/resources/location?view=graph-rest-beta) para [locationDataModel](/graph/api/resources/locationdatamodel?view=graph-rest-beta) |
|Alteração | Beta | Foram alterados os tipos de dados das seguintes propriedades de [meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-beta): <br> **attendeeAvailability**: do conjunto de **attendeeAvailability** para a coleção de [attendeeAvailabilityDataModel](/graph/api/resources/attendeeavailabilitydatamodel?view=graph-rest-beta) <br> **locations**: do conjunto de [location](/graph/api/resources/location?view=graph-rest-beta) para coleção de [locationDataModel](/graph/api/resources/locationdatamodel?view=graph-rest-beta) <br> **meetingTimeSlot**: de [timeSlot](/graph/api/resources/timeslot?view=graph-rest-beta) para [meetingTimeSlotDataModel](/graph/api/resources/meetingtimeslotdatamodel?view=graph-rest-beta) <br> **organizerAvailability**: de **freeBusyStatus** para **availabilityStatus** |
|Adição | Beta | Novos tipos complexos: <br> [attendeeAvailabilityDataModel](/graph/api/resources/attendeeavailabilitydatamodel?view=graph-rest-beta) <br> [attendeeDataModel](/graph/api/resources/attendeedatamodel?view=graph-rest-beta) <br> [findMeetingTimesResponse](/graph/api/resources/findmeetingtimesresponse?view=graph-rest-beta) <br> [findMeetingTimesTimeConstraints](/graph/api/resources/findmeetingtimestimeconstraints?view=graph-rest-beta) <br> [locationConstraints](/graph/api/resources/locationconstraints?view=graph-rest-beta) <br> [locationDataModel](/graph/api/resources/locationdatamodel?view=graph-rest-beta) <br> [meetingTimeSlotDataModel](/graph/api/resources/meetingtimeslotdatamodel?view=graph-rest-beta) <br> [postalAddress](/graph/api/resources/postaladdress?view=graph-rest-beta) <br> [searchWindowTimeSlot](/graph/api/resources/searchwindowtimeslot?view=graph-rest-beta)|
|Adição | Beta | Novas enumerações: <br> **addressType** <br> **availabilityStatus** |
|Adição | Beta | Foi adicionada a propriedade **order** a [meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-beta) |
|Exclusão | Beta | Foram removidos os seguintes tipos complexos: <br> **attendeeAvailability** <br> **locationConstraint** <br> **meetingTimeSuggestionsResult** <br>**timeConstraint** |

### <a name="security-apis"></a>APIs de segurança

| **Tipo de alteração** | **Versão** | **Descrição**              |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta       | O indicador de inteligência contra ameaças (TI)[API de segurança](/graph/api/resources/security-api-overview?view=graph-rest-beta) foi adicionado, incluindo os seguintes recursos e operações:<br/>[tiindicator](/graph/api/resources/tiindicator?view=graph-rest-beta) (e entidades relacionadas)<br/> [Obter tiIndicator](/graph/api/tiindicator-get?view=graph-rest-beta)<br/>[Criar tiIndicator](/graph/api/tiindicators-post?view=graph-rest-beta)<br/>[Lista tiIndicators](/graph/api/tiindicators-list?view=graph-rest-beta)<br/>[Atualizar tiIndicator](/graph/api/tiindicator-update?view=graph-rest-beta) <br/>[Excluir tiIndicator](/graph/api/tiindicator-delete?view=graph-rest-beta) <br/>[deleteTiIndicators](/graph/api/tiindicator-deletetiindicators?view=graph-rest-beta) <br/>[deleteTiIndicatorsByExternalId](/graph/api/tiindicator-deletetiindicatorsbyexternalid?view=graph-rest-beta) <br/>[submitTiIndicators](/graph/api/tiindicator-submittiindicators?view=graph-rest-beta) <br/>[updateTiIndicators](/graph/api/tiindicator-updatetiindicators?view=graph-rest-beta)|
| Adição        | Beta       | A ação de segurança de APIs [API de segurança](/graph/api/resources/security-api-overview?view=graph-rest-beta) foi adicionada, incluindo os seguintes recursos e operações:<br/>[securityAction](/graph/api/resources/securityaction?view=graph-rest-beta) (e entidades relacionadas)<br/> [Obter securityAction](/graph/api/securityaction-get?view=graph-rest-beta)<br/>[Criar securityAction](/graph/api/securityactions-post?view=graph-rest-beta)<br/>[Lista securityAction](/graph/api/securityactions-list?view=graph-rest-beta)<br/>[Cancelar securityAction](/graph/api/securityaction-cancelsecurityaction?view=graph-rest-beta)
| Adição        | Beta        | Introduzido um novo tipo complexo de conjunto [historyStates](/graph/api/resources/alerthistorystate?view=graph-rest-beta) para alerta. </br>Adicionada a funcionalidade [updateAlerts](/graph/api/alert-updatealerts?view=graph-rest-beta) para atualizar vários alertas em uma solicitação. |

## <a name="january-2019"></a>Janeiro de 2019

### <a name="azure-ad-apis"></a>APIs do Azure AD

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Adição |v1.0|Introduzido um novo tipo de recurso da entidade [identityProvider](/graph/api/resources/identityprovider?view=graph-rest-v1.0) e as operações [criar](/graph/api/identityprovider-post-identityproviders?view=graph-rest-v1.0), [lista](/graph/api/identityprovider-list?view=graph-rest-v1.0), [obter](/graph/api/identityprovider-get?view=graph-rest-v1.0), [atualizar](/graph/api/identityprovider-update?view=graph-rest-v1.0) e [excluir](/graph/api/identityprovider-delete?view=graph-rest-v1.0).|

### <a name="directory-apis"></a>APIs de Diretório

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição | v1.0 | Adicionado novo método transitiveMembers para [grupos](/graph/api/group-list-transitivemembers?view=graph-rest-1.0). Esse método retorna uma lista simples de membros, inclusive os aninhados.|
| Adição | v1.0 | Adicionado novo método transitiveMemberOf para [usuários](/graph/api/user-list-transitivemembersof?view=graph-rest-1.0), [grupos](/graph/api/group-list-transitivemembersof?view=graph-rest-beta) e [dispositivos](/graph/api/device-list-transitivemembersof?view=graph-rest-1.0).|
| Adição | v1.0 | Adicionadas novas propriedades para [usuários](/graph/api/resources/user?view=graph-rest-1.0): **employeeId**, **faxNumber**, **onPremisesDistinguishedName**, **showInAddressList** e **otherMails**.|
| Adição | v1.0 | Adicionada a propriedade **forceChangePasswordNextSignInWithMfa** para o tipo complexo [passwordProfile](/graph/api/resources/passwordprofile?view=graph-rest-v1.0).|
| Adição | v1.0 | Adicionada a propriedade **licenseAssignmentStates** para a entidade de[usuário](/graph/api/resources/user?view=graph-rest-1.0) para [Licenciamento Baseado em Grupo](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).|
| Adição | v1.0 | Adicionado o recurso **licenseAssignmentState** para [Licenciamento Baseado em Grupo](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).| 
| Adição | v1.0 | Adicionadas as propriedades **assignedLicenses**, **licenseProcessingState**, **hasMembersWithLicenseErrors** e **membersWithLicenseErrors** para o relacionamento da entidade[Grupo ](/graph/api/resources/group?view=graph-rest-1.0) para [Licenciamento Baseado em Grupo](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).|
| Adição | beta | Adicionar a propriedade **createdDateTime** para o recurso [usuário](/graph/api/resources/user?view=graph-rest-beta).|

### <a name="microsoft-intune-apis"></a>APIs do Microsoft Intune

|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|beta|Foram adicionadas novas entidades:<br/>[appleVppTokenTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-applevpptokentroubleshootingevent?view=graph-rest-beta)<br/>[appLogCollectionRequest](/graph/api/resources/intune-devices-applogcollectionrequest?view=graph-rest-beta)<br/>[windowsUpdateState](/graph/api/resources/intune-deviceconfig-windowsupdatestate?view=graph-rest-beta)<br/>|
|Adição|beta|Foram adicionados novos tipos complexos:<br/>[appLogCollectionDownloadDetails](/graph/api/resources/intune-devices-applogcollectiondownloaddetails?view=graph-rest-beta)<br/>**deviceManagementTroubleshootingErrorDetails**<br/>[deviceManagementTroubleshootingErrorResource](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingerrorresource?view=graph-rest-beta)<br/>[win32LobAppAssignmentSettings](/graph/api/resources/intune-apps-win32lobappassignmentsettings?view=graph-rest-beta)<br/>|
|Adição|Beta|Foram adicionados novos tipos de enumeração:<br/>[appLogDecryptionAlgorithm](/graph/api/resources/intune-devices-applogdecryptionalgorithm?view=graph-rest-beta)<br/>[appLogUploadState](/graph/api/resources/intune-devices-apploguploadstate?view=graph-rest-beta)<br/>[win32LobAppNotification](/graph/api/resources/intune-apps-win32lobappnotification?view=graph-rest-beta)<br/>[windowsUpdateStatus](/graph/api/resources/intune-deviceconfig-windowsupdatestatus?view=graph-rest-beta)<br/>|
|Adição|beta|Foi adicionada a ação **createDownloadUrl** no [appLogCollectionRequest](/graph/api/resources/intune-devices-applogcollectionrequest?view=graph-rest-beta) |
|Exclusão|beta|Foram removidas as seguintes entidades:<br/>**deviceManagementApplicabilityRuleOsEdition**<br/>**deviceManagementApplicabilityRuleOsVersion**<br/>|
|Adição|beta|Foi adicionada a propriedade **passwordSignInFailureCountBeforeFactoryReset** à entidade [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta)|
|Adição|beta|Foi adicionada a propriedade **passwordSignInFailureCountBeforeFactoryReset** à entidade [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta)|
|Adição|beta|Foi adicionada a propriedade **passwordSignInFailureCountBeforeFactoryReset** à entidade [androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta)|
|Exclusão|beta|Foi removida a propriedade **defaultProfileDisplayName** da entidade [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta)|
|Adição|beta|Foi adicionada a propriedade **runAs32Bit** à entidade [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta)|
|Adição|beta|Foram adicionadas as propriedades **troubleshootingErrorDetails**, **eventName** e **additionalInformation** à entidade [deviceManagementTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingevent?view=graph-rest-beta)|
|Alteração|beta|Foram alteradas as seguintes propriedades na entidade [macOSCertificateProfileBase](/graph/api/resources/intune-deviceconfig-macoscertificateprofilebase?view=graph-rest-beta):<br/>**subjectAlternativeNameType** de obrigatória para opcional<br/>|
|Adição|beta|Foram adicionadas as propriedades **certificateStore** e **customSubjectAlternativeNames** para a entidade [macOSScepCertificateProfile](/graph/api/resources/intune-deviceconfig-macosscepcertificateprofile?view=graph-rest-beta)|
|Adição|beta|Foi adicionada a propriedade **officeConfigurationXml** à entidade [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta)|
|Adição|beta|Foi adicionada a propriedade **createdDateTime** à entidade [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta)|
|Adição|beta|Foi adicionada a propriedade **bitLockerAllowStandardUserEncryption** à entidade [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Exclusão|beta|Foram removidas as propriedades **localSecurityOptionsEnableAdministratorAccount**, **localSecurityOptionsEnableGuestAccount** e **lanManagerWorkstationEnableInsecureGuestLogons** da entidade [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Adição|beta|Foi adicionada a propriedade **useSecurityKeyForSignin** à entidade [windowsIdentityProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsidentityprotectionconfiguration?view=graph-rest-beta)|
|Adição|beta|Foi adicionada a propriedade de navegação **mobileAppTroubleshootingEvents** à entidade [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade de navegação **appLogCollectionRequests** à entidade [mobileAppTroubleshootingEvent](/graph/api/resources/intune-devices-mobileapptroubleshootingevent?view=graph-rest-beta)|

### <a name="microsoft-teams-apis"></a>APIs do Microsoft Teams

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Adição |beta| EducationStandard, educationClass, educationProfessionalLearningCommunity, educationStaff e unknownFutureValue foram adicionados para a enumeração [teamSpecialization](/graph/api/resources/teamspecialization?view=graph-rest-beta).|

### <a name="reports-apis"></a>APIs de relatórios

| **Tipo de alteração** | **Versão** | **Descrição**                  |
|:----------------|:------------|:-----------------------------------------|
| Adição        | Beta  | Foram adicionadas as propriedades **office365Active** e **office365Inactive** à entrada [office365ServicesUserCounts](/graph/api/resources/office365ServicesUserCounts?view=graph-rest-beta).|

## <a name="december-2018"></a>Dezembro de 2018

### <a name="data-policy-api"></a>API da Política de Dados

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
|Adição |v1.0| Foi adicionada a nova entidade [dataPolicyOperation](/graph/api/resources/datapolicyoperation?view=graph-rest-1.0). Isso representa uma operação de política de dados enviados para fins de acompanhamento.
|Adição |v1.0| Foi adicionada a ação [exportPersonalData](/graph/api/user-exportpersonaldata?view=graph-rest-1.0) em [users](/graph/api/resources/users?view=graph-rest-1.0). Essa ação envia uma solicitação de operação de política de dados para exportar dados pessoais armazenados pela Microsoft para um usuário. |
|Adição |v1.0| Foi adicionado o método [dataPolicyOperations](/graph/api/datapolicyoperation-get?view=graph-rest-1.0). Isso recupera propriedades do objeto dataPolicyOperation.|

### <a name="directory-apis"></a>APIs de diretório

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição | beta | Adicionar a nova propriedade `expirationDateTime` para [grupos](https://docs.microsoft.com/en-us/graph/api/group-list-transitivemembers?view=graph-rest-beta) para [grupo vencimento](https://docs.microsoft.com/pt-BR/azure/active-directory/users-groups-roles/groups-lifecycle).|
| Adição | beta | Adicionado novo tipo de recurso [directoryObjectPartnerReference](/graph/api/resources/directoryobjectpartnerreference?view=graph-rest-beta).|
| Adição | beta | Adicionada a propriedade `createdDateTime` para o recurso [organization](/graph/api/resources/organization?view=graph-rest-beta).|
| Adição | v1.0 | Adicionado método `memberOf` para obter uma direta [associação](/graph/api/resources/device?view=graph-rest-1.0) de [dispositivos](/graph/api/device-list-memberOf?view=graph-rest-1.0). Esse método foi adicionado para obter a lista de associações, incluindo associações aninhadas.|
| Alteração    | Beta | O recurso de [contatos organizacionais](/graph/api/resources/orgcontact?view=graph-rest-beta) foi reestruturado. As propriedades de endereço físico (`city`, `country`, `postalCode`, `streetAddress` e `state`) e `officeLocation` agora estão em uma coleção de `addresses` (do novo tipo de recursos [physicalOfficeAddress](/graph/api/resources/physicalofficeaddress?view=graph-rest-beta)), e `mobilePhone`, `businessPhones` e `faxNumber` agora estão em uma coleção de `phones`. `companyName` e `imAddresses` também foram adicionados|

### <a name="microsoft-teams-apis"></a>APIs do Microsoft Teams

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Adição |beta| Introduzido um novo tipo de recurso [teamsTemplate](/graph/api/resources/teamstemplate?view=graph-rest-beta).|
|Adição |beta| Introduzido um novo tipo de recurso [teamsSpecialization](/graph/api/resources/teamspecialization?view=graph-rest-beta).|
|Adição |beta| Adicionadas as propriedades isFavoriteByDefault, email e webUrl para o[canal](/graph/api/resources/channel?view=graph-rest-beta).|
|Adição |beta| Adicionou a propriedade displayName a [equipe](/graph/api/resources/team?view=graph-rest-beta).|
|Adição |beta| Adicionou a propriedade de descrição a [equipe](/graph/api/resources/team?view=graph-rest-beta).|
|Adição |beta| Adicionou a propriedade classificação a [equipe](/graph/api/resources/team?view=graph-rest-beta).|
|Adição |beta| Adicionou a propriedade [especialização](/graph/api/resources/teamspecialization?view=graph-rest-beta) a [equipe](/graph/api/resources/team?view=graph-rest-beta).|
|Adição |beta| Adicionou a propriedade [visibilidade](/graph/api/resources/teamvisibilitytype?view=graph-rest-beta) a [equipe](/graph/api/resources/team?view=graph-rest-beta).|
|Adição |beta| Adicionou a propriedade [modelo](/graph/api/resources/teamstemplate?view=graph-rest-beta) a [equipe](/graph/api/resources/team?view=graph-rest-beta).|
|Adição |beta| Adicionado o conjunto de proprietários [equipe](/graph/api/resources/team?view=graph-rest-beta).|
|Adição |beta| Apresentamos a nova enumeração do membro unknownFutureValue para teamVisibilityType.|
|Adição |beta| Apresentamos a nova enumeração do membro unknownFutureValue para giphyRatingType.|
|Adição |beta| Apresentamos a nova enumeração do membro unknownFutureValue para teamsAsyncOperationType.|
|Adição |beta| Apresentamos a nova enumeração do membro unknownFutureValue para teamsAsyncOperationStatus.|
|Adição |beta| Apresentamos a nova enumeração do membro unknownFutureValue para teamsAppDistributionMethod.|
|Adição |beta| Introduzido um novo recurso [/teamsTemplates](/graph/api/resources/teamstemplate?view=graph-rest-beta).|
|Adição | v1.0 | Adicionado suporte para permissões de administrador às operações de [team](/graph/api/resources/team?view=graph-rest-1.0), [channel](/graph/api/resources/channel?view=graph-rest-1.0) e [tab](/graph/api/resources/teamstab?view=graph-rest-1.0). |

### <a name="privileged-identity-management-apis"></a>APIs de Privileged Identity Management

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição | beta | Adicionada a propriedade `registeredRoot` à entidade[governanceResource](/graph/api/resources/governanceresource?view=graph-rest-beta).|
| Alteração | beta | Renomeada a propriedade `onboardDateTime` na entidade[governanceResource](/graph/api/resources/governanceresource?view=graph-rest-beta) para `registeredDateTime`.|
| Adição | beta | Adicionada a nova ação [Registre-se o recurso](/graph/api/governanceresource-register?view=graph-rest-beta).|
| Remoção | beta | Remover a entidade `isPermanent` propriedade no [governanceRoleAssignment](/graph/api/resources/governanceroleassignment?view=graph-rest-beta).|
| Remoção | beta | Remover a entidade `roleAssignmentStartDateTime` propriedade no [governanceRoleAssignmentRequest](/graph/api/resources/governanceroleassignmentrequest?view=graph-rest-beta).|
| Remoção | beta | Remover a entidade `roleAssignmentEndDateTime` propriedade no [governanceRoleAssignmentRequest](/graph/api/resources/governanceroleassignmentrequest?view=graph-rest-beta).|

### <a name="security-apis"></a>APIs de segurança

| **Tipo de alteração** | **Versão** | **Descrição**              |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Introduzido um novo tipo complexo [complianceInformation](/graph/api/complianceInformation/team?view=graph-rest-beta).|
| Adição        | Beta        | Introduzido um novo tipo complexo [certificationControl](/graph/api/certificationControl/team?view=graph-rest-beta).|

## <a name="november-2018"></a>Novembro de 2018

### <a name="data-policy-operations-api"></a>API de Operações de Política de Dados

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | beta        | Adicionada nova propriedade **progress** a [dataPolicyOperation](/graph/api/resources/dataPolicyOperation?view=graph-rest-beta). Isso especifica o progresso de uma operação.

### <a name="directory-apis"></a>APIs de Diretório

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição | v1.0 | Adicionada a ação [forceDelete](/graph/api/domain-forcedelete?view=graph-rest-1.0) aos [domínios](/graph/api/resources/domain?view=graph-rest-1.0).|
| Adição | beta | Adicionado novo método transitiveMembers em [grupos](/graph/api/group-list-transitivemembers?view=graph-rest-beta). Esse método retorna uma lista simples de membros, inclusive os aninhados.|
| Adição | beta | Adicionado novo método transitiveMemberOf em [usuários](/graph/api/user-list-transitivemembersof?view=graph-rest-beta), [grupos](/graph/api/group-list-transitivemembersof?view=graph-rest-beta), [dispositivos](/graph/api/device-list-transitivemembersof?view=graph-rest-beta) e [entidades de serviço](/graph/api/serviceprincipal-list-transitivemembersof?view=graph-rest-beta).|
| Adição | beta | Adicionado método memberOf para obter uma direta [associação](/graph/api/device-list-members?view=graph-rest-beta) de dispositivos. Esse método foi adicionado para obter a lista de associações, incluindo associações aninhadas.|
| Adição | beta | Adicionadas novas propriedades para [usuários](/graph/api/resources/user?view=graph-rest-beta): **fax**, **onPremisesDistinguishedName**, e **otherMails**.|
| Adição | beta | Adicionada a propriedade **forceChangePasswordNextSignInWithMfa** para o tipo complexo [passwordProfile](/graph/api/resources/passwordprofile?view=graph-rest-beta).|
| Adição    | beta | Adicionadas as propriedades 'externalUserState' e "externalUserStateChangeDateTime" para o objeto [usuário](/graph/api/resources/user?view=graph-rest-beta).|

### <a name="microsoft-teams-apis"></a>APIs do Microsoft Teams

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Adição |v1.0| Introduzido um novo tipo de recurso [equipe](/graph/api/resources/team?view=graph-rest-1.0).|
|Adição |v1.0| Introduzido um novo tipo de recurso [canal](/graph/api/resources/channel?view=graph-rest-1.0).|
|Adição |v1.0| Introduzido um novo tipo de recurso [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-1.0).|
|Adição |v1.0| Introduzido um novo tipo de recurso [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-1.0).|
|Adição |v1.0| Introduzido um novo tipo de recurso [teamsAppInstallation](/graph/api/resources/teamsappinstallation?view=graph-rest-1.0).|
|Adição |v1.0| Introduzido um novo tipo de recurso [teamsAsyncOperation](/graph/api/resources/teamsasyncoperation?view=graph-rest-1.0). |
|Adição |v1.0| Introduzido um novo tipo complexo [teamGuestSettings](/graph/api/resources/teamguestsettings?view=graph-rest-1.0). |
|Adição |v1.0| Introduzido um novo tipo complexo [teamMemberSettings](/graph/api/resources/teammembersettings?view=graph-rest-1.0). |
|Adição |v1.0| Introduzido um novo tipo complexo [teamMessagingSettings](/graph/api/resources/teammessagingsettings?view=graph-rest-1.0). |
|Adição |v1.0| Introduzido um novo tipo complexo [teamFunSettings](/graph/api/resources/teamfunsettings?view=graph-rest-1.0). |
|Adição |v1.0| Introduzido uma nova ação [Clonar equipe](/graph/api/team-clone?view=graph-rest-1.0). |
|Adição |v1.0| Introduzido nova ação [Equipe de arquivo](/graph/api/team-archive?view=graph-rest-1.0).|
|Adição |v1.0| Introduzido uma nova ação [equipe Unarchive](/graph/api/team-unarchive?view=graph-rest-1.0). |
|Adição         | Beta          | Adicionado o suporte a permissões de aplicativos para [clonar equipe](/graph/api/team-clone?view=graph-rest-beta). |
|Adição |beta| Introduzido [/teams/ {id} / installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta), que substituirá /teams/ {id} / aplicativos com algumas diferenças na carga. |
|Adição |beta| Introduzido [{/appCatalogs/teamsApps/id de} / appDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta), que substituirá a propriedade de versão [{/appCatalogs/teamsApps/id de}](/graph/api/resources/teamsapp?view=graph-rest-beta). |
|Alteração   |beta| Renomeado o tipo de [/appCatalogs/teamsApps](/graph/api/resources/teamsapp?view=graph-rest-beta) do teamsCatalogApp para teamsApp. |
|Alteração   |beta| Renomeado o tipo de propriedade distributionMethod no [/appCatalogs/teamsApps](/graph/api/resources/teamsapp?view=graph-rest-beta) de teamsCatalogAppDistributionMethod para teamsAppDistributionMethod  |
|Remoção |beta| teamsCatalogAppDistributionMethod foi renomeado como teamsAppDistributionMethod  |
|Adição |beta| Introduzido [/teams/ {id} / installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta), que substituirá /teams/ {id} / aplicativos com algumas diferenças na carga. |
|Adição |beta| Adicionou a propriedade displayName a [teamsTab](/graph/api/resources/teamstab?view=graph-rest-beta). |
|Adição |beta| Adicionada a propriedade de messageId [teamsTab](/graph/api/resources/teamstab?view=graph-rest-beta) |
|Adição |beta| Adicionada a propriedade teamsApp [teamsTab](/graph/api/resources/teamstab?view=graph-rest-beta) |
|Adição |beta| Introduzido um novo tipo de recurso [teamsAppInstallation](/graph/api/resources/teamsappinstallation?view=graph-rest-beta).|
|Adição |beta| Introduzido um novo tipo de recurso [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-beta).|
|Adição |beta| Introduzido um novo tipo de recurso [teamsAppDefinition](/graph/api/resources/teamsappdefinition?view=graph-rest-beta).|
|Adição |beta| Apresentamos a nova enumeração do membro hiddenMembership para teamVisibilityType.|
|Adição |beta| Apresentamos a nova enumeração membro createTeam para teamsAsyncOperationType.|
|Adição |beta| Introduzida a nova enumeração do membro teamsAppDistributionMethod.|
|Adição |beta| Introduzida nova ação de atualização do aplicativo em [/teams/ {id} / installedApps](/graph/api/resources/teamsappinstallation?view=graph-rest-beta). |

### <a name="reports-apis"></a>APIs de relatórios

| Tipo de alteração | Versão                                    | Descrição                              |
| :---------- | :----------------------------------------- | :--------------------------------------- |
| Adição    | Versão Beta do Microsoft Graph China operado pela 21Vianet | As seguintes APIs foram adicionadas:<br>[getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta)<br>[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta)<br>[getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta)<br>[getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-beta)<br>[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-beta)<br>[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-beta)<br>[getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-beta)<br>[getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta)<br>[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-beta)<br>[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-beta)<br>[getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-beta)<br>[getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-beta)<br>[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-beta)<br>[getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-beta)<br>[getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-beta)<br>[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-beta)<br>[getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-beta)<br> [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-beta)<br>[getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-beta)<br>[getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-beta)<br>[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-beta)<br>[getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-beta)<br>[getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-beta)<br>[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-beta)<br>[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-beta)<br>[getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-beta)<br>[getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-beta)<br>[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-beta)<br>[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-beta)<br>[getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-beta)<br>[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta)<br>[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-beta)<br>[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-beta)<br>[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-beta)<br>[getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-beta)<br>[getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-beta)<br>[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-beta). |

## <a name="october-2018"></a>Outubro de 2018

### <a name="directory-apis"></a>APIs de diretório

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição | beta | Adicionado novo método transitiveMembers em [grupos](/graph/api/group-list-transitivemembers?view=graph-rest-beta). Esse método retorna uma lista simples de membros, inclusive os aninhados.|
| Adição | beta | Adicionado novo método transitiveMemberOf em [usuários](/graph/api/user-list-transitivemembersof?view=graph-rest-beta), [grupos](/graph/api/group-list-transitivemembersof?view=graph-rest-beta), [dispositivos](/graph/api/device-list-transitivemembersof?view=graph-rest-beta) e [entidades de serviço](/graph/api/serviceprincipal-list-transitivemembersof?view=graph-rest-beta).|
| Adição | beta | Adicionado método memberOf para obter uma direta [associação](/graph/api/device-list-members?view=graph-rest-beta) de dispositivos. Esse método foi adicionado para obter a lista de associações, incluindo associações aninhadas.|
| Adição | beta | Adicionadas novas propriedades para [usuários](/graph/api/resources/user?view=graph-rest-beta): **fax**, **onPremisesDistinguishedName**, e **otherMails**.|

### <a name="riskyusers-apis"></a>APIs RiskyUsers

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Adição |beta| Introduzida a [API riskyUsers](/graph/api/resources/riskyuser?view=graph-rest-beta), que representa os usuários do Azure Active Directory que estão em risco, conforme detectado pelo Azure AD Identity Protection. |


### <a name="signin-apis"></a>APIs de entrada

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Alteração   |beta| Renomeada a propriedade `conditionalAccessPolicies` para `appliedConditionalAccessPolicy`.|
|Adição |beta| Introduzidas propriedades adicionais de risco na [API signIn](/graph/api/resources/signin?view=graph-rest-beta), incluindo `riskDetail`, `riskLevelAggregated`, `riskLevelDuringSignIn`, `riskEventTypes`, e `riskState`.|
|Adição |beta| Introduzidas propriedades adicionais de login em [signIn API](/graph/api/resources/signin?view=graph-rest-beta), incluindo `authenticationProcessingDetails`, `originalRequestID`, `isInteractive`, `tokenIssuerName`, `tokenIssuerType`, `correlationId`, e `processingTimeinMilliseconds`.|
|Remoção   |beta| Remover a propriedade `isRisky`.|

## <a name="october-2018"></a>Outubro de 2018

### <a name="delta-query"></a>Consulta delta

| **Tipo de alteração** | **Versão** | **Descrição**                  |
|:------------|:--------|:-----------------------------------------|
| Adição    | Beta   | Adicionadoo recurso de [consulta delta](delta-query-overview.md) para [directoryObject](/graph/api/directoryobject-delta?view=graph-rest-beta) |
| Alteração      | v1.0 e beta  | Comportamento alternativo para retornar propriedades alteradas apenas na resposta JSON para [usuários](/graph/api/user-delta?view=graph-rest-1.0) e [grupos](/graph/api/group-delta?view=graph-rest-1.0). |
| Adição    | v1.0   | Adicionada a função [delta](/graph/api/directoryrole-delta?view=graph-rest-1.0) para [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-1.0) para dar suporte ao [controle de alterações do uso da consulta delta](delta-query-overview.md). |

### <a name="directory-apis"></a>APIs de diretório

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição | Beta | Adicionada a propriedade **licenseAssignmentStates** para a entidade de[usuário](/graph/api/resources/user?view=graph-rest-beta) para [Licenciamento Baseado em Grupo](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).|
| Adição | Beta | Adicionado o recurso **licenseAssignmentState** para [Licenciamento Baseado em Grupo](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).|
| Adição | Beta | Adicionadas as propriedades **assignedLicenses**, **licenseProcessingState**, **hasMembersWithLicenseErrors** e **membersWithLicenseErrors** para a entidade[Grupo ](/graph/api/resources/group?view=graph-rest-beta) para [Licenciamento Baseado em Grupo](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-licensing-whatis-azure-portal).|

### <a name="microsoft-intune-apis"></a>APIs do Microsoft Intune

|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|v1.0|Adicionada a propriedade**tenantLockdownRequireNetworkDuringOutOfBoxExperience** para a entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-1.0)|
|Adição|v1.0|A propriedade **v12_0** foi adicionada ao tipo complexo [iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-1.0)|
|Adição|beta|Adicionada a propriedade **lastReportAggregationDateTime** para a entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)|
|Adição|beta|Foram adicionadas novas entidades:<br/>[intuneBrandingProfile](/graph/api/resources/intune-wip-intunebrandingprofile?view=graph-rest-beta)<br/>|
|Adição|beta|Foram adicionados novos tipos complexos:<br/>[deviceAndAppManagementAssignedRoleIds](/graph/api/resources/intune-rbac-deviceandappmanagementassignedroleids?view=graph-rest-beta)<br/>|
|Adição|Beta|Foram adicionados novos tipos de enumeração:<br/>[applicationGuardEnabledOptions](/graph/api/resources/intune-deviceconfig-applicationguardenabledoptions?view=graph-rest-beta)<br/>[autoRestartNotificationDismissalMethod](/graph/api/resources/intune-deviceconfig-autorestartnotificationdismissalmethod?view=graph-rest-beta)<br/>[meteredConnectionLimitType](/graph/api/resources/intune-deviceconfig-meteredconnectionlimittype?view=graph-rest-beta)<br/>|
|Adição|beta|Adicionada a ação[enableLegacyPcManagement](/graph/api/intune-deviceconfig-devicemanagement-enablelegacypcmanagement?view=graph-rest-beta)em [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) |
|Adição|beta|Adicionada a ação[extendFeatureUpdatesPause](/graph/api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendfeatureupdatespause?view=graph-rest-beta) em [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) |
|Adição|beta|Adicionada a ação [extendQualityUpdatesPause](/graph/api/intune-deviceconfig-windowsupdateforbusinessconfiguration-extendqualityupdatespause?view=graph-rest-beta) em [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) |
|Adição|beta|Adicionada a ação [unassignUserFromDevice](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-unassignuserfromdevice?view=graph-rest-beta) em [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) |
|Adição|beta|Adicionada a função [getAssignedRoleIdsForLoggedInUser](/graph/api/intune-rbac-devicemanagement-getassignedroleidsforloggedinuser?view=graph-rest-beta) em [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) |
|Adição|beta|Adicionada a função [getManagedDevicesWithAppFailures](/graph/api/intune-troubleshooting-user-getmanageddeviceswithappfailures?view=graph-rest-beta) em [usuário](/graph/api/resources/intune-devices-user?view=graph-rest-beta) |
|Adição|beta|Adicionada a função [managedDeviceEnrollmentAbandonmentSummary](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentabandonmentsummary?view=graph-rest-beta) em [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) |
|Adição|beta|A função [managedDeviceEnrollmentAbandonmentDetails](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentabandonmentdetails?view=graph-rest-beta) foi adicionada ao [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) |
|Exclusão|beta|Remover a propriedade **subjectAlternativeNameType** propriedade na entidade [androidForWorkCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkcertificateprofilebase?view=graph-rest-beta)|
|Adição|beta|A propriedade **subjectAlternativeNameType** foi adicionada à entidade [androidForWorkPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta)|
|Adição|beta|Adicionado o **certificateStore**, **customSubjectAlternativeNames** e propriedades**subjectAlternativeNameType**para a entidade[ androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta)|
|Exclusão|beta|Remover a propriedade **subjectAlternativeNameType** na entidade[androidWorkProfileCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofilecertificateprofilebase?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **subjectAlternativeNameType** para a entidade [androidWorkProfilePkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile?view=graph-rest-beta)|
|Adição|beta|Adicionado o **certificateStore**, **customSubjectAlternativeNames** e propriedades**subjectAlternativeNameType**para a entidade[androidWorkProfileScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilescepcertificateprofile?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **legacyPcManangementEnabled** para a entidade [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Exclusão|beta|Remover a propriedade **pinRequiredOnLaunchInsteadOfBiometric** na entidade [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta)|
|Adição|beta|A propriedade de navegação **roleScopeTagIds** foi adicionada à entidade [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **applicationGuardEnabledOptions** para a entidade [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **selectedMobileAppIds** para a entidade [windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta) |
|Adição|beta|Adicionadas as propriedades **engagedRestartDeadlineInDays**, **engagedRestartSnoozeScheduleInDays**, **engagedRestartTransitionScheduleInDays**, ** autoRestartNotificationDismissal**, **scheduleRestartWarningInHours** e **scheduleImminentRestartWarningInMinutes** à entidade[ windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) |
|Adição|beta|Adicionadas as propriedades**preSharedKey** e **meteredConnectionLimit** para a entidade [windowsWifiConfiguration](/graph/api/resources/intune-deviceconfig-windowswificonfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade de navegação**intuneBrandingProfiles** para a entidade[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades**v6_0**, **v7_0**, **v7_1**, **v8_0**, **v8_1** e **v9_0**para o tipo complexo [androidMinimumOperatingSystem](/graph/api/resources/intune-apps-androidminimumoperatingsystem?view=graph-rest-beta)|
|Adição|beta|A propriedade **v12_0** foi adicionada ao tipo complexo [iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-beta)|
|Exclusão|beta|Remover a propriedade**runAsLoggedOnUser** no tipo complexo[win32LobAppPowerShellScriptDetection](/graph/api/resources/intune-apps-win32lobapppowershellscriptdetection?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **lastUpdateDateTime** para o tipo complexo[osVersionCount](/graph/api/resources/intune-devices-osversioncount?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **lastUpdateDateTime** para o tipo complexo[windowsMalwareCategoryCount](/graph/api/resources/intune-devices-windowsmalwarecategorycount?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade**lastUpdateDateTime** para o tipo complexo [windowsMalwareExecutionStateCount](/graph/api/resources/intune-devices-windowsmalwareexecutionstatecount?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **lastUpdateDateTime** para o tipo complexo[windowsMalwareNameCount](/graph/api/resources/intune-devices-windowsmalwarenamecount?view=graph-rest-beta) |
|Adição|beta|Adicionada a propriedade **lastUpdateDateTime** para o tipo complexo [windowsMalwareStateCount](/graph/api/resources/intune-devices-windowsmalwarestatecount?view=graph-rest-beta) |

### <a name="microsoft-teams-apis"></a>APIs do Microsoft Teams

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Adição|beta|Adicionado o suporte a permissões de aplicativos para APIs.[arquivar equipe](/graph/api/team-archive?view=graph-rest-beta) e [unarchive equipe](/graph/api/team-unarchive?view=graph-rest-beta).|

### <a name="outlook-contacts"></a>Contatos do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Remoção         | v1.0        | Isso é uma correção para a documentação: removida a propriedade**sinalizador** no tópico entidade [entre em contato com](/graph/api/resources/contact?view=graph-rest-1.0). A propriedade nunca foi disponibilizada na entidade **entre em contato com**.|

### <a name="privileged-identity-management-apis"></a>APIs de Privileged Identity Management

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Alteração | beta | Alterar a entidade [privilegedapproval](/graph/api/resources/privilegedapproval?view=graph-rest-beta).|
| Adição | beta | A entidade [privilegedroleassignmentrequest](/graph/api/resources/privilegedroleassignmentrequest?view=graph-rest-beta) e os seguintes métodos e ações foram adicionados:<br> [List](/graph/api/privilegedroleassignmentrequest-list?view=graph-rest-beta) <br> [Create](/graph/api/privilegedroleassignmentrequest-post?view=graph-rest-beta) <br> [Cancel](/graph/api/privilegedroleassignmentrequest-cancel?view=graph-rest-beta) <br> [Pessoal](/graph/api/privilegedroleassignmentrequest-my?view=graph-rest-beta) |
| Adição | beta | Adicionada a [atualização](/graph/api/privilegedrolesettings-update?view=graph-rest-beta) para [privilegedRoleSettings](/graph/api/resources/privilegedrolesettings?view=graph-rest-beta)|
| Remoção |beta| Foi substituído a [Auto Ativação da Atribuição de Função](/graph/api/privilegedrole_selfactivate?view=graph-rest-beta)|

### <a name="reports-apis"></a>APIs de relatórios
| Tipo de alteração | Versão | Descrição                              |
|:------------|:--------|:-----------------------------------------|
| Adição    | v1.0    | Adicionada a propriedade **ID do Site** para[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0). |

## <a name="september-2018"></a>Setembro de 2018

### <a name="calls-and-online-meetings-api"></a>Chamadas e reuniões online API

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | O recurso [aplicativo](/graph/api/resources/application?view=graph-rest-beta) foi atualizado para adicionar um conjunto de chamadas. |
| Alteração          | Beta        | O recurso[operação](/graph/api/resources/operation?view=graph-rest-beta) foi atualizado para oferecer suporte para chamadas de longa duração e APIs de reuniões. |
| Adição        | Beta        | Adicionado o recurso de [chamada](/graph/api/resources/call?view=graph-rest-beta) para gerenciar chamadas de áudio / vídeo (inicialmente, no Microsoft Teams), incluindo APIs para [criar chamadas](/graph/api/application-post-calls?view=graph-rest-beta), [recuperar uma chamada](/graph/api/call-get?view=graph-rest-beta), [excluir (desligar) uma chamada](/graph/api/call-delete?view=graph-rest-beta), [atender uma chamada](/graph/api/call-answer?view=graph-rest-beta), [rejeitar uma chamada](/graph/api/call-reject?view=graph-rest-beta), [redirecionar uma chamada](/graph/api/call-redirect?view=graph-rest-beta) e [transferir uma chamada](/graph/api/call-transfer?view=graph-rest-beta). Também adicionamos APIs para dar suporte aos [cenários IVR](/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta): [reproduzir um aviso](/graph/api/call-playprompt?view=graph-rest-beta), [gravar uma chamada](/graph/api/call-record?view=graph-rest-beta), [Cancelar processamento de mídia](/graph/api/call-cancelmediaprocessing?view=graph-rest-beta)e [assinar notificações de tom de toque.](/graph/api/call-subscribetotone?view=graph-rest-beta). |
| Adição        | Beta        | Adicionado o recurso [participante](/graph/api/resources/call?view=graph-rest-beta) e as APIs de gerenciamento de participantes em chamadas de áudio/vídeo e reuniões, incluindo [recuperar um objeto participante](/graph/api/participant-get?view=graph-rest-beta), [configurar áudio mixer para um participante](/graph/api/participant-configuremixer?view=graph-rest-beta), tirar o som de [um](/graph/api/participant-mute?view=graph-rest-beta) ou [todos](/graph/api/participant-muteall?view=graph-rest-beta) os participantes [recuperar uma lista de participantes](/graph/api/call-list-participants?view=graph-rest-beta) em uma reunião/chamada e [convidar participantes](/graph/api/participant-invite?view=graph-rest-beta) para reunião/chamada. |
| Adição        | Beta        | APIs adicionadas para aplicativos para gerenciar e participar de chamadas e reuniões, incluindo a possibilidade de [compartilhar conteúdo](/graph/api/call-changescreensharingrole?view=graph-rest-beta), [ativar e desativar o áudio](/graph/api/call-unmute?view=graph-rest-beta), e [atualizar metadados associadas uma chamada](/graph/api/call-updatemetadata?view=graph-rest-beta). |
| Adição        | Beta        | Adicionado o [recurso de grupo de roteamento de áudio](/graph/api/resources/audioroutinggroup?view=graph-rest-beta) e APIs para gerenciar rotas de áudio privadas entre participantes em uma conversa com vários participantes, incluindo a [criação de grupos de roteamento de áudio](/graph/api/call-post-audioroutinggroups?view=graph-rest-beta), [a recuperação de uma lista deles](/graph/api/audioroutinggroup-get?view=graph-rest-beta) e a [atualização](/graph/api/audioroutinggroup-update?view=graph-rest-beta) e a [exclusão](/graph/api/audioroutinggroup-delete?view=graph-rest-beta) deles. |
| Adição        | Beta        | Adicionando o recurso [reunião online](/graph/api/resources/audioroutinggroup?view=graph-rest-beta) e as APIs de gerenciamento de reuniões online do Microsoft Teams. Inicialmente, há apenas uma API para reuniões online, ao [recuperar um objeto de reunião online](/graph/api/onlinemeeting-get?view=graph-rest-beta). Um recurso relacionado para as[informações de audioconferência](/graph/api/resources/audioconferencing?view=graph-rest-beta) associadas a uma reunião (por exemplo, URL discada, senhas e números de telefone) também foi adicionado. |
| Adição        | Beta        | Muitas das APIs de chamadas e reuniões demoram para serem concluídas, de modo que foram adicionados recursos para essas operações de longa duração: [operações específicas de chamada](/graph/api/resources/commsoperation?view=graph-rest-beta), [reproduzir instruções de áudio](/graph/api/resources/playpromptoperation?view=graph-rest-beta), e [ gravação](/graph/api/resources/recordoperation?view=graph-rest-beta).  |

### <a name="dynamics-365-business-central-api"></a>API Central do Dynamics 365 Business

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | Beta          | Adicionadas APIs financeiras para o Dynamics 365 Business Central. Para saber mais, confira o [referência da API de finanças](/graph/api/resources/dynamics-graph-reference?view=graph-rest-beta)

### <a name="microsoft-graph-data-connect"></a>Conexão de dados do Microsoft Graph

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Adição         | Não aplicável| Introduziu a capacidade de acessar dados do Office 365 em massa. Para saber mais, confira [conexão de dados do Microsoft Graph (visualização)](data-connect-overview.md).|

### <a name="microsoft-intune-apis"></a>APIs do Microsoft Intune
|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|v1.0|A ação [assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-1.0) foi adicionada a [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-1.0) |
|Adição|beta|Foram adicionadas novas entidades:<br/>[officeClientConfiguration](/graph/api/resources/intune-cirrus-officeclientconfiguration?view=graph-rest-beta)<br/>[officeClientConfigurationAssignment](/graph/api/resources/intune-cirrus-officeclientconfigurationassignment?view=graph-rest-beta)<br/>[officeConfiguration](/graph/api/resources/intune-cirrus-officeconfiguration?view=graph-rest-beta)<br/>[windowsOfficeClientConfiguration](/graph/api/resources/intune-cirrus-windowsofficeclientconfiguration?view=graph-rest-beta)<br/>[windowsOfficeClientSecurityConfiguration](/graph/api/resources/intune-cirrus-windowsofficeclientsecurityconfiguration?view=graph-rest-beta)<br/>|
|Adição|beta|Foram adicionados novos tipos complexos:<br/>[officeClientCheckinStatus](/graph/api/resources/intune-cirrus-officeclientcheckinstatus?view=graph-rest-beta)<br/>[officeConfigurationAssignmentTarget](/graph/api/resources/intune-cirrus-officeconfigurationassignmenttarget?view=graph-rest-beta)<br/>[officeConfigurationGroupAssignmentTarget](/graph/api/resources/intune-cirrus-officeconfigurationgroupassignmenttarget?view=graph-rest-beta)<br/>[officeUserCheckinSummary](/graph/api/resources/intune-cirrus-officeusercheckinsummary?view=graph-rest-beta)<br/>|
|Adição|beta|Adicionar a ação [atribua](/graph/api/intune-cirrus-officeclientconfiguration-assign?view=graph-rest-beta) em [officeClientConfiguration](/graph/api/resources/intune-cirrus-officeclientconfiguration?view=graph-rest-beta) |
|Adição|beta|Adicionar a ação **updatePrioritie** no conjunto[officeClientConfiguration](/graph/api/resources/intune-cirrus-officeclientconfiguration?view=graph-rest-beta)  |
|Adição|beta|Foram adicionadas novas entidades:<br/>[deviceConfigurationConflictSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationconflictsummary?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta)<br/>[win32LobApp](/graph/api/resources/intune-apps-win32lobapp?view=graph-rest-beta)<br/>|
|Adição|beta|Foram adicionados novos tipos complexos:<br/>[deviceConfigurationTargetedUserAndDevice](/graph/api/resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice?view=graph-rest-beta)<br/>[win32LobAppDetection](/graph/api/resources/intune-apps-win32lobappdetection?view=graph-rest-beta)<br/>[win32LobAppFileSystemDetection](/graph/api/resources/intune-apps-win32lobappfilesystemdetection?view=graph-rest-beta)<br/>[win32LobAppInstallExperience](/graph/api/resources/intune-apps-win32lobappinstallexperience?view=graph-rest-beta)<br/>[win32LobAppMsiInformation](/graph/api/resources/intune-apps-win32lobappmsiinformation?view=graph-rest-beta)<br/>[win32LobAppPowerShellScriptDetection](/graph/api/resources/intune-apps-win32lobapppowershellscriptdetection?view=graph-rest-beta)<br/>[win32LobAppProductCodeDetection](/graph/api/resources/intune-apps-win32lobappproductcodedetection?view=graph-rest-beta)<br/>[win32LobAppRegistryDetection](/graph/api/resources/intune-apps-win32lobappregistrydetection?view=graph-rest-beta)<br/>[win32LobAppReturnCode](/graph/api/resources/intune-apps-win32lobappreturncode?view=graph-rest-beta)<br/>[windows10AppsForceUpdateSchedule](/graph/api/resources/intune-deviceconfig-windows10appsforceupdateschedule?view=graph-rest-beta)<br/>|
|Adição|Beta|Foram adicionados novos tipos de enumeração:<br/>[administratorConfiguredDeviceComplianceState](/graph/api/resources/intune-deviceconfig-administratorconfigureddevicecompliancestate?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUploadStatus](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus?view=graph-rest-beta)<br/>[microsoftStoreForBusinessPortalSelectionOptions](/graph/api/resources/intune-onboarding-microsoftstoreforbusinessportalselectionoptions?view=graph-rest-beta)<br/>[win32LobAppDetectionOperator](/graph/api/resources/intune-apps-win32lobappdetectionoperator?view=graph-rest-beta)<br/>[win32LobAppFileSystemDetectionType](/graph/api/resources/intune-apps-win32lobappfilesystemdetectiontype?view=graph-rest-beta)<br/>[win32LobAppMsiPackageType](/graph/api/resources/intune-apps-win32lobappmsipackagetype?view=graph-rest-beta)<br/>[win32LobAppRegistryDetectionType](/graph/api/resources/intune-apps-win32lobappregistrydetectiontype?view=graph-rest-beta)<br/>[win32LobAppReturnCodeType](/graph/api/resources/intune-apps-win32lobappreturncodetype?view=graph-rest-beta)<br/>[windows10AppsUpdateRecurrence](/graph/api/resources/intune-deviceconfig-windows10appsupdaterecurrence?view=graph-rest-beta)<br/>[windowsAppStartLayoutTileSize](/graph/api/resources/intune-deviceconfig-windowsappstartlayouttilesize?view=graph-rest-beta)<br/>[windowsAutopilotProfileAssignmentDetailedStatus](/graph/api/resources/intune-enrollment-windowsautopilotprofileassignmentdetailedstatus?view=graph-rest-beta)<br/>|
|Adição|beta|Adicionada a ação **overrideComplianceState** em [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|Adição|beta|Adicionada a ação **getTargetedUsersAndDevices** no conjunto [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) |
|Adição|beta|Adicionada a função [autopilotDeviceStream](/graph/api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-autopilotdevicestream?view=graph-rest-beta) em [importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta) |
|Adição|beta|Adicionada a propriedade **restrictedApps** à entidade [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) |
|Adição|beta|Adicionada a propriedade**tokenCreationDateTime** para a entidade [androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta)|
|Exclusão|beta|Removida a propriedade **restrictedApps** na entidade[androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta)|
|Exclusão|beta|Removida a propriedade **restrictedApps** na entidade[androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta)|
|Alteração|beta|Foram alteradas as seguintes propriedades na entidade [appleVpnConfiguration](/graph/api/resources/intune-deviceconfig-applevpnconfiguration?view=graph-rest-beta):<br/>**enablePerApp** de obrigatório para opcional<br/>|
|Adição|beta|As propriedades**disableProtectionOfManagedOutboundOpenInData** e **protectInboundDataFromUnknownSources** foram adicionadas à entidade[defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) |
|Adição|beta|A propriedade **microsoftStoreForBusinessPortalSelection** foi adicionada à entidade [deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-beta) |
|Adição|beta|A propriedade**passcodeMinutesOfInactivityBeforeScreenTimeout** foi adicionada à entidade [iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-beta)|
|Adição|beta|Foi adicionada a propriedade **useOAuth** à entidade[iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta)|
|Adição|beta|Foram adicionadas às propriedades **kioskModeBlockVolumeButtons**, **classroomForceRequestPermissionToLeaveClasses**, **keychainBlockCloudSync**, ** pkiBlockOTAUpdates**, **privacyForceLimitAdTracking**, **enterpriseBookBlockBackup**, **enterpriseBookBlockMetadataSync**, **airPrintBlocked**, **airPrintBlockCredentialsStorage**, **airPrintForceTrustedTLS**, **airPrintBlockiBeaconDiscovery**, **blockSystemAppRemoval** e **vpnBlockCreation** à entidade[iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta)|
|Adição|beta|As propriedades**disableProtectionOfManagedOutboundOpenInData** e **protectInboundDataFromUnknownSources** foram adicionadas à entidade[iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) |
|Adição|beta|Foi adicionada a propriedade **gatekeeperAllowedAppSource** à entidade[macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta)|
|Adição|beta|Foram adicionadas as propriedades**keychainBlockCloudSync**, **airPrintBlocked**, **airPrintForceTrustedTLS** e **airPrintBlockiBeaconDiscovery** para a entidade[macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta) |
|Adição|beta|Foram adicionadas as propriedades**deviceModel** e **deviceManufacturer** à entidade[managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **enabledForScopeValidation** para a entidade [resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **claimTokenManagementFromExternalMdm** propriedade para a entidade [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) |
|Adição|beta|Adicionada a propriedade **windows10AppsForceUpdateSchedule** para a entidade[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **deploymentProfileAssignmentDetailedStatus** para a entidade [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades**deviceConfigurationConflictSummary** e **importedWindowsAutopilotDeviceIdentityUploads** propriedades de navegação para a entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) |
|Adição|beta|Adicionar a propriedade de navegação **intendedDeploymentProfile** para a entidade [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)|
|Adição|beta|Adicionar as propriedades**startLayoutTileSize** e **nome** para o tipo complexo[windowsKioskAppBase](/graph/api/resources/intune-deviceconfig-windowskioskappbase?view=graph-rest-beta) |
|Adição|beta|Adicionadas as propriedades**desktopApplicationId** e **desktopApplicationLinkPath** para o tipo complexo[windowsKioskDesktopApp](/graph/api/resources/intune-deviceconfig-windowskioskdesktopapp?view=graph-rest-beta)|
|Exclusão|beta|Removida a propriedade o **nome** no tipo complexo[windowsKioskDesktopApp](/graph/api/resources/intune-deviceconfig-windowskioskdesktopapp?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **disallowDesktopApps** para o tipo complexo[windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta)|
|Alteração|beta|Foram alteradas as seguintes propriedades do tipo complexo[windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta):<br/>**startMenuLayoutXml** de obrigatória para opcional<br/>|
|Adição|beta|Adicionadas as propriedades **v10_1607**, **v10_1703**, **v10_1709** e **v10_1803** do tipo complexo [ windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-beta)|
|Adição|beta|Foi adicionado o membro **paloAltoGlobalProtect** ao tipo de enumeração [androidWorkProfileVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconnectiontype?view=graph-rest-beta)|
|Adição|beta|Adicionar o membro**remoteLock** para os tipos de enumeração [deviceComplianceActionType](/graph/api/resources/intune-deviceconfig-devicecomplianceactiontype?view=graph-rest-beta)|


### <a name="microsoft-teams-apis"></a>APIs do Microsoft Teams

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Adição|beta|Adicionar API para [guias](/graph/api/resources/teamstab?view=graph-rest-beta).|
|Adição|beta|Adicionar API para [publicação de aplicativos para sua organização](/graph/api/resources/teamsapp?view=graph-rest-beta).|
|Adição|beta|Adicionado o suporte a permissões de aplicativos para  [GET/teams/{id}](/graph/api/team-get?view=graph-rest-beta). |
|Adição|beta|Adicionado o suporte a permissões de aplicativos para  [GET/teams/{id} /canais](/graph/api/group-list-channels?view=graph-rest-beta). |
|Adição|beta|Adicionado o suporte a permissões do aplicativo para [GET /teams/ {id} /channels/ {id}](/graph/api/channel-get?view=graph-rest-beta). |
|Adição|beta|Adicionado o suporte a permissões de aplicativos para [PUT / groups / {id} / team](/graph/api/team-put-teams?view=graph-rest-beta). |
|Adição|beta|Adicionado o suporte a permissões de aplicativo para[PATCH /teams/ {id}](/graph/api/team-update?view=graph-rest-beta). |
|Adição|beta|Adicionado o suporte a permissões de aplicativos para [Criar canal](/graph/api/channel-post?view=graph-rest-beta), [Canal de atualização](/graph/api/channel-patch?view=graph-rest-beta), e [Excluir canal](/graph/api/channel-delete?view=graph-rest-beta). |
|Exclusão|beta| Removidas as propriedades isBlocks e installedState do [teamsApp](/graph/api/resources/teamsapp?view=graph-rest-beta).|
|Alteração| beta | A propriedade de contexto em[teamsApp](/graph/api/resources/teamsapp?view=graph-rest-beta) foi renomeada como distributionMethod.|

### <a name="onedrive-and-sharepoint-apis"></a>APIs do OneDrive e SharePoint

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Adicionado o argumento **deferCommit** para a ação[createUploadSession](/graph/api/driveitem-createuploadsession?view=graph-rest-beta) em [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta)|
| Adição        | Beta        | Adicionado[storagePlanInformation](/graph/api/resources/storageplaninformation?view=graph-rest-beta) tipo complexo |
| Adição        | Beta        | Adicionada a propriedade**storagePlanInformation** para a  [cota](/graph/api/resources/quota?view=graph-rest-beta) tipo complexo |
| Adição        | Beta        | Adicionada a propriedade de navegação**seguintes** para a entidade [unidade](/graph/api/resources/drive?view=graph-rest-beta) |
| Adição        | Beta        | Adicionada a ação [siga](/graph/api/driveitem-follow?view=graph-rest-beta) no [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) |
| Adição        | Beta        | Adicionar a API [parar de seguir](/graph/api/driveitem-unfollow?view=graph-rest-beta) |
| Adição        | Beta        | Adicionada a propriedade **hasPassword** para a entidade [permissão](/graph/api/resources/permission?view=graph-rest-beta)  |
| Adição        | Beta        | Foi adicionada a propriedade **preventsDownload** para o tipo complexo[sharingLink](/graph/api/resources/sharinglink?view=graph-rest-beta)  |
| Adição        | Beta        | Adicionada a propriedade de navegação **permissão** para a entidade[sharedDriveItem](/graph/api/resources/shareddriveitem?view=graph-rest-beta) |
| Adição        | Beta        | Adicionada a propriedade **localização geográfica** para a entidade [columnDefinition](/graph/api/resources/columndefinition?view=graph-rest-beta) |
| Adição        | Beta        | Adicionado o [geolocationColumn](/graph/api/resources/geolocationcolumn?view=graph-rest-beta) tipo complexo |
| Adição        | Beta        | Adicionada a propriedade**analytics** para a entidade [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) |
| Adição        | Beta        | Adicionada a propriedade **analytics** para a entidade [site](/graph/api/resources/site?view=graph-rest-beta) |
| Adição        | Beta        | Adicionada a propriedade**analytics** para a entidade [listItem](/graph/api/resources/listitem?view=graph-rest-beta) |
| Adição        | Beta        | Adicionada a função**getActivitiesByInterval** na entidade[driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) |
| Adição        | Beta        | Adicionada a função**getActivitiesByInterval** na entidade[site](/graph/api/resources/site?view=graph-rest-beta) |
| Adição        | Beta        | Adicionada a função**getActivitiesByInterval** na entidade[listItem](/graph/api/resources/listitem?view=graph-rest-beta) |
| Adição        | Beta        | Adicionada a entidade [itemAnalytics](/graph/api/resources/itemanalytics?view=graph-rest-beta)  |
| Adição        | Beta        | Adicionada a entidade[itemActivityStat](/graph/api/resources/itemactivity?view=graph-rest-beta)  |
| Adição        | Beta        | Adicionado o tipo complexo [itemActionStat](/graph/api/resources/itemactionstat?view=graph-rest-beta) |
| Adição        | Beta        | Adicionar o tipo complexo[accessAction](/graph/api/resources/accessaction?view=graph-rest-beta) |
| Adição        | Beta        | Adicionado o tipo complexo [incompleteData](/graph/api/resources/incompletedata?view=graph-rest-beta)  |
| Adição        | Beta        | Adicionada a propriedade **acesso** para o tipo complexo[itemActivity](/graph/api/resources/itemactivity?view=graph-rest-beta) |
| Adição        | Beta        | Adicionada a propriedade **local** para o tipo complexo[itemActivity](/graph/api/resources/itemactivity?view=graph-rest-beta) |
| Adição        | v1.0        | Foi adicionada a ação **preview** na entidade [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) |
| Adição        | v1.0        | Adicionado o tipo complexo [itemPreviewInfo](/graph/api/resources/itempreviewinfo?view=graph-rest-1.0) |

### <a name="outlook-mail"></a>Email do Outlook

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0 e beta | A propriedade**internetMessageHeaders** da entidade [mensagem](/graph/api/resources/message?view=graph-rest-1.0) é gravável na criação de mensagens. |


### <a name="project-rome-notifications-api"></a>Notificações de Rome API do Project

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição          | Beta        | Adicionar o tipo de recurso [notificação](/graph/api/resources/projectrome-notification?view=graph-rest-beta). |
| Adição          | Beta        | Adicionada a API [Criar e publicar notificação] (/ graph / api / projectrome_notification_post? View = graph-rest-beta).|

### <a name="security-apis"></a>APIs de segurança

| **Tipo de alteração** | **Versão** | **Descrição**              |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta       | A pontuação de segurança de APIs [API de segurança](/graph/api/resources/securescore-api-overview?view=graph-rest-beta) foi adicionada, incluindo os seguintes recursos e operações:<br/>[secureScores](/graph/api/resources/securescores?view=graph-rest-beta) (e entidades relacionadas)<br/>[Lista secureScores](/graph/api/securescores-list?view=graph-rest-beta)<br/>[secureScoreControlProfiles](/graph/api/resources/securescorecontrolprofiles?view=graph-rest-beta)<br/>[Lista secureScoreControlProfiles](/graph/api/securescorecontrolprofiles-list?view=graph-rest-beta)<br/>[Atualizar secureScoreControlProfiles](/graph/api/securescorecontrolprofiles-update?view=graph-rest-beta) |
| Adição        | Beta        | Introduzido um novo tipo complexo [secureScoreControlStateUpdate](/graph/api/resources/securescorecontrolstateupdate?view=graph-rest-beta) |


## <a name="august-2018"></a>Agosto de 2018

### <a name="delta-query"></a>Consulta delta

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Adicionado o recurso de [consulta delta](delta-query-overview.md) para as entidades a seguir no Azure Active Directory:<br/>[application](/graph/api/application-delta?view=graph-rest-beta)<br/>[directoryRole](/graph/api/directoryrole-delta?view=graph-rest-beta)<br/>[servicePrincipal](/graph/api/serviceprincipal-delta?view=graph-rest-beta) |

### <a name="directory-apis"></a>APIs de diretório

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição | v1.0 | Adicionada a propriedade isMultipleDataLocationsForServicesEnabled para o recurso [Organização](/graph/api/resources/organization?view=graph-rest-beta) que permite que os aplicativos verifiquem se esse locatário está habilitado para funcionalidades Multi-Geo. Adicionada a propriedade preferredDataLocation aos recursos [usuário](/graph/api/resources/user?view=graph-rest-beta) e [grupo](/graph/api/resources/group?view=graph-rest-beta) que permitem a configurar os locais de dados preferenciais para um usuário e um grupo.|
| Adição | v1.0 | Adicionada a propriedade [onPremisesProvisioningErrors](/graph/api/resources/onpremisesprovisioningerror?view=graph-rest-1.0) às entidades [Usuário](/graph/api/resources/user?view=graph-rest-1.0) e [Grupo](/graph/api/resources/group?view=graph-rest-1.0) que representa erros de sincronização de diretório ao sincronizar diretórios locais com o Active Directory do Azure ao usar o produto de sincronização da Microsoft (incluindo o Microsoft Azure AD Connect, DirSync e o MIM + Connector).|
| Adição | v1.0 | Adicionada a propriedade [onPremisesExtensionAttributes](/graph/api/resources/onpremisesextensionattributes?view=graph-rest-1.0) à entidade [User](/graph/api/resources/user?view=graph-rest-1.0) que contém quinze propriedades de atributo de extensão personalizadas. Para um usuário onPremisesSyncEnabled, esse conjunto de propriedades é masterizado no Active Directory local e sincronizado com o Azure Active Directory e é somente leitura. Para um usuário somente na nuvem (onde onPremisesSyncEnabled é falso), essas propriedades podem ser definidas durante a criação ou atualização.|
|Adição|v1.0|Foram adicionadas as propriedades **onPremisesDomainName**, **onPremisesSamAccountName** e **onPremisesUserPrincipalName** à entidade [User](/graph/api/resources/user?view=graph-rest-1.0)|

### <a name="microsoft-intune-apis"></a>APIs do Microsoft Intune

|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|v1.0|Foram adicionadas novas entidades:<br/>[androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-1.0)<br/>[androidWorkProfileCustomConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilecustomconfiguration?view=graph-rest-1.0)<br/>[androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-1.0)<br/>|
|Adição|v1.0|Foram adicionados novos tipos de enumeração:<br/>[androidWorkProfileCrossProfileDataSharingType](/graph/api/resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype?view=graph-rest-1.0)<br/>[androidWorkProfileDefaultAppPermissionPolicyType](/graph/api/resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype?view=graph-rest-1.0)<br/>[androidWorkProfileRequiredPasswordType](/graph/api/resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype?view=graph-rest-1.0)<br/>|
|Adição|v1.0|A função [managedDeviceEnrollmentFailureDetails](/graph/api/intune-shared-reportroot-manageddeviceenrollmentfailuredetails?view=graph-rest-1.0) foi adicionada ao [reportRoot](/graph/api/resources/intune-shared-reportroot?view=graph-rest-1.0) |
|Adição|v1.0|A função [managedDeviceEnrollmentTopFailures](/graph/api/intune-shared-reportroot-manageddeviceenrollmenttopfailures?view=graph-rest-1.0) foi adicionada ao [reportRoot](/graph/api/resources/intune-shared-reportroot?view=graph-rest-1.0) |
|Adição|v1.0|Adicionar a propriedade**kioskModeBuiltInAppId** para a entidade [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-1.0)|
|Adição|v1.0|Adicionar o membro **não atribuído** para o tipo de enumeração [complianceStatus](/graph/api/resources/intune-shared-compliancestatus?view=graph-rest-1.0)|
|Adição|v1.0|Adicionar o membro**pushNotification** para o tipo de enumeração[deviceComplianceActionType](/graph/api/resources/intune-deviceconfig-devicecomplianceactiontype?view=graph-rest-1.0)|
|Adição|v1.0|Adicionado o membro**userAbandonment** para o tipo de enumeração [deviceEnrollmentFailureReason](/graph/api/resources/intune-troubleshooting-deviceenrollmentfailurereason?view=graph-rest-1.0)|
|Adição|v1.0|Adicionados os membros **comprometidos** e **mal configurados** ao tipo de enumeração [managedDevicePartnerReportedHealthState](/graph/api/resources/intune-devices-manageddevicepartnerreportedhealthstate?view=graph-rest-1.0)|
|Adição|v1.0|Adicionar o membro **assignedToExternalMDM** para o tipo de enumeração [vppTokenState](/graph/api/resources/intune-onboarding-vpptokenstate?view=graph-rest-1.0)|
||
|Adição|beta|Foram adicionadas novas entidades:<br/>[advancedThreatProtectionOnboardingDeviceSettingState](/graph/api/resources/intune-deviceconfig-advancedthreatprotectiononboardingdevicesettingstate?view=graph-rest-beta)<br/>[advancedThreatProtectionOnboardingStateSummary](/graph/api/resources/intune-deviceconfig-advancedthreatprotectiononboardingstatesummary?view=graph-rest-beta)<br/>[depEnrollmentBaseProfile](/graph/api/resources/intune-enrollment-depenrollmentbaseprofile?view=graph-rest-beta)<br/>[depEnrollmentProfile](/graph/api/resources/intune-enrollment-depenrollmentprofile?view=graph-rest-beta)<br/>[depIOSEnrollmentProfile](/graph/api/resources/intune-enrollment-depiosenrollmentprofile?view=graph-rest-beta)<br/>[depMacOSEnrollmentProfile](/graph/api/resources/intune-enrollment-depmacosenrollmentprofile?view=graph-rest-beta)<br/>[enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta)<br/>[importedAppleDeviceIdentity](/graph/api/resources/intune-enrollment-importedappledeviceidentity?view=graph-rest-beta)<br/>[importedAppleDeviceIdentityResult](/graph/api/resources/intune-enrollment-importedappledeviceidentityresult?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta)<br/>[roleScopeTag](/graph/api/resources/intune-rbac-rolescopetag?view=graph-rest-beta)<br/>[windowsIdentityProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsidentityprotectionconfiguration?view=graph-rest-beta)<br/>|
|Adição|beta|Foram adicionados novos tipos complexos:<br/>[configurationManagerClientHealthState](/graph/api/resources/intune-devices-configurationmanagerclienthealthstate?view=graph-rest-beta)<br/>[customSubjectAlternativeName](/graph/api/resources/intune-deviceconfig-customsubjectalternativename?view=graph-rest-beta)<br/>[deviceManagementUserRightsLocalUserOrGroup](/graph/api/resources/intune-deviceconfig-devicemanagementuserrightslocaluserorgroup?view=graph-rest-beta)<br/>[deviceManagementUserRightsSetting](/graph/api/resources/intune-deviceconfig-devicemanagementuserrightssetting?view=graph-rest-beta)<br/>[managementCertificateWithThumbprint](/graph/api/resources/intune-enrollment-managementcertificatewiththumbprint?view=graph-rest-beta)<br/>[mobileAppSupportedDeviceType](/graph/api/resources/intune-troubleshooting-mobileappsupporteddevicetype?view=graph-rest-beta)<br/>[osVersionCount](/graph/api/resources/intune-devices-osversioncount?view=graph-rest-beta)<br/>[windowsMalwareCategoryCount](/graph/api/resources/intune-devices-windowsmalwarecategorycount?view=graph-rest-beta)<br/>[windowsMalwareExecutionStateCount](/graph/api/resources/intune-devices-windowsmalwareexecutionstatecount?view=graph-rest-beta)<br/>[windowsMalwareNameCount](/graph/api/resources/intune-devices-windowsmalwarenamecount?view=graph-rest-beta)<br/>[windowsMalwareOverview](/graph/api/resources/intune-devices-windowsmalwareoverview?view=graph-rest-beta)<br/>[windowsMalwareStateCount](/graph/api/resources/intune-devices-windowsmalwarestatecount?view=graph-rest-beta)<br/>|
|Adição|Beta|Foram adicionados novos tipos de enumeração:<br/>[configurationManagerClientState](/graph/api/resources/intune-devices-configurationmanagerclientstate?view=graph-rest-beta)<br/>[depTokenType](/graph/api/resources/intune-enrollment-deptokentype?view=graph-rest-beta)<br/>[discoverySource](/graph/api/resources/intune-enrollment-discoverysource?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentityUploadStatus](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus?view=graph-rest-beta)<br/>[iTunesPairingMode](/graph/api/resources/intune-enrollment-itunespairingmode?view=graph-rest-beta)<br/>[lanManagerAuthenticationLevel](/graph/api/resources/intune-deviceconfig-lanmanagerauthenticationlevel?view=graph-rest-beta)<br/>[localSecurityOptionsMinimumSessionSecurity](/graph/api/resources/intune-deviceconfig-localsecurityoptionsminimumsessionsecurity?view=graph-rest-beta)<br/>[resultantAppStateDetail](/graph/api/resources/intune-apps-resultantappstatedetail?view=graph-rest-beta)<br/>[vpnProviderType](/graph/api/resources/intune-deviceconfig-vpnprovidertype?view=graph-rest-beta)<br/>[windowsMalwareThreatState](/graph/api/resources/intune-devices-windowsmalwarethreatstate?view=graph-rest-beta)<br/>|
|Adição|beta|A ação [uploadDepToken](/graph/api/intune-enrollment-deponboardingsetting-uploaddeptoken?view=graph-rest-beta) em [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) foi adicionada |
|Adição|beta|A ação [syncWithAppleDeviceEnrollmentProgram](/graph/api/intune-enrollment-deponboardingsetting-syncwithappledeviceenrollmentprogram?view=graph-rest-beta) em [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) foi adicionada |
|Adição|beta|A ação [setDefaultProfile](/graph/api/intune-enrollment-enrollmentprofile-setdefaultprofile?view=graph-rest-beta) foi adicionada à entidade [enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta) |
|Adição|beta|Adicionada a ação **importAppleDeviceIdentityList** da coleção [importedAppleDeviceIdentity](/graph/api/resources/intune-enrollment-importedappledeviceidentity?view=graph-rest-beta) |
|Adição|beta|Adicionada a ação [updateDeviceProfileAssignment](/graph/api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment?view=graph-rest-beta) do [enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta) |
|Adição|beta|A ação [shareForSchoolDataSyncService](/graph/api/intune-enrollment-deponboardingsetting-shareforschooldatasyncservice?view=graph-rest-beta) foi adicionada à entidade [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) |
|Adição|beta|A ação [unshareForSchoolDataSyncService](/graph/api/intune-enrollment-deponboardingsetting-unshareforschooldatasyncservice?view=graph-rest-beta) foi adicionada à entidade [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) |
|Adição|beta|Adicionada a ação [assignUserFromDevice](/graph/api/intune-enrollment-windowsautopilotdeviceidentity-assignusertodevice?view=graph-rest-beta) em [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta) |
|Adição|beta|Adicionada a função [getRoleScopeTagsByResource](/graph/api/intune-rbac-devicemanagement-getrolescopetagsbyresource?view=graph-rest-beta) no [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) |
|Adição|beta|Adicionada a função[getRoleScopeTagsByIds](/graph/api/intune-rbac-devicemanagement-getrolescopetagsbyids?view=graph-rest-beta) em [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) |
|Adição|beta|A função [getEncryptionPublicKey](/graph/api/intune-enrollment-deponboardingsetting-getencryptionpublickey?view=graph-rest-beta) em [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) foi adicionada |
|Adição|beta|Adicionar a função[exportMobileConfig](/graph/api/intune-enrollment-enrollmentprofile-exportmobileconfig?view=graph-rest-beta) em[enrollmentProfile](/graph/api/resources/intune-enrollment-enrollmentprofile?view=graph-rest-beta) |
|Adição|beta|Adicionada a função [autopilotDeviceStream](/graph/api/intune-enrollment-importedwindowsautopilotdeviceidentityupload-autopilotdevicestream?view=graph-rest-beta) em [importedWindowsAutopilotDeviceIdentityUpload](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload?view=graph-rest-beta) |
|Exclusão|beta|Remover o conjunto **uploadDepToken** |
|Exclusão|beta|A ação **syncWithAppleDeviceEnrollmentProgram** na em [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) foi removida |
|Exclusão|beta|A função **getEncryptionPublicKey**foi removida em [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) |
|Adição|beta|Adicionada a propriedade **restrictedApps** na entidade[androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **vpnAlwaysOnPackageIdentifier** e **vpnEnableAlwaysOnLockdownMode** para a entidade[androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) |
|Exclusão|beta|Removida a propriedade **packageName**na entidade [androidForWorkMobileAppConfiguration](/graph/api/resources/intune-apps-androidforworkmobileappconfiguration?view=graph-rest-beta) |
|Adição|beta|Adicionada a propriedade **restrictedApps** na entidade[androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **vpnAlwaysOnPackageIdentifier** e **vpnEnableAlwaysOnLockdownMode** para a entidade[androidForWorkProfileDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta) |
|Adição|beta|A propriedade **optInToDeviceIdSharing** foi adicionada à entidade [appleVpnConfiguration](/graph/api/resources/intune-deviceconfig-applevpnconfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **tokenType**, **tokenName**, **syncedDeviceCount**, **defaultProfileDisplayName** e ** dataSharingConsentGranted** para a entidade[depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **roleScopeTagIds** para a entidade[deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **roleScopeTagIds** e **supportsScopeTags** à entidade [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade **windowsMalwareOverview** foi adicionada à entidade [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Alteração|beta|Foram alteradas as seguintes propriedades na entidade [iosCertificateProfileBase](/graph/api/resources/intune-deviceconfig-ioscertificateprofilebase?view=graph-rest-beta):<br/>**subjectAlternativeNameType** de obrigatória para opcional<br/>|
|Adição|beta|Adicionada a propriedade **restrictedApps** à entidade [iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-beta) |
|Adição|beta|Adicionadas as propriedades **certificateStore** e **customSubjectAlternativeNames** para a entidade[iosScepCertificateProfile](/graph/api/resources/intune-deviceconfig-iosscepcertificateprofile?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade**enforcedSoftwareUpdateDelayInDays** para a entidade [iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **providerType**, **userDomain**, **strictEnforcement**, **cloudName** e **excludeList**para a entidade [iosVpnConfiguration](/graph/api/resources/intune-deviceconfig-iosvpnconfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **safariBlockAutofill**, **cameraBlocked**, **iTunesBlockMusicService**, **spotlightBlockInternetResults**, **keyboardBlockDictation**, **definitionLookupBlocked**, **appleWatchBlockAutoUnlock**, **iTunesBlockFileSharing**, **iCloudBlockDocumentSync**, **iCloudBlockMail**, **iCloudBlockAddressBook**, **iCloudBlockCalendar** , **iCloudBlockReminders**, **iCloudBlockBookmarks**, **iCloudBlockNotes**, **airDropBlocked**, **passwordBlockModification** e **passwordBlockFingerprintUnlock** para a entidade[macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-beta) |
|Adição|beta|Adicionadas as propriedades **roleScopeTagIds**, **windowsActiveMalwareCount**, **windowsRemediatedMalwareCount**, **anotações** e **configurationManagerClientHealthState** para a entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Adição|beta|A propriedade **installStateDetail** foi adicionada à entidade [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta)|
|Adição|beta|Adicionar a propriedade **roleScopeTagIds** para a entidade [notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-beta) |
|Adição|beta|Adicionar as propriedades **targetVersion** e **updateVersion** para a entidade [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) |
|Adição|beta|Adicionada a propriedade **recurso** para a entidade [resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **localStorage**, **setPowerPolicies** e **signInOnResume** à entidade [sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **configurationManagerComplianceRequired** para a entidade [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta)|
|Adição|beta|Foram adicionadas as propriedades**userRightsAccessCredentialManagerAsTrustedCaller**, **userRightsAllowAccessFromNetwork**, **userRightsBlockAccessFromNetwork**, **userRightsActAsPartOfTheOperatingSystem**, **userRightsLocalLogOn**, **userRightsBackupData**, **userRightsChangeSystemTime**, **userRightsCreateGlobalObjects**, **userRightsCreatePageFile**, **userRightsCreatePermanentSharedObjects**, **userRightsCreateSymbolicLinks**, **userRightsCreateToken**, **userRightsDebugPrograms**, **userRightsRemoteDesktopServicesLogOn**, **userRightsDelegation**, **userRightsGenerateSecurityAudits**, **userRightsImpersonateClient**, ** userRightsIncreaseSchedulingPriority**, **userRightsLoadUnloadDrivers**, **userRightsLockMemory**, ** userRightsManageAuditingAndSecurityLogs**, **userRightsManageVolumes**, **userRightsModifyFirmwareEnvironment**, ** userRightsModifyObjectLabels**, **userRightsProfileSingleProcess**, **userRightsRemoteShutdown**, **userRightsRestoreData**, **userRightsTakeOwnership**, **userRightsRegisterProcessAsService**, ** localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedClients**, **localSecurityOptionsMinimumSessionSecurityForNtlmSspBasedServers**, ** lanManagerAuthenticationLevel** e **lanManagerWorkstationEnableInsecureGuestLogons** à entidade[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) |
|Adição|beta|Adicionada as propriedades **passwordMinimumAgeInDays**, **tenantLockdownRequireNetworkDuringOutOfBoxExperience** e **dataProtectionBlockDirectMemoryAccess** à entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **extendedKeyUsages** para a entidade [windows10PkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10pkcscertificateprofile?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **enableDnsRegistration** e **dnsSuffixes** para a entidade [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **customSubjectAlternativeNames** para a entidade[windows81CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows81certificateprofilebase?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **extractHardwareHash** e **deviceNameTemplate** para a entidade [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **addressableUserName** e **userPrincipalName** para a entidade [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **threatState** para a entidade [windowsDeviceMalwareState](/graph/api/resources/intune-devices-windowsdevicemalwarestate?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **qualityUpdatesPauseStartDateTime**, **featureUpdatesPauseStartDateTime**, **featureUpdatesRollbackWindowInDays**, ** qualityUpdatesWillBeRolledBack**, **featureUpdatesWillBeRolledBack**, **qualityUpdatesRollbackStartDateTime** e ** featureUpdatesRollbackStartDateTime** para a entidade [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) |
|Adição|beta|Adicionada a propriedade **trustedServerCertificateNames** para a entidade [windowsWifiEnterpriseEAPConfiguration](/graph/api/resources/intune-deviceconfig-windowswifienterpriseeapconfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades de navegação **defaultIosEnrollmentProfile**, **defaultMacOsEnrollmentProfile**, **enrollmentProfiles** e **importedAppleDeviceIdentities** para a entidade [depOnboardingSetting](/graph/api/resources/intune-enrollment-deponboardingsetting?view=graph-rest-beta) |
|Adição|beta|A propriedade de navegação **roleScopeTags** foi adicionada à entidade [deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades de navegação**advancedThreatProtectionOnboardingStateSummary**, **roleScopeTags** e **importedWindowsAutopilotDeviceIdentityUploads** à entidade [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **supportedDeviceTypes** para o tipo complexo [mobileAppIntentAndStateDetail](/graph/api/resources/intune-troubleshooting-mobileappintentandstatedetail?view=graph-rest-beta)|
|Adição|beta|A propriedade **hideEscapeLink** foi adicionada ao tipo complexo [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta)|
|Adição|beta|Os membros**zscalerPrivateAccess**, **f5Access2018**, **citrixSso** e **paloAltoGlobalProtectV2** foram adicionados ao tipo de enumeração[appleVpnConnectionType](/graph/api/resources/intune-deviceconfig-applevpnconnectiontype?view=graph-rest-beta)|
|Adição|beta|Adicionado o membro**userAbandonment** para o tipo de enumeração [deviceEnrollmentFailureReason](/graph/api/resources/intune-troubleshooting-deviceenrollmentfailurereason?view=graph-rest-beta)|
|Adição|beta|Adicionado o membro **bloqueados** na enumeração tipo [enrollmentState](/graph/api/resources/intune-enrollment-enrollmentstate?view=graph-rest-beta) |
|Adição|beta|Adicionado o membro**microsoft365ManagedMdm** na enumeração tipo [managementAgentType](/graph/api/resources/intune-devices-managementagenttype?view=graph-rest-beta)|
|Adição|beta|O membro **domainNameService** foi adicionado na enumeração tipo[subjectAlternativeNameType](/graph/api/resources/intune-deviceconfig-subjectalternativenametype?view=graph-rest-beta)|
|Adição|beta|Os membros **wpa2Personal** e **wpa2Enterprise** foram adicionados à enumeração tipo [wiFiSecurityType](/graph/api/resources/intune-deviceconfig-wifisecuritytype?view=graph-rest-beta) |
|Adição|beta|Os membros **enterpriseUnwantedSoftware**, **resgate** e **hipsRule**foram adicionados À enumeração tipo[windowsMalwareCategory](/graph/api/resources/intune-devices-windowsmalwarecategory?view=graph-rest-beta)|

### <a name="outlook-calendar"></a>Calendário do Outlook

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição | Beta | Os tipos complexos [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-beta) ação e o [freeBusyError](/graph/api/resources/freebusyerror?view=graph-rest-beta), [scheduleInformation](/graph/api/resources/scheduleinformation?view=graph-rest-beta), e [scheduleItem](/graph/api/resources/scheduleitem?view=graph-rest-beta) foram adicionados para oferecer suporte [obter informações de disponibilidade, informações de disponibilidade para listas de distribuição, usuários e recursos em um determinado período de tempo](outlook-get-free-busy-schedule.md). |

### <a name="outlook-mail"></a>Email do Outlook

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0        | Foi adicionado suporte para a ação [getMailTips](/graph/api/user-getmailtips?view=graph-rest-1.0) para obter Dicas de Email para destinatários específicos. Foram adicionados os seguintes recursos: [automaticRepliesMailTips](/graph/api/resources/automaticrepliesmailtips?view=graph-rest-1.0), [mailTips](/graph/api/resources/mailtips?view=graph-rest-1.0), [mailTipsError](/graph/api/resources/mailtipserror?view=graph-rest-1.0). |

### <a name="reports-apis"></a>APIs de relatórios
| Tipo de alteração | Versão | Descrição                              |
|:------------|:--------|:-----------------------------------------|
| Adição    | v1.0    | Adicionada a propriedade **ativado no computador compartilhado** para [getoffice365activationsuserdetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-1.0). |
| Adição    | v1.0    | Adicionada a propriedade **ativação de computador compartilhado** para [getoffice365activationsusercounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-1.0). |

### <a name="security-apis"></a>APIs de segurança

| **Tipo de alteração** | **Versão** | **Descrição**              |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | beta       | Adicionadas as propriedades**activityGroupName**, **cloudAppStates**, **confiança**, e **registryKeyStates** para [alerta ](/graph/api/resources/alert?view=graph-rest-beta ). |
|Exclusão|beta| Removidas as propriedades **activityGroupStates**, **applicationStates**, **malwareWasRunning**, **riskScore** e **tipo** do [alerta](/graph/api/resources/alert?view=graph-rest-beta ). |
|Alteração|beta| Tipo de **comentários** alterados de a `String`para a`String collection` e tipo de**gravidade** alterado de um `String`para um enum de  [alertSeverity](/graph/api/resources/alertseverityenumtype?view=graph-rest-beta) em [alerta](/graph/api/resources/alert?view=graph-rest-beta). |
| Adição        | beta       | Adicionar os seguintes tipos de recurso: <br/> [cloudAppSecurityState](/graph/api/resources/cloudappsecuritystate?view=graph-rest-beta) <br/> [fileHash](/graph/api/resources/filehash?view=graph-rest-beta) <br/> [registryKeyState](/graph/api/resources/registrykeystate?view=graph-rest-beta) |
|Exclusão|beta| Remover os seguintes tipos de recurso: <br/> **activityGroupState**  <br/> **applicationSecurityState** |
| Adição        | beta       | As seguintes enums foram adicionadas: <br/> [alertSeverity](/graph/api/resources/alertseverityenumtype?view=graph-rest-beta) <br/> [connectionDirection](/graph/api/resources/connectiondirectionenumtype?view=graph-rest-beta) <br/> [connectionStatus](/graph/api/resources/connectionstatusenumtype?view=graph-rest-beta) <br/> [emailRole](/graph/api/resources/emailroleenumtype?view=graph-rest-beta) <br/> [fileHashType](/graph/api/resources/filehashtypeenumtype?view=graph-rest-beta) <br/> [registryHive](/graph/api/resources/registryhiveenumtype?view=graph-rest-beta)  <br/> [registryOperation](/graph/api/resources/registryoperationenumtype?view=graph-rest-beta) <br/> [registryValueType](/graph/api/resources/registryvaluetypeenumtype?view=graph-rest-beta)|
|Exclusão|Beta| Foram removidos os seguintes tipos de enumeração: <br/> **alertType** <br/> **applicationPermissionsRequired** |
| Adição        | beta       | Adicionada a propriedade **fileHash**´para [fileSecurityState](/graph/api/resources/filesecuritystate?view=graph-rest-beta ).|
|Exclusão|beta| Removidas as propriedades **authenticodeHash256** e **sha256** de [fileSecurityState](/graph/api/resources/filesecuritystate?view=graph-rest-beta). |
| Adição | beta | Adicionadas a propriedade **sistema operacional**para [hostSecurityState](/graph/api/resources/hostsecuritystate?view=graph-rest-beta).|
| Adição | beta | Adicionadas as propriedades **categoria**, **família**, e **wasRunning** para [malwareState](/graph/api/resources/malwarestate?view=graph-rest-beta).|
|Exclusão|beta| Removida a propriedade **aliases** em [malwareState](/graph/api/resources/malwarestate?view=graph-rest-beta). |
|Alteração|beta| Movida a propriedade **malwareWasRunning** na [alerta](/graph/api/resources/alert?view=graph-rest-beta ) ao [malwareState](/graph/api/resources/malwarestate?view=graph-rest-beta) e renomeadas para **wasRunning**. |
| Adição        | beta       | Adicionadas as propriedades **applicationName**, **destinationDomain**, **direção**, **domainRegisteredDateTime**, **localDnsName **, **natDestinationAddress**, **natDestinationPort**, **natSourceAddress**, **natSourcePort** , **riskScore**, **status**, e **urlParameters** para[networkConnection](/graph/api/resources/networkconnection?view=graph-rest-beta ).|
|Alteração|beta| Alterada propriedade**uri** para **destinationUrl** no [networkConnection](/graph/api/resources/networkconnection?view=graph-rest-beta ). |
| Adição        | beta       | Adicionada a propriedade**fileHash** para[processo](/graph/api/resources/process?view=graph-rest-beta ).|
|Exclusão|beta| Removidas as propriedades **authenticodeHash256** e **sha256** de [processo](/graph/api/resources/process?view=graph-rest-beta ). |
| Adição        | beta       | Adicionadas as propriedades **aadUserId**, **emailRole**, **isVpn**, e **logonIp** para[userSecurityState](/graph/api/resources/usersecuritystate?view=graph-rest-beta).|
|Alteração|beta| Alterada a propriedade **logonIpAddress** para **logonIp** no [userSecurityState](/graph/api/resources/usersecuritystate?view=graph-rest-beta). |
| Adição        | beta       | Adicionada a propriedade**wasRunning** para [vulnerabilityState](/graph/api/resources/vulnerabilitystate?view=graph-rest-beta).|
|Exclusão|beta| Removida a propriedade **nome** em[vulnerabilityState](/graph/api/resources/vulnerabilitystate?view=graph-rest-beta). |

## <a name="july-2018"></a>Julho de 2018

### <a name="application-and-serviceprincipal-api-changes"></a>Alterações da API Application e servicePrincipal

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | As APIs de [aplicativo](/graph/api/resources/application?view=graph-rest-beta) e [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) serão atualizadas na visualização (beta). O primeiro conjunto de alterações será aplicado em 16 de julho de 2018. As alterações incluem a renomeação e a reestruturação de propriedade. A maioria das propriedades existentes não estará disponível até que as alterações sejam concluídas. Novas propriedades serão adicionadas. As alterações serão lançadas na Visualização (beta) antes do lançamento da versão 1.0. |

### <a name="directory-apis"></a>APIs de Diretório

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Alteração|beta|Atualizado o recurso [Mensagem de chat](/graph/api/resources/chatmessage?view=graph-rest-beta)|
|Adição|beta|Adicionado o tipo de recurso [Anexo de chat](/graph/api/resources/chatattachment?view=graph-rest-beta)|
|Adição|beta|Adicionado o tipo de recurso [Menção a chat](/graph/api/resources/chatattachment?view=graph-rest-beta)|
|Adição|beta|Adicionado o tipo de recurso [Reação a chat](/graph/api/resources/chatattachment?view=graph-rest-beta)|
|Adição|beta|Adicionada a [API Obter todas as mensagens de canal](/graph/api/channel-list-messages?view=graph-rest-beta) |
|Adição|beta|Adicionada a [API Obter mensagem do canal](/graph/api/channel-get-message?view=graph-rest-beta) |
|Adição|beta|Adicionada a [API Obter todas as respostas a mensagens](/graph/api/channel-list-messagereplies?view=graph-rest-beta) |
|Adição|beta|Adicionada a [API Obter resposta a mensagem](/graph/api/channel-get-messagereply?view=graph-rest-beta) |

### <a name="microsoft-teams-apis"></a>APIs do Microsoft Teams
| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Adição|beta|Adicionado o suporte a permissões do aplicativo para [/users/{id}/joinedTeams](/graph/api/user-list-joinedteams?view=graph-rest-beta) |
|Adição|beta|Adicionada a [API Obter todas as mensagens de canal](/graph/api/channel-list-messages?view=graph-rest-beta) |
|Adição|beta|Adicionada a [API Obter mensagem do canal](/graph/api/channel-get-message?view=graph-rest-beta) |
|Adição|beta|Adicionada a [API Obter todas as respostas a mensagens](/graph/api/channel-list-messagereplies?view=graph-rest-beta) |
|Adição|beta|Adicionada a [API Obter resposta a mensagem](/graph/api/channel-get-messagereply?view=graph-rest-beta) |
|Adição|beta|Adicionado o tipo de recurso [Anexo de chat](/graph/api/resources/chatattachment?view=graph-rest-beta)|
|Adição|beta|Adicionado o tipo de recurso [Menção a chat](/graph/api/resources/chatattachment?view=graph-rest-beta)|
|Adição|beta|Adicionado o tipo de recurso [Reação a chat](/graph/api/resources/chatattachment?view=graph-rest-beta)|
|Alteração|beta|Atualizado o recurso [Mensagem de chat](/graph/api/resources/chatmessage?view=graph-rest-beta))|
|Exclusão|beta|Removido DELETE /groups/{id}/team/channels/{id}, em vez disso use DELETE /teams/{id}/channels/{id}. |
|Exclusão|beta|Removido GET /groups/{id}/team/channels/{id}, em vez disso use GET /teams/{id}/channels/{id}. |
|Exclusão|beta|Removido PATCH /groups/{id}/team/channels/{id}, em vez disso use PATCH /teams/{id}/channels/{id}. |
|Exclusão|beta|Removido POST /groups/{id}/team/channels/{id}/chatthreads, em vez disso use POST /teams/{id}/channels/{id}/chatthreads. |
|Exclusão|beta|Removido GET /groups/{id}/team/channels, em vez disso use GET /teams/{id}/channels. |
|Exclusão|beta|Removido DELETE /groups/{id}/channels/{id}, em vez disso use DELETE /teams/{id}/channels/{id}. |
|Exclusão|beta|Removido GET /groups/{id}/channels/{id}, em vez disso use GET /teams/{id}/channels/{id}. |
|Exclusão|beta|Removido PATCH /groups/{id}/channels/{id}, em vez disso use PATCH /teams/{id}/channels/{id}. |
|Exclusão|beta|Removido POST /groups/{id}/channels/{id}/chatthreads, em vez disso use POST /teams/{id}/channels/{id}/chatthreads. |
|Exclusão|beta|Removido GET /groups/{id}/channels, em vez disso use GET /teams/{id}/channels. |
|Exclusão|beta|Removido POST /groups/{id}/team/channels, em vez disso use POST /teams/{id}/channels. |
|Exclusão|beta|Removido GET /groups/{id}/team, em vez disso use GET /teams/{id}. |
|Exclusão|beta|Removido PATCH /groups/{id}/team, em vez disso use PATCH /teams/{id}. |
|Adição|beta|Adicionada API para [listar todas as equipes da organização](teams-list-all-teams.md). |

### <a name="outlook-contacts"></a>Contatos do Outlook
| **Tipo de alteração** | **Versão**   | **Descrição**                          |
|:--------------- |:------------- |:---------------------------------------- |
|Adição |Beta | Adicionado o tipo complexo [typedEmailAddress](/graph/api/resources/typedemailaddress?view=graph-rest-beta). |
|Alteração | Beta | Alterado o tipo da propriedade **emailAddresses** de [contacto](/graph/api/resources/contact?view=graph-rest-beta) para ser um conjunto de instâncias **typedEmailAddress**.|

### <a name="synchronization-apis"></a>APIs de Sincronização

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição | Beta | Adicionadas as propriedades **andamento** [sychronizationStatus](/graph/api/resources/synchronization-synchronizationstatus?view=graph-rest-beta) para permitir que clientes monitorem o andamento de um trabalho de sincronização.|

### <a name="webhooks"></a>Webhooks
| Tipo de alteração | Versão | Descrição                              |
|:------------|:--------|:-----------------------------------------|
| Alteração significativa | Beta e v1.0 | [Webhooks](/graph/api/resources/webhooks?view=graph-rest-1.0) [reduzidos ao tempo de expiração máximo da assinatura](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type) para itens raiz da unidade, ou seja, três dias. |


## <a name="june-2018"></a>Junho de 2018

### <a name="directory-apis"></a>APIs de diretório

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição | Tudo | Novas permissões de aplicativos _Application.ReadWrite.All_ e __Application.ReadWrite.OwnedBy_ que permitem ao aplicativo cliente criar, ler, atualizar e excluir aplicativos e entidades de serviço como descrito no [tópico de permissões](permissions-reference.md#application-resource-permissions). |
| Adição | v1.0 | Adicionadas as propriedades **ageGroup**, **legalAgeGroupClassification**, e **ConsentRequiredForMinor** para recursos de [usuário](/graph/api/resources/user?view=graph-rest-1.0)

### <a name="identity-and-access-apis"></a>Identidades e acesso APIs

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição | beta | Adicionar o recurso [acessar avaliações](/graph/api/resources/accessreviews-root?view=graph-rest-beta) para [Azure AD](/graph/api/resources/azure-ad-overview?view=graph-rest-beta). |

### <a name="microsoft-intune-apis"></a>APIs do Microsoft Intune

|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|v1.0|A propriedade **connectorServerName** foi adicionada à entidade [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-1.0)|
|Adição|v1.0|As propriedades **firewallEnabled**, **firewallBlockAllIncoming** e **firewallEnableStealthMode** foram adicionadas à entidade [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-1.0)|
|Adição|v1.0|O membro **unknown** foi adicionado ao tipo de enumeração [iosUpdatesInstallStatus](/graph/api/resources/intune-deviceconfig-iosupdatesinstallstatus?view=graph-rest-1.0)|
|Adição|beta|Foram adicionadas novas entidades:<br/>[androidDeviceOwnerWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownerwificonfiguration?view=graph-rest-beta)<br/>[iosVppAppAssignedDeviceLicense](/graph/api/resources/intune-apps-iosvppappassigneddevicelicense?view=graph-rest-beta)<br/>[iosVppAppAssignedLicense](/graph/api/resources/intune-apps-iosvppappassignedlicense?view=graph-rest-beta)<br/>[iosVppAppAssignedUserLicense](/graph/api/resources/intune-apps-iosvppappassigneduserlicense?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationState](/graph/api/resources/intune-deviceconfig-manageddevicemobileappconfigurationstate?view=graph-rest-beta)<br/>[userPFXCertificate](/graph/api/resources/intune-raimportcerts-userpfxcertificate?view=graph-rest-beta)<br/>[vppTokenLicenseSummary](/graph/api/resources/intune-onboarding-vpptokenlicensesummary?view=graph-rest-beta)<br/>|
|Adição|beta|Foram adicionados novos tipos complexos:<br/>[iosVppAppRevokeLicensesActionResult](/graph/api/resources/intune-apps-iosvppapprevokelicensesactionresult?view=graph-rest-beta)<br/>|
|Adição|Beta|Foram adicionados novos tipos de enumeração:<br/>[androidDeviceOwnerSystemUpdateInstallType](/graph/api/resources/intune-deviceconfig-androiddeviceownersystemupdateinstalltype?view=graph-rest-beta)<br/>[androidDeviceOwnerWiFiSecurityType](/graph/api/resources/intune-deviceconfig-androiddeviceownerwifisecuritytype?view=graph-rest-beta)<br/>[userPfxIntendedPurpose](/graph/api/resources/intune-raimportcerts-userpfxintendedpurpose?view=graph-rest-beta)<br/>[userPfxPaddingScheme](/graph/api/resources/intune-raimportcerts-userpfxpaddingscheme?view=graph-rest-beta)<br/>|
|Adição|beta|A ação [createGooglePlayWebToken](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-creategoogleplaywebtoken?view=graph-rest-beta) foi adicionada a [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) |
|Adição|beta|A ação [revokeAllLicenses](/graph/api/intune-apps-iosvppapp-revokealllicenses?view=graph-rest-beta) foi adicionada a [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) |
|Adição|beta|A ação [revokeUserLicense](/graph/api/intune-apps-iosvppapp-revokeuserlicense?view=graph-rest-beta) foi adicionada a [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) |
|Adição|beta|A ação [revokeDeviceLicense](/graph/api/intune-apps-iosvppapp-revokedevicelicense?view=graph-rest-beta) foi adicionada a [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) |
|Adição|beta|A ação [sendCustomNotificationToCompanyPortal](/graph/api/intune-shared-devicemanagement-sendcustomnotificationtocompanyportal?view=graph-rest-beta) foi adicionada a [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) |
|Adição|beta|A ação **getLicensesForApp** foi adicionada ao conjunto [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) |
|Exclusão|Beta|Foram removidos os seguintes tipos de enumeração:<br/>**windowsUpdateInsiderBuildControl**<br/>|
|Adição|beta|As propriedades **systemUpdateWindowStartMinutesAfterMidnight**, **systemUpdateWindowEndMinutesAfterMidnight** e **systemUpdateInstallType** foram adicionadas à entidade [androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta)|
|Alteração|beta|Foi alterado o tipo das seguintes propriedades na entidade [androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta):<br/>**passwordMinutesOfInactivityBeforeScreenTimeout** de Int64 para Int32<br/>|
|Adição|beta|A propriedade **customKeyValueData** foi adicionada à entidade [androidForWorkVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkvpnconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade **customKeyValueData** foi adicionada à entidade [androidVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidvpnconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade **customKeyValueData** foi adicionada à entidade [androidWorkProfileVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade **customKeyValueData** foi adicionada à entidade [appleVpnConfiguration](/graph/api/resources/intune-deviceconfig-applevpnconfiguration?view=graph-rest-beta)|
|Adição|beta|As propriedades **userId** e **userPrincipalName** foram adicionadas à entidade [deviceCompliancePolicyState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicystate?view=graph-rest-beta)|
|Adição|beta|As propriedades **userId** e **userPrincipalName** foram adicionadas à entidade [deviceConfigurationState](/graph/api/resources/intune-deviceconfig-deviceconfigurationstate?view=graph-rest-beta)|
|Adição|beta|A propriedade **connectorServerName** foi adicionada à entidade [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-beta)|
|Exclusão|beta|A propriedade **settingXml** foi removida da entidade [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta)|
|Adição|beta|As propriedades **vppTokenId** e **revokeLicenseActionResults** foram adicionadas à entidade [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta)|
|Adição|beta|As propriedades **firewallEnabled**, **firewallBlockAllIncoming** e **firewallEnableStealthMode** foram adicionadas à entidade [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta)|
|Exclusão|beta|A propriedade **remoteAssistanceSessionErrorString** foi removida da entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Adição|beta|As propriedades **antivirusRequired** e **antiSpywareRequired** foram adicionadas à entidade [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta)|
|Adição|beta|As propriedades **defenderOfficeAppsOtherProcessInjection**, **defenderOfficeAppsExecutableContentCreationOrLaunch**, **defenderOfficeAppsLaunchChildProcess**, **defenderOfficeMacroCodeAllowWin32Imports**, **defenderScriptObfuscatedMacroCode**, **defenderScriptDownloadedPayloadExecution**, **defenderProcessCreation**, **defenderUntrustedUSBProcess**, **defenderUntrustedExecutable** e **defenderEmailContentExecution** foram adicionadas à entidade [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Adição|beta|As propriedades **searchDisableLocation**, **inkWorkspaceAccessState**, **defenderPotentiallyUnwantedAppActionSetting** e **defenderCloudExtendedTimeoutInSeconds** foram adicionadas à entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade **updatesMinimumAutoInstallClassification** foi adicionada à entidade [windows81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows81generalconfiguration?view=graph-rest-beta)|
|Exclusão|beta|A propriedade **previewBuildSetting** foi removida da entidade [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade de navegação **userPfxCertificates** foi adicionada à entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)|
|Adição|beta|A propriedade de navegação **assignedLicenses** foi adicionada à entidade [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta)|
|Adição|beta|A propriedade de navegação **managedDeviceMobileAppConfigurationStates** foi adicionada à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Adição|beta|A propriedade **websiteList** foi adicionada ao tipo complexo [iosWebContentFilterSpecificWebsitesAccess](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterspecificwebsitesaccess?view=graph-rest-beta)|
|Adição|beta|O membro **androidWorkProfile** foi adicionado ao tipo de enumeração [devicePlatformType](/graph/api/resources/intune-deviceconfig-deviceplatformtype?view=graph-rest-beta)|
|Adição|beta|O membro **notConfigured** foi adicionado ao tipo de enumeração [editionUpgradeLicenseType](/graph/api/resources/intune-deviceconfig-editionupgradelicensetype?view=graph-rest-beta)|
|Adição|beta|O membro **unknown** foi adicionado ao tipo de enumeração [iosUpdatesInstallStatus](/graph/api/resources/intune-deviceconfig-iosupdatesinstallstatus?view=graph-rest-beta)|
|Adição|beta|O membro **userRequestedInstall** foi adicionado ao tipo de enumeração [mobileAppActionType](/graph/api/resources/intune-troubleshooting-mobileappactiontype?view=graph-rest-beta)|
|Adição|beta|O membro **notConfigured** foi adicionado ao tipo de enumeração [windows10EditionType](/graph/api/resources/intune-deviceconfig-windows10editiontype?view=graph-rest-beta)

### <a name="microsoft-teams-apis"></a>APIs do Microsoft Teams
| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
|Adição         | Beta          | As APIs [archive](/graph/api/team-archive?view=graph-rest-beta) e [unarchive](/graph/api/team-unarchive?view=graph-rest-beta) de equipe foram adicionadas.|
|Adição         | Beta          | A operação [clone](/graph/api/team-clone?view=graph-rest-beta) foi adicionada. |
|Adição         | Beta          | As APIs foram adicionadas para adicionar e remover [apps](/graph/api/resources/teamsapp?view=graph-rest-beta) de equipes. |
|Alteração|Beta|Foi atualizado o caminho para a entidade [team](/graph/api/resources/team?view=graph-rest-beta).|
|Alteração|Beta|Foi atualizado o caminho para a entidade [channel](/graph/api/resources/channel?view=graph-rest-beta).|


### <a name="privileged-identity-management-apis"></a>APIs de Privileged Identity Management

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição | beta | A entidade [privilegedAccess](/graph/api/resources/privilegedaccess?view=graph-rest-beta) foi adicionada.|
| Adição | beta | A entidade [governanceResource](/graph/api/resources/governanceresource?view=graph-rest-beta) e os seguintes métodos e ações foram adicionados: <br> [List](/graph/api/governanceresource-list?view=graph-rest-beta) <br> [Get](/graph/api/governanceresource-get?view=graph-rest-beta)<br>|
| Adição | beta | A entidade [governanceSubject](/graph/api/resources/governancesubject?view=graph-rest-beta) foi adicionada.|
| Adição | beta | A entidade [governanceRoleDefinition](/graph/api/resources/governanceroledefinition?view=graph-rest-beta) e os seguintes métodos e ações foram adicionados:<br> [List](/graph/api/governanceroledefinition-list?view=graph-rest-beta) <br> [Get](/graph/api/governanceroledefinition-get?view=graph-rest-beta) |
| Adição | beta | A entidade [governanceRoleAssignment](/graph/api/resources/governanceroleassignment?view=graph-rest-beta) e os seguintes métodos e ações foram adicionados:<br> [List](/graph/api/governanceroleassignment-list?view=graph-rest-beta) <br> [Get](/graph/api/governanceroleassignment-get?view=graph-rest-beta) <br> [Export](/graph/api/governanceroleassignment-export?view=graph-rest-beta) |
| Adição | beta | A entidade [governanceRoleAssignmentRequest](/graph/api/resources/governanceroleassignmentrequest?view=graph-rest-beta) e os seguintes métodos e ações foram adicionados:<br> [List](/graph/api/governanceroleassignmentrequest-list?view=graph-rest-beta) <br> [Get](/graph/api/governanceroleassignmentrequest-get?view=graph-rest-beta) <br> [Create](/graph/api/governanceroleassignmentrequest-post?view=graph-rest-beta) <br> [Cancel](/graph/api/governanceroleassignmentrequest-cancel?view=graph-rest-beta) <br> [Update](/graph/api/governanceroleassignmentrequest-update?view=graph-rest-beta) |
| Adição | beta | A entidade [governanceRoleSetting](/graph/api/resources/governancerolesetting?view=graph-rest-beta) e os seguintes métodos e ações foram adicionados:<br> [List](/graph/api/governancerolesetting-list?view=graph-rest-beta) <br> [Get](/graph/api/governancerolesetting-get?view=graph-rest-beta) <br> [Update](/graph/api/governancerolesetting-update?view=graph-rest-beta) |
| Adição | beta | Os seguintes tipos complexos foram adicionados: <br> [governancePermission](/graph/api/resources/governancepermission?view=graph-rest-beta) <br> [governanceRoleAssignmentRequestStatus](/graph/api/resources/governanceroleassignmentrequeststatus?view=graph-rest-beta) <br> [governanceRuleSetting](/graph/api/resources/governancerulesetting?view=graph-rest-beta) <br> [governanceSchedule](/graph/api/resources/governanceschedule?view=graph-rest-beta)|

### <a name="security-apis"></a>APIs de segurança

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | Beta        | Foram adicionados novos tipos de enumeração:<br/>[alertFeedback](/graph/api/resources/alertfeedbackenumtype?view=graph-rest-beta)<br/>[alertStatus](/graph/api/resources/alertstatusenumtype?view=graph-rest-beta)<br/>[alertType](/graph/api/resources/alerttypeenumtype?view=graph-rest-beta)<br/>[applicationPermissionsRequired](/graph/api/resources/applicationpermissionsrequiredenumtype?view=graph-rest-beta)<br/>[logonType](/graph/api/resources/logontypeenumtype?view=graph-rest-beta)<br/>[processIntegrityLevel](/graph/api/resources/processintegritylevelenumtype?view=graph-rest-beta)<br/>[securityNetworkProtocol](/graph/api/resources/securitynetworkprotocolenumtype?view=graph-rest-beta)<br/>[userAccountSecurityType](/graph/api/resources/useraccountsecuritytypeenumtype?view=graph-rest-beta)<br/>

## <a name="may-2018"></a>Maio de 2018

### <a name="azure-ad-apis"></a>APIs do Azure AD

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Alteração           | Beta          | A propriedade **creatorUserId** da entidade [assinatura](/graph/api/resources/subscription?view=graph-rest-beta) foi renomeada para **creatorId** para refletir melhor o significado. |

### <a name="directory-apis"></a>APIs de Diretório

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0        | Foi adicionada a ação [Listar itens excluídos de propriedade de um usuário](/graph/api/directory-deleteditems-user-owned?view=graph-rest-1.0) ao recurso [directory (deleted items)](/graph/api/resources/directory?view=graph-rest-1.0) |
| Adição | beta | A função [getUserOwnedObjects](/graph/api/directory-deleteditems-user-owned?view=graph-rest-beta) foi adicionada ao recurso [directory](/graph/api/resources/directory?view=graph-rest-beta) para listar os grupos excluídos pertencentes a um determinado usuário. |

### <a name="education-api"></a>API de Educação

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Alteração          | v1.0 e beta | O escopo **Members.Read.Hidden** é necessário para ler ou atualizar o conjunto **Members** em uma entidade [educationClass](/graph/api/resources/educationclass?view=graph-rest-1.0) usando tokens somente de aplicativo. |
|Alteração           |Beta           |Atualizado os valores possíveis do tipo **educationSubmissionStatus** na propriedade de status do  [educationsubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta).|
|Alteração           |Beta           |Adicionado o tipo complexo **educationAssignmentIndividualRecipient** à propriedade assignTo do [educationAssignment](/graph/api/resources/educationassignment?view=graph-rest-beta).|
|Alteração           |Beta           |Adicionada a propriedade **unsubmittedBy**, **unsubmittedDate**, **returnedBy**, **returnedDate** do [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta).|
|Adição         |Beta           |Adicionada a ação [return](/graph/api/educationsubmission-return?view=graph-rest-beta) e [unsubmit](/graph/api/educationsubmission-unsubmit?view=graph-rest-beta) ao [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta).|
|Alteração           |Beta           |Removida a ação de lançamento e  cancelamento do [educationSubmission](/graph/api/resources/educationsubmission?view=graph-rest-beta).|

### <a name="groups"></a>Grupos

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0 e beta | A propriedade **importance** foi adicionada à entidade [post](/graph/api/resources/post?view=graph-rest-1.0). |

### <a name="insights-api"></a>API do Insights

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | Beta          | Foi adicionada a entidade [settings](/graph/api/resources/user-settings?view=graph-rest-beta) e os seguintes métodos CRUD: <br> [Get](/graph/api/user-get-settings?view=graph-rest-beta) <br> [Update](/graph/api/user-update-settings?view=graph-rest-beta) |

### <a name="microsoft-bookings-api"></a>API do Microsoft Bookings

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | Beta          | Foi adicionada a entidade [bookingBusiness](/graph/api/resources/bookingbusiness?view=graph-rest-beta) e os seguintes métodos e ações CRUD: <br> [List](/graph/api/bookingbusiness-list?view=graph-rest-beta) <br> [Create](/graph/api/bookingbusiness-post-bookingbusinesses?view=graph-rest-beta) <br> [Get](/graph/api/bookingbusiness-get?view=graph-rest-beta) <br> [Atualizar](/graph/api/bookingbusiness-update?view=graph-rest-beta) <br> [Delete](/graph/api/bookingbusiness-delete?view=graph-rest-beta) <br> [Publish](/graph/api/bookingbusiness-publish?view=graph-rest-beta) <br> [Unpublish](/graph/api/bookingbusiness-unpublish?view=graph-rest-beta). <br> Saiba mais sobre a integração com a [API do Microsoft Bookings](booking-concept-overview.md). |
| Adição        | Beta          | Foi adicionada a entidade [bookingAppointment](/graph/api/resources/bookingappointment?view=graph-rest-beta) e os seguintes métodos e ação CRUD: <br> [List](/graph/api/bookingbusiness-list-appointments?view=graph-rest-beta) <br> [Create](/graph/api/bookingbusiness-post-appointments?view=graph-rest-beta) <br> [Get](/graph/api/bookingappointment-get?view=graph-rest-beta) <br> [Atualizar](/graph/api/bookingappointment-update?view=graph-rest-beta) <br> [Delete](/graph/api/bookingappointment-delete?view=graph-rest-beta) <br> [Cancel](/graph/api/bookingappointment-cancel?view=graph-rest-beta). |
| Adição        | Beta          | Foi adicionada a entidade [bookingCurrency](/graph/api/resources/bookingcurrency?view=graph-rest-beta) e os seguintes métodos: <br> [List](/graph/api/bookingcurrency-list?view=graph-rest-beta) <br> [Get](/graph/api/bookingcurrency-get?view=graph-rest-beta). |
| Adição        | Beta          | Foi adicionada a entidade [bookingCustomer](/graph/api/resources/bookingcustomer?view=graph-rest-beta) e os seguintes métodos CRUD: <br> [List](/graph/api/bookingbusiness-list-customers?view=graph-rest-beta) <br> [Create](/graph/api/bookingbusiness-post-customers?view=graph-rest-beta) <br> [Get](/graph/api/bookingcustomer-get?view=graph-rest-beta) <br> [Update](/graph/api/bookingcustomer-update?view=graph-rest-beta) <br> [Delete](/graph/api/bookingcustomer-delete?view=graph-rest-beta).|
| Adição        | Beta          | Foi adicionada a entidade [bookingService](/graph/api/resources/bookingservice?view=graph-rest-beta) e os seguintes métodos CRUD: <br> [List](/graph/api/bookingbusiness-list-services?view=graph-rest-beta) <br> [Create](/graph/api/bookingbusiness-post-services?view=graph-rest-beta) <br> [Get](/graph/api/bookingservice-get?view=graph-rest-beta) <br> [Update](/graph/api/bookingservice-update?view=graph-rest-beta) <br> [Delete](/graph/api/bookingservice-delete?view=graph-rest-beta).|
| Adição        | Beta          | Foi adicionada a entidade [bookingStaffMember](/graph/api/resources/bookingstaffmember?view=graph-rest-beta) e os seguintes métodos CRUD: <br> [List](/graph/api/bookingbusiness-list-staffmembers?view=graph-rest-beta) <br> [Create](/graph/api/bookingbusiness-post-staffmembers?view=graph-rest-beta) <br> [Get](/graph/api/bookingstaffmember-get?view=graph-rest-beta) <br> [Update](/graph/api/bookingstaffmember-update?view=graph-rest-beta) <br> [Delete](/graph/api/bookingstaffmember-delete?view=graph-rest-beta).|
| Adição        | Beta          | Os seguintes tipos complexos foram adicionados: <br> [bookingNamedEntity](/graph/api/resources/bookingnamedentity?view=graph-rest-beta) <br> [bookingPerson](/graph/api/resources/bookingperson?view=graph-rest-beta) <br> [bookingReminder](/graph/api/resources/bookingreminder?view=graph-rest-beta) <br> [bookingWorkHours](/graph/api/resources/bookingworkhours?view=graph-rest-beta) <br> [bookingWorkTimeSlot](/graph/api/resources/bookingworktimeslot?view=graph-rest-beta).|

### <a name="microsoft-intune-apis"></a>APIs do Microsoft Intune
|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|beta|Foram adicionadas novas entidades:<br/>[androidWorkProfileCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidworkprofilecompliancepolicy?view=graph-rest-beta)<br/>[easEmailProfileConfigurationBase](/graph/api/resources/intune-deviceconfig-easemailprofileconfigurationbase?view=graph-rest-beta)<br/>[mobileAppIntentAndState](/graph/api/resources/intune-troubleshooting-mobileappintentandstate?view=graph-rest-beta)<br/>[mobileAppTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingevent?view=graph-rest-beta)<br/>[unsupportedDeviceConfiguration](/graph/api/resources/intune-deviceconfig-unsupporteddeviceconfiguration?view=graph-rest-beta)<br/>[windowsKioskConfiguration](/graph/api/resources/intune-deviceconfig-windowskioskconfiguration?view=graph-rest-beta)<br/>|
|Adição|beta|Foram adicionados novos tipos complexos:<br/>[managedDeviceCleanupSettings](/graph/api/resources/intune-devices-manageddevicecleanupsettings?view=graph-rest-beta)<br/>[mobileAppIntentAndStateDetail](/graph/api/resources/intune-troubleshooting-mobileappintentandstatedetail?view=graph-rest-beta)<br/>[mobileAppTroubleshootingAppPolicyCreationHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingapppolicycreationhistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingAppStateHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingappstatehistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingAppTargetHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingapptargethistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingAppUpdateHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingappupdatehistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingDeviceCheckinHistory](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootingdevicecheckinhistory?view=graph-rest-beta)<br/>[mobileAppTroubleshootingHistoryItem](/graph/api/resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem?view=graph-rest-beta)<br/>[unsupportedDeviceConfigurationDetail](/graph/api/resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail?view=graph-rest-beta)<br/>**windowsAutoPilotEnrollmentSettings**<br/>[windowsKioskActiveDirectoryGroup](/graph/api/resources/intune-deviceconfig-windowskioskactivedirectorygroup?view=graph-rest-beta)<br/>[windowsKioskAppBase](/graph/api/resources/intune-deviceconfig-windowskioskappbase?view=graph-rest-beta)<br/>[windowsKioskAppConfiguration](/graph/api/resources/intune-deviceconfig-windowskioskappconfiguration?view=graph-rest-beta)<br/>[windowsKioskAutologon](/graph/api/resources/intune-deviceconfig-windowskioskautologon?view=graph-rest-beta)<br/>[windowsKioskAzureADGroup](/graph/api/resources/intune-deviceconfig-windowskioskazureadgroup?view=graph-rest-beta)<br/>[windowsKioskAzureADUser](/graph/api/resources/intune-deviceconfig-windowskioskazureaduser?view=graph-rest-beta)<br/>[windowsKioskDesktopApp](/graph/api/resources/intune-deviceconfig-windowskioskdesktopapp?view=graph-rest-beta)<br/>[windowsKioskLocalGroup](/graph/api/resources/intune-deviceconfig-windowskiosklocalgroup?view=graph-rest-beta)<br/>[windowsKioskLocalUser](/graph/api/resources/intune-deviceconfig-windowskiosklocaluser?view=graph-rest-beta)<br/>[windowsKioskMultipleApps](/graph/api/resources/intune-deviceconfig-windowskioskmultipleapps?view=graph-rest-beta)<br/>[windowsKioskProfile](/graph/api/resources/intune-deviceconfig-windowskioskprofile?view=graph-rest-beta)<br/>[windowsKioskSingleUWPApp](/graph/api/resources/intune-deviceconfig-windowskiosksingleuwpapp?view=graph-rest-beta)<br/>[windowsKioskUser](/graph/api/resources/intune-deviceconfig-windowskioskuser?view=graph-rest-beta)<br/>[windowsKioskUWPApp](/graph/api/resources/intune-deviceconfig-windowskioskuwpapp?view=graph-rest-beta)<br/>[windowsKioskVisitor](/graph/api/resources/intune-deviceconfig-windowskioskvisitor?view=graph-rest-beta)<br/>|
|Adição|Beta|Foram adicionados novos tipos de enumeração:<br/>[defenderScheduleScanDay](/graph/api/resources/intune-deviceconfig-defenderschedulescanday?view=graph-rest-beta)<br/>[defenderSubmitSamplesConsentType](/graph/api/resources/intune-deviceconfig-defendersubmitsamplesconsenttype?view=graph-rest-beta)<br/>[domainNameSource](/graph/api/resources/intune-deviceconfig-domainnamesource?view=graph-rest-beta)<br/>[localSecurityOptionsSmartCardRemovalBehaviorType](/graph/api/resources/intune-deviceconfig-localsecurityoptionssmartcardremovalbehaviortype?view=graph-rest-beta)<br/>[mobileAppActionType](/graph/api/resources/intune-troubleshooting-mobileappactiontype?view=graph-rest-beta)<br/>[mobileAppIntent](/graph/api/resources/intune-troubleshooting-mobileappintent?view=graph-rest-beta)<br/>[roleAssignmentScopeType](/graph/api/resources/intune-rbac-roleassignmentscopetype?view=graph-rest-beta)<br/>[usernameSource](/graph/api/resources/intune-deviceconfig-usernamesource?view=graph-rest-beta)<br/>[windowsDeviceUsageType](/graph/api/resources/intune-enrollment-windowsdeviceusagetype?view=graph-rest-beta)<br/>|
|Adição|beta|Adicionado o [setDeviceName](/graph/api/intune-devices-manageddevice-setdevicename?view=graph-rest-beta)<br/>ação no [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|Exclusão|beta|Foram removidas as seguintes entidades:<br/>**depEnrollmentProfile**<br/>**enrollmentProfile**<br/>**importedAppleDeviceIdentity**<br/>**importedAppleDeviceIdentityResult**<br/>|
|Exclusão|beta|Foram removidos os seguintes tipos complexos:<br/>**managementCertificateWithThumbprint**<br/>|
|Exclusão|Beta|Foram removidos os seguintes tipos de enumeração:<br/>**depTokenType**<br/>**discoverySource**<br/>**iTunesPairingMode**<br/>|
|Exclusão|beta|Removida a ação importAppleDeviceIdentityList da coleção [importedAppleDeviceIdentity](/graph/api/resources/intune-corpenrollment-importedappledeviceidentity?view=graph-rest-beta) |
|Exclusão|beta|Removida a ação [updateDeviceProfileAssignment](/graph/api/intune-corpenrollment-enrollmentprofile-updatedeviceprofileassignment?view=graph-rest-beta) do [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) |
|Exclusão|beta|Removida a ação setDefaultProfile do [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) |
|Exclusão|beta|Removida a ação shareForSchoolDataSyncService do [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) |
|Exclusão|beta|Removida a ação unshareForSchoolDataSyncService do [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) |
|Exclusão|beta|Removida a função exportMobileConfig] (/ graph / api / intune_corpenrollment_enrollmentprofile_exportmobileconfig? View = graph-rest-beta) no [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) |
|Adição|beta|Adicionadas as propriedades **userDomainNameSource** e **customDomainName** à entidade [androidEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-androideasemailprofileconfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **workProfileBlockCamera** e **workProfileBlockCrossProfileContactsSearch** à entidade [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **workProfileBlockCamera** e **workProfileBlockCrossProfileContactsSearch** à entidade [androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **thirdPartyKeyboardsBlocked** e **filterOpenInToOnlyManagedApps** à entidade [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **conflictCount** à entidade [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **conflictCount** à entidade [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **managedDeviceCleanupSettings** à entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)|
|Exclusão|beta|Removida a propriedade **usernameSource** propriedade da entidade [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **thirdPartyKeyboardsBlocked** e **filterOpenInToOnlyManagedApps** à entidade [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **ignoreVersionDetection** à entidade [macOSLobApp](/graph/api/resources/intune-apps-macoslobapp?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **pinRequiredOnLaunchInsteadOfBiometric** e **pinRequiredInsteadOfBiometricTimeout** à entidade [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **autopilotEnrolled**, **requireUserEnrollmentApproval**, **iccid** e **udid** à entidade [ managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Exclusão|beta|Removida a propriedade **isAutopilotEnrolled** da entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **notApplicablePlatformCount** e **conflictCount** à entidade [managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **conflictCount** à entidade [managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **scopeType** à entidade [roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta)|
|Exclusão|beta|Removida a propriedade **usernameSource** da entidade [windows10EasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-windows10easemailprofileconfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **localSecurityOptionsDisableClientDigitallySignCommunicationsIfServerAgrees**, **localSecurityOptionsClientSendUnencryptedPasswordToThirdPartySMBServers**, **localSecurityOptionsDisableServerDigitallySignCommunicationsAlways**, **localSecurityOptionsDisableServerDigitallySignCommunicationsIfClientAgrees**, **localSecurityOptionsRestrictAnonymousAccessToNamedPipesAndShares**, **localSecurityOptionsDoNotAllowAnonymousEnumerationOfSAMAccounts**, **localSecurityOptionsAllowAnonymousEnumerationOfSAMAccountsAndShares**, **localSecurityOptionsDoNotStoreLANManagerHashValueOnNextPasswordChange** e **localSecurityOptionsSmartCardRemovalBehavior** à entidade [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **showInstallationProgress**, **blockDeviceSetupRetryByUser**, **allowDeviceResetOnInstallFailure**, ** allowLogCollectionOnInstallFailure**, **customErrorMessage**, **installProgressTimeoutInMinutes** e **allowDeviceUseOnInstallFailure** à entidade [windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta)|
|Exclusão|beta|Removidas as propriedades **title**, **bodyText**, **moreInfoUrl** e **moreInfoText** da entidade [ windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **defenderBlockOnAccessProtection**, **defenderScheduleScanDay** e **defenderSubmitSamplesConsentType** à entidade [ windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **language** e **enrollmentSettings** à entidade [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta)|
|Adição|beta|Adicionada a propriedade **useDeviceContext** à entidade [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta)|
|Exclusão|beta|Removida a propriedade **usernameSource** da entidade [windowsPhoneEASEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-windowsphoneeasemailprofileconfiguration?view=graph-rest-beta)|
|Exclusão|beta|Removida a propriedade **localActions** da entidade [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta)|
|Exclusão|beta|Removidas as propriedades **enrollmentProfiles** e **importedAppleDeviceIdentities** da entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades de navegação **mobileAppIntentAndStates** e **mobileAppTroubleshootingEvents** à entidade [user](/graph/api/resources/intune-shared-user?view=graph-rest-beta)|
|Adição|beta|Adicionadas as propriedades **deviceUsageType** e **skipKeyboardSelectionPage** ao tipo complexo [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta)|
|Exclusão|beta|Removido o membro **paloAltoGlobalProtect** do tipo de enumeração [androidForWorkVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidforworkvpnconnectiontype?view=graph-rest-beta)|
|Adição|beta|Adicionados os membros **samAccountName** e **primarySmtpAddress** ao tipo de enumeração [androidUsernameSource](/graph/api/resources/intune-deviceconfig-androidusernamesource?view=graph-rest-beta)|
|Exclusão|beta|Removido o membro **paloAltoGlobalProtect** do tipo de enumeração [androidVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidvpnconnectiontype?view=graph-rest-beta)|
|Adição|beta|Adicionado o membro **paloAltoGlobalProtect** ao tipo de enumeração [windows10VpnConnectionType](/graph/api/resources/intune-deviceconfig-windows10vpnconnectiontype?view=graph-rest-beta)|

## <a name="april-2018"></a>Abril de 2018

### <a name="audit-log-api"></a>API do log de auditoria

|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|Beta|Foram adicionadas as entidades [directoryAudit](/graph/api/resources/directoryaudit?view=graph-rest-beta) e [signIn](/graph/api/resources/signin?view=graph-rest-beta) para oferecer suporte à nova API de log de auditoria |
|Adição|Beta|Os seguintes recursos para oferecer suporte à API do log de auditoria foram adicionados: [appIndentity](/graph/api/resources/appidentity?view=graph-rest-beta), [auditActivityInitiator](/graph/api/resources/auditactivityinitiator?view=graph-rest-beta), [conditionalAccessPolicy](/graph/api/resources/conditionalaccesspolicy?view=graph-rest-beta), [deviceDetail](/graph/api/resources/devicedetail?view=graph-rest-beta), [mfaDetail](/graph/api/resources/mfadetail?view=graph-rest-beta), [modifiedProperty](/graph/api/resources/modifiedproperty?view=graph-rest-beta), [signinLocation](/graph/api/resources/signinlocation?view=graph-rest-beta), [signinStatus](/graph/api/resources/signinstatus?view=graph-rest-beta), [targetResource](/graph/api/resources/targetresource?view=graph-rest-beta), [targetResourceApp](/graph/api/resources/targetresourceapp?view=graph-rest-beta), [targetResourceDevice](/graph/api/resources/targetresourcedevice?view=graph-rest-beta), [targetResourceDirectory](/graph/api/resources/targetresourcedirectory?view=graph-rest-beta), [targetResourceGroup](/graph/api/resources/targetresourcegroup?view=graph-rest-beta), [targetResourceOther](/graph/api/resources/targetresourceother?view=graph-rest-beta), [targetResourcePolicy](/graph/api/resources/targetresourcepolicy?view=graph-rest-beta), [targetResourceRole](/graph/api/resources/targetresourcerole?view=graph-rest-beta), [targetResourceServicePrincipal](/graph/api/resources/targetresourceserviceprincipal?view=graph-rest-beta), [targetResourceUser](/graph/api/resources/targetresourceuser?view=graph-rest-beta), [userIdentity](/graph/api/resources/useridentity?view=graph-rest-beta) |

### <a name="directory-apis"></a>APIs de diretório

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Adicionado o tipo complexo **privacyProfile** à entidade [organization](/graph/api/resources/organization?view=graph-rest-1.0). |
| Adição        | v1.0        | Adicionado o tipo complexo **legalAgeGroup, ageGroup e consentProvidedForMinor** à entidade [user](/graph/api/resources/user?view=graph-rest-1.0). |
| Adição        | v1.0        | Foi adicionado suporte a usuários e grupos nas assinaturas de notificação do [webhook](/graph/api/resources/webhooks?view=graph-rest-1.0). |
| Adição        | Beta        | Foi adicionada a ação [Listar itens excluídos de propriedade de um usuário](/graph/api/directory-deleteditems-user-owned?view=graph-rest-beta) ao recurso [directory (deleted items)](/graph/api/resources/directory?view=graph-rest-beta) |

### <a name="education-apis"></a>APIs de educação

|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Alteração|Beta|Adição da propriedade reportableIdentifier a [educationsynchronizationerror](/graph/api/resources/educationsynchronizationerror?view=graph-rest-beta).|
|Alteração|Beta|Atualização das opções de resposta para a API [uploadUrl](/graph/api/educationsynchronizationprofile-uploadurl?view=graph-rest-beta).|
|Alteração|Beta|Atualização do texto de descrição do tipo de recurso [educationSynchronizationError](/graph/api/resources/educationsynchronizationerror?view=graph-rest-beta).|
|Alteração|Beta|Atualização do texto de descrição da API [obter erros de sincronização](/graph/api/educationsynchronizationerrors-get?view=graph-rest-beta).|


### <a name="microsoft-intune-apis"></a>APIs do Microsoft Intune
|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|v1.0|Foram adicionadas novas entidades:<br/>[managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-1.0)<br/>|
|Adição|v1.0|Foram adicionados novos tipos de enumeração:<br/>[managedDeviceOwnerType](/graph/api/resources/intune-devices-manageddeviceownertype?view=graph-rest-1.0)<br/>|
|Adição|v1.0|Foi adicionada a propriedade **managedDeviceOwnerType** à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0)|
|Adição|v1.0|Foi adicionada a propriedade de navegação **deviceStatuses** à entidade [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-1.0)|
|Adição|v1.0|Foi adicionado o membro **androidWorkProfile** ao tipo de enumeração [policyPlatformType](/graph/api/resources/intune-deviceconfig-policyplatformtype?view=graph-rest-1.0)|
|Adição|beta|Foram adicionadas novas entidades:<br/>[androidWorkProfileCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofilecertificateprofilebase?view=graph-rest-beta)<br/>[androidWorkProfileCustomConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilecustomconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileEasEmailProfileBase](/graph/api/resources/intune-deviceconfig-androidworkprofileeasemailprofilebase?view=graph-rest-beta)<br/>[androidWorkProfileEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofileenterprisewificonfiguration?view=graph-rest-beta)<br/>[androidWorkProfileGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileGmailEasConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileNineWorkEasConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration?view=graph-rest-beta)<br/>[androidWorkProfilePkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile?view=graph-rest-beta)<br/>[androidWorkProfileScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidworkprofilescepcertificateprofile?view=graph-rest-beta)<br/>[androidWorkProfileTrustedRootCertificate](/graph/api/resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate?view=graph-rest-beta)<br/>[androidWorkProfileVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconfiguration?view=graph-rest-beta)<br/>[androidWorkProfileWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidworkprofilewificonfiguration?view=graph-rest-beta)<br/>[restrictedAppsViolation](/graph/api/resources/intune-deviceconfig-restrictedappsviolation?view=graph-rest-beta)<br/>[windowsAutopilotDeploymentProfileAssignment](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofileassignment?view=graph-rest-beta)<br/>|
|Adição|beta|Foram adicionados novos tipos complexos:<br/>[managedDeviceModelsAndManufacturers](/graph/api/resources/intune-devices-manageddevicemodelsandmanufacturers?view=graph-rest-beta)<br/>[managedDeviceReportedApp](/graph/api/resources/intune-devices-manageddevicereportedapp?view=graph-rest-beta)<br/>[windowsEnrollmentStatusScreenSettings](/graph/api/resources/intune-enrollment-windowsenrollmentstatusscreensettings?view=graph-rest-beta)<br/>|
|Adição|Beta|Foram adicionados novos tipos de enumeração:<br/>[androidWorkProfileCrossProfileDataSharingType](/graph/api/resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype?view=graph-rest-beta)<br/>[androidWorkProfileDefaultAppPermissionPolicyType](/graph/api/resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype?view=graph-rest-beta)<br/>[androidWorkProfileRequiredPasswordType](/graph/api/resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype?view=graph-rest-beta)<br/>[androidWorkProfileVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidworkprofilevpnconnectiontype?view=graph-rest-beta)<br/>[bitLockerRecoveryInformationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryinformationtype?view=graph-rest-beta)<br/>[localSecurityOptionsInformationShownOnLockScreenType](/graph/api/resources/intune-deviceconfig-localsecurityoptionsinformationshownonlockscreentype?view=graph-rest-beta)<br/>[managedAppRemediationAction](/graph/api/resources/intune-mam-managedappremediationaction?view=graph-rest-beta)<br/>[managedDeviceOwnerType](/graph/api/resources/intune-devices-manageddeviceownertype?view=graph-rest-beta)<br/>[restrictedAppsState](/graph/api/resources/intune-deviceconfig-restrictedappsstate?view=graph-rest-beta)<br/>[windows10VpnProfileTarget](/graph/api/resources/intune-deviceconfig-windows10vpnprofiletarget?view=graph-rest-beta)<br/>|
|Adição|Beta|Foi adicionada a ação [playLostModeSound](/graph/api/intune-devices-manageddevice-playlostmodesound?view=graph-rest-beta) em [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|Exclusão|Beta|Foram removidos os seguintes tipos de enumeração:<br/>**bitLockerRecoveryinformationType**<br/>**windowsUpdateRestartMode**<br/>|
|Adição|Beta|Foram adicionadas as propriedades **workProfileBlockScreenCapture** e **workProfileBlockCrossProfileCallerId** à entidade [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta)|
|Adição|Beta|Foram adicionadas as propriedades **minimumWipePatchVersion**, **allowedAndroidDeviceManufacturers** e **appActionIfAndroidDeviceManufacturerNotAllowed** à entidade [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta)|
|Adição|Beta|Foram adicionadas as propriedades **minimumWipeSdkVersion**, **minimumWipePatchVersion**, **allowedIosDeviceModels**, **appActionIfIosDeviceModelNotAllowed**, **allowedAndroidDeviceManufacturers** e **appActionIfAndroidDeviceManufacturerNotAllowed** à entidade [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)|
|Adição|Beta|Foram adicionadas as propriedades **notApplicablePlatformCount** e **conflictCount** à entidade [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta)|
|Adição|Beta|Foram adicionadas as propriedades **notApplicablePlatformCount** e **conflictCount** à entidade [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta)|
|Adição|Beta|Foi adicionada a propriedade **accountMoveCompletionDateTime** à entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)|
|Adição|Beta|Foram adicionadas as propriedades **minimumWipeSdkVersion**, **allowedIosDeviceModels** e **appActionIfIosDeviceModelNotAllowed** à entidade [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta)|
|Adição|Beta|Foram adicionadas as propriedades **minimumWipeOsVersion**, **minimumWipeAppVersion**, **appActionIfDeviceComplianceRequired** e **appActionIfMaximumPinRetriesExceeded** à entidade [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta)|
|Adição|Beta|Foram adicionadas as propriedades **managedDeviceOwnerType**, **preferMdmOverGroupPolicyAppliedDateTime**, **isAutopilotEnrolled** e **requestUserEnrollmentApproval** à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Adição|Beta|Foi adicionada a propriedade **managedDeviceModelsAndManufacturers** à entidade [managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-beta)|
|Adição|Beta|Foram adicionadas as propriedades **localSecurityOptionsMachineInactivityLimitInMinutes**, **localSecurityOptionsAllowRemoteCallsToSecurityAccountsManagerHelperBool**, **localSecurityOptionsInformationShownOnLockScreen**, **defenderSecurityCenterDisableAccountUI**, **defenderSecurityCenterDisableHardwareUI**, **defenderSecurityCenterDisableRansomwareUI**, **defenderSecurityCenterDisableSecureBootUI** e **defenderSecurityCenterDisableTroubleshootingUI** à entidade [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Adição|Beta|Foram adicionadas as propriedades **printerNames**, **printerDefaultName**, **printerBlockAddition** e **searchBlockWebResults** à entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Adição|Beta|Foram adicionadas as propriedades **profileTarget**, **enableAlwaysOn** e **enableDeviceTunnel** à entidade [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta)|
|Adição|Beta|Foi adicionada a propriedade **enrollmentStatusScreenSettings** à entidade [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta)|
|Adição|Beta|Foi adicionada a propriedade de navegação **deviceConfigurationRestrictedAppsViolations** à entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)|
|Adição|Beta|Foi adicionada a propriedade de navegação **assignments** à entidade [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta)|
|Adição|Beta|Foi adicionada a propriedade de navegação **networkAccessConfigurations** à entidade [windowsDomainJoinConfiguration](/graph/api/resources/intune-deviceconfig-windowsdomainjoinconfiguration?view=graph-rest-beta)|
|Exclusão|Beta|Foi removida a propriedade **permissions** do tipo complexo [auditActor](/graph/api/resources/intune-auditing-auditactor?view=graph-rest-beta)|
|Alteração|beta|Foi alterado o tipo das seguintes propriedades no tipo complexo [bitLockerRecoveryOptions](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryoptions?view=graph-rest-beta):<br/>**recoveryInformationToStore** de [bitLockerRecoveryinformationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryinformationtype?view=graph-rest-beta) para [bitLockerRecoveryInformationType](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryinformationtype?view=graph-rest-beta)<br/>|
|Adição|Beta|Foi adicionada a propriedade **deviceInactivityBeforeRetirementInDay** ao tipo complexo [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta)|
|Adição|Beta|Foi adicionada a propriedade **landingPageCustomizedImage** ao tipo complexo [intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta)|
|Exclusão|Beta|Foi removida a propriedade **ipAddressOrFqdn** do tipo complexo [vpnServer](/graph/api/resources/intune-deviceconfig-vpnserver?view=graph-rest-beta)|
|Exclusão|Beta|Foi removida a propriedade **restartMode** do tipo complexo [windowsUpdateScheduledInstall](/graph/api/resources/intune-deviceconfig-windowsupdatescheduledinstall?view=graph-rest-beta)|
|Adição|Beta|Foi adicionado o membro **paloAltoGlobalProtect** ao tipo de enumeração [androidForWorkVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidforworkvpnconnectiontype?view=graph-rest-beta)|
|Adição|Beta|Foi adicionado o membro **paloAltoGlobalProtect** ao tipo de enumeração [androidVpnConnectionType](/graph/api/resources/intune-deviceconfig-androidvpnconnectiontype?view=graph-rest-beta)|
|Adição|Beta|Foi adicionado o membro **paloAltoGlobalProtect** ao tipo de enumeração [appleVpnConnectionType](/graph/api/resources/intune-deviceconfig-applevpnconnectiontype?view=graph-rest-beta)|
|Adição|Beta|Foi adicionado o membro **androidWorkProfile** ao tipo de enumeração [policyPlatformType](/graph/api/resources/intune-deviceconfig-policyplatformtype?view=graph-rest-beta)|

### <a name="microsoft-teams"></a>Microsoft Teams

|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|Beta|Foi adicionada a nova entidade [teamMemberSettings](/graph/api/resources/teammembersettings?view=graph-rest-beta).|
|Adição|Beta|Foi adicionada a nova entidade [teamGuestSettings](/graph/api/resources/teamguestsettings?view=graph-rest-beta).|
|Adição|Beta|Foi adicionada a nova entidade [teamMessagingSettings](/graph/api/resources/teammessagingsettings?view=graph-rest-beta).|
|Adição|Beta|Foi adicionada a nova entidade [teamFunSettings](/graph/api/resources/teamfunsettings?view=graph-rest-beta).|
|Adição|Beta|Foi adicionada a nova operação [delete channel](/graph/api/channel-delete?view=graph-rest-beta).|
|Adição|Beta|Foi adicionada a nova operação [patch channel](/graph/api/channel-patch?view=graph-rest-beta).|
|Adição|Beta|A nova propriedade webUrl foi adicionada ao recurso [team](/graph/api/resources/team?view=graph-rest-beta).|
|Alteração|Beta|Foi atualizado o caminho para a entidade [channel](/graph/api/resources/channel?view=graph-rest-beta).|

### <a name="outlook-calendar"></a>Calendário do Outlook

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0          | A propriedade **locations** foi adicionada à entidade [event](/graph/api/resources/event?view=graph-rest-1.0) para dar suporte à organização de um evento em que os participantes podem participar de mais de um local. |
| Adição        | v1.0          | A propriedade **locationType** foi adicionada ao tipo complexo [location](/graph/api/resources/location?view=graph-rest-1.0). |
| Adição        | v1.0          | As propriedades **uniqueId** e **uniqueIdType** foram adicionadas ao tipo complexo [location](/graph/api/resources/location?view=graph-rest-1.0). Atualmente, essas propriedades são apenas para uso interno. |


### <a name="outlook-contacts"></a>Contatos do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0          | Adição da propriedade **flag** à entidade [contact](/graph/api/resources/contact?view=graph-rest-1.0). Adição do tipo complexo [followupFlag](/graph/api/resources/followupflag?view=graph-rest-1.0) compartilhado.|


### <a name="outlook-mail"></a>Email do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0          | Adição da propriedade **flag** à entidade [message](/graph/api/resources/message?view=graph-rest-1.0). Adição do tipo complexo [followupFlag](/graph/api/resources/followupflag?view=graph-rest-1.0) compartilhado.|
| Adição        | v1.0        | A propriedade **internetMessageHeaders** foi adicionada à entidade [message](/graph/api/resources/message?view=graph-rest-1.0). |
| Adição        | v1.0        | O tipo complexo [internetMessageHeader](/graph/api/resources/internetmessageheader?view=graph-rest-1.0) foi adicionado. |
| Adição        | v1.0        | A propriedade de navegação **messageRules** foi adicionada à entidade [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0). **messageRules** é uma coleção das instâncias [messageRule](/graph/api/resources/messagerule?view=graph-rest-1.0). |
| Adição        | v1.0        | A entidade [messageRule](/graph/api/resources/messagerule?view=graph-rest-1.0) e os tipos complexos [messageRuleActions](/graph/api/resources/messageruleactions?view=graph-rest-1.0), [messageRulePredicates](/graph/api/resources/messagerulepredicates?view=graph-rest-1.0) e [sizeRange](/graph/api/resources/sizerange?view=graph-rest-1.0) foram adicionados. |
| Adição        | v1.0        | As seguintes operações CRUD às regras de mensagem foram adicionadas: [create](/graph/api/mailfolder-post-messagerules?view=graph-rest-1.0), [list](/graph/api/mailfolder-list-messagerules?view=graph-rest-1.0), [get](/graph/api/messagerule-get?view=graph-rest-1.0), [update](/graph/api/messagerule-update?view=graph-rest-1.0) e [delete](/graph/api/messagerule-delete?view=graph-rest-1.0). |
| Adição | Beta | Adicionado [mailSearchFolder](/graph/api/resources/mailsearchfolder?view=graph-rest-beta). |
| Adição | Beta | Adição das seguintes APIs à pasta de pesquisa de email: [Criar](/graph/api/mailsearchfolder-post?view=graph-rest-beta), [Atualizar](/graph/api/mailsearchfolder-update?view=graph-rest-beta). |
| Alteração | Beta | Adição de suporte para a pasta de pesquisa de email [excluir mailFolder](/graph/api/mailfolder-delete?view=graph-rest-beta), [obter mailFolder](/graph/api/mailfolder-get?view=graph-rest-beta) e [listar pastas filhas](/graph/api/mailfolder-list-childfolders?view=graph-rest-beta). |


### <a name="outlook-user-choices"></a>Opções de usuário do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | A nova propriedade de navegação **masterCategories** foi adicionada à entidade [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-1.0). **masterCategories** é uma coleção de objetos [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-1.0). |
| Adição        | v1.0        | A entidade [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-1.0) foi adicionada. |
| Adição        | v1.0        | As seguintes operações CRUD para [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-1.0) foram adicionadas: [create](/graph/api/outlookuser-post-mastercategories?view=graph-rest-1.0), [get](/graph/api/outlookcategory-get?view=graph-rest-1.0), [update](/graph/api/outlookcategory-update?view=graph-rest-1.0) e [delete](/graph/api/outlookcategory-delete?view=graph-rest-1.0). |
| Adição        | v1.0        | A nova função [supportedLanguages](/graph/api/outlookuser-supportedlanguages?view=graph-rest-1.0) foi adicionada à entidade [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-1.0). |
| Adição        | v1.0        | A nova função [supportedTimeZones](/graph/api/outlookuser-supportedtimezones?view=graph-rest-1.0) foi adicionada à entidade [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-1.0). |
|Adição | v1.0 | A nova propriedade **workingHours** foi adicionada a [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-1.0). Confira [tipo de recurso workingHours](/graph/api/resources/workinghours?view=graph-rest-1.0) para saber mais sobre casos de uso com suporte.|
|Adição | v1.0 | Os seguintes tipos complexos foram adicionados: <br> [workingHours](/graph/api/resources/workinghours?view=graph-rest-1.0) <br> [timeZoneBase](/graph/api/resources/timezonebase?view=graph-rest-1.0) <br> [customTimeZone](/graph/api/resources/customtimezone?view=graph-rest-1.0) <br> [standardTimeZoneOffset](/graph/api/resources/standardtimezoneoffset?view=graph-rest-1.0) <br> [daylightTimeZoneOffset](/graph/api/resources/daylighttimezoneoffset?view=graph-rest-1.0)|


### <a name="project-rome-apis"></a>APIs do Project Rome

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição | v1.0 | A API [Obter atividades recentes](/graph/api/projectrome-get-recent-activities?view=graph-rest-1.0) foi adicionada |
| Adição | v1.0 | A API [Obter atividades](/graph/api/projectrome-get-activities?view=graph-rest-1.0) foi adicionada |
| Adição | v1.0 | Foi adicionada a [Upsert Activity](/graph/api/projectrome-put-activity?view=graph-rest-1.0) |
| Adição | v1.0 | Foi adicionado [Upsert HistoryItem](/graph/api/projectrome-put-historyitem?view=graph-rest-1.0) |
| Adição | v1.0 | Foi adicionada a [Delete Activity](/graph/api/projectrome-delete-activity?view=graph-rest-1.0) |
| Adição | v1.0 | Foi adicionado [Upsert HistoryItem](/graph/api/projectrome-delete-historyitem?view=graph-rest-1.0) |
| Adição | v1.0 | Foi adicionada [activity](/graph/api/resources/projectrome-activity?view=graph-rest-1.0) |
| Adição | v.10 | Foi adicionado [HistoryItem](/graph/api/resources/projectrome-historyitem?view=graph-rest-1.0) |
| Adição | v1.0 | Foi adicionado [visualInfo](/graph/api/resources/projectrome-visualinfo?view=graph-rest-1.0) |
| Adição | v1.0 | Foi adicionado [imageInfo](/graph/api/resources/projectrome-imageinfo?view=graph-rest-1.0) |
| Adição | v.10 | Foi adicionada a [visão geral do Project Rome](/graph/api/resources/project-rome-overview?view=graph-rest-1.0) |
| Alteração | Beta | Foi adicionada a documentação de deep insert para [Upsert Activity](/graph/api/projectrome-put-activity?view=graph-rest-beta) |

### <a name="reports-apis"></a>APIs de relatórios
|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|beta| Adição de suporte para acesso do delegado. |
|Adição|v1.0| Adição de suporte para acesso delegado. |

### <a name="security-apis"></a>APIs de segurança

| **Tipo de alteração** | **Versão** | **Descrição**              |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta       | A [API de segurança](/graph/api/resources/security-api-overview?view=graph-rest-beta) foi adicionada, incluindo os seguintes recursos e operações:<br/>[alerta](/graph/api/resources/alert?view=graph-rest-beta) (e entidades relacionadas)<br/>[Obter alerta](/graph/api/alert-get?view=graph-rest-beta)<br/>[Listar alertas](/graph/api/alert-list?view=graph-rest-beta)<br/>[Atualizar alertas](/graph/api/alert-update?view=graph-rest-beta)<br/><br/>A seguinte documentação de suporte foi adicionada:<br/>[Erros](/graph/api/resources/security-error-codes?view=graph-rest-beta)<br/>[Integrar com um SIEM](security-siemintegration.md)


## <a name="march-2018"></a>Março de 2018

### <a name="activityfeedservice-apis"></a>APIs de ActivityFeedService

| **Tipo de alteração** | **Versão** | **Descrição**              |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta       | A [API Obter atividades recentes](/graph/api/projectrome-get-recent-activities?view=graph-rest-beta) foi adicionada |
| Adição        | Beta       | A [API Obter atividades](/graph/api/projectrome-get-activities?view=graph-rest-beta) foi adicionada |
| Alteração | Beta | A permissão UserActivity.ReadWrite.CreatedByApp foi adicionada a [Upsert Activity](/graph/api/projectrome-put-activity?view=graph-rest-beta) |
| Alteração | Beta | A permissão UserActivity.ReadWrite.CreatedByApp foi adicionada a [Upsert HistoryItem](/graph/api/projectrome-put-historyitem?view=graph-rest-beta) |
| Alteração | Beta | A permissão UserActivity.ReadWrite.CreatedByApp foi adicionada a [Excluir Atividade](/graph/api/projectrome-delete-activity?view=graph-rest-beta) |
| Alteração | Beta | A permissão UserActivity.ReadWrite.CreatedByApp foi adicionada a [Upsert HistoryItem](/graph/api/projectrome-delete-historyitem?view=graph-rest-beta) |
| Alteração | Beta | A propriedade **status** foi adicionada a [activity](/graph/api/resources/projectrome-activity?view=graph-rest-beta) |
| Alteração | Beta | A propriedade de navegação **activity** foi adicionada a [historyItem](/graph/api/resources/projectrome-historyitem?view=graph-rest-beta) |
| Alteração | Beta | As novas APIs foram adicionadas a [Visão geral do Project Rome](/graph/api/resources/project-rome-overview?view=graph-rest-beta) |

### <a name="azure-ad-apis"></a>APIs do Azure AD

|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Alteração|beta|As propriedades **applicationID** e **creatorUserID** foram adicionadas ao recurso [subscription](/graph/api/resources/subscription?view=graph-rest-beta). |
|Alteração|beta|A operação [list](/graph/api/subscription-list?view=graph-rest-beta) foi adicionada à entidade [subscription](/graph/api/resources/subscription?view=graph-rest-beta). |

### <a name="data-policy-operations"></a>Operações de Política de Dados

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | beta        | Foi adicionada a nova entidade [dataPolicyOperation](/graph/api/resources/datapolicyoperation?view=graph-rest-beta). Isso representa uma operação de política de dados enviados para fins de acompanhamento.
| Adição        | Beta        | Foi adicionada a ação [exportPersonalData](/graph/api/user-exportpersonaldata?view=graph-rest-beta) em [users](/graph/api/resources/users?view=graph-rest-beta). Essa ação envia uma solicitação de operação de política de dados para exportar dados pessoais armazenados pela Microsoft para um usuário. |

### <a name="directory-apis"></a>APIs de Diretório

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Adicionado o tipo complexo **onPremisesExtensionAttributes** à entidade [user](/graph/api/resources/user?view=graph-rest-beta) entity. Ele contém os atributos de extensão do AD locais, 1-15. |
| Adição        | Beta        | Adicionado o tipo complexo **privacyProfile** à entidade [organization](/graph/api/resources/organization?view=graph-rest-beta). |
| Adição        | v1.0        | Adicionado o suporte para a [restauração e a exclusão permanente de usuários e grupos](/graph/api/resources/directory?view=graph-rest-1.0). |

### <a name="excel-apis"></a>APIs do Excel

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
|Alteração|v1.0|A propriedade **legacyId** foi adicionada à entidade [tabela do Excel](/graph/api/resources/table?view=graph-rest-1.0). Isso inclui o identificador do valor numérico (tipo de dados String) que permanecerá constante para uma determinada tabela do Excel. Isso é fornecido como metadados adicionais se o aplicativo dependeu do identificador antigo usado em aplicativos cliente anteriores. Observação: a propriedade `id` e `legacyId` deve ser tratada como um valor de cadeia de caracteres opacas e não deve ser analisada para qualquer outro tipo no seu aplicativo. |

### <a name="group-lifecycle-policy"></a>Política de ciclo de vida do grupo

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Foi adicionado [groupLifecyclePolicy](/graph/api/resources/grouplifecyclepolicy?view=graph-rest-1.0). |
| Adição        | v1.0        | As seguintes APIs de política de ciclo de vida de grupo foram adicionadas: [Criar](/graph/api/grouplifecyclepolicy-post-grouplifecyclepolicies?view=graph-rest-1.0), [Listar](/graph/api/grouplifecyclepolicy-list?view=graph-rest-1.0), [Obter](/graph/api/grouplifecyclepolicy-get?view=graph-rest-1.0), [Atualizar](/graph/api/grouplifecyclepolicy-update?view=graph-rest-1.0), [Excluir](/graph/api/grouplifecyclepolicy-delete?view=graph-rest-1.0), [Adicionar grupo](/graph/api/grouplifecyclepolicy-addgroup?view=graph-rest-1.0), [Remover grupo](/graph/api/grouplifecyclepolicy-removegroup?view=graph-rest-1.0) |
| Adição        | v1.0        | Foi adicionada a função [List groupLifecyclePolicies](/graph/api/group-list-grouplifecyclepolicies?view=graph-rest-1.0) a [group](/graph/api/resources/group?view=graph-rest-1.0). |
| Alteração | v1.0 | A propriedade renewedDateTime e [renew](/graph/api/group-renew?view=graph-rest-1.0) foi adicionada ao [group](/graph/api/resources/group?view=graph-rest-1.0) |

### <a name="microsoft-intune-apis"></a>APIs do Microsoft Intune

|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|v1.0|Foram adicionadas novas entidades:<br/>[iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-1.0)<br/>[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-1.0)<br/>|
|Adição|v1.0|Foram adicionados novos tipos complexos:<br/>[appConfigurationSettingItem](/graph/api/resources/intune-apps-appconfigurationsettingitem?view=graph-rest-1.0)<br/>|
|Adição|v1.0|A ação [syncLicenses](/graph/api/intune-onboarding-vpptoken-synclicenses?view=graph-rest-1.0) foi adicionada a [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-1.0) |
|Adição|v1.0|A propriedade de navegação **vppTokens** foi adicionada à entidade [deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-1.0)|
|Adição|beta|A propriedade **managementCertificateExpirationDate** foi adicionada à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|Adição|beta|A propriedade **enhancedJailBreak** foi adicionada ao tipo complexo [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta)|
|Adição|beta|Foram adicionadas novas entidades:<br/>[androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta)<br/>[androidDeviceOwnerGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration?view=graph-rest-beta)<br/>[androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta)<br/>[androidManagedStoreAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidmanagedstoreappconfigurationschema?view=graph-rest-beta)<br/>[dataSharingConsent](/graph/api/resources/intune-devices-datasharingconsent?view=graph-rest-beta)<br/>[deviceConfigurationUserStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatesummary?view=graph-rest-beta)<br/>[macOSEndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-macosendpointprotectionconfiguration?view=graph-rest-beta)<br/>[macOSImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-macosimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[macOSLobApp](/graph/api/resources/intune-apps-macoslobapp?view=graph-rest-beta)<br/>[managedEBookCategory](/graph/api/resources/intune-books-managedebookcategory?view=graph-rest-beta)<br/>[microsoftStoreForBusinessContainedApp](/graph/api/resources/intune-apps-microsoftstoreforbusinesscontainedapp?view=graph-rest-beta)<br/>[mobileContainedApp](/graph/api/resources/intune-apps-mobilecontainedapp?view=graph-rest-beta)<br/>[windowsUniversalAppXContainedApp](/graph/api/resources/intune-apps-windowsuniversalappxcontainedapp?view=graph-rest-beta)<br/>|
|Adição|beta|Foram adicionados novos tipos complexos:<br/>[androidManagedStoreAppConfigurationSchemaItem](/graph/api/resources/intune-androidforwork-androidmanagedstoreappconfigurationschemaitem?view=graph-rest-beta)<br/>[deviceAndAppManagementData](/graph/api/resources/intune-onboarding-deviceandappmanagementdata?view=graph-rest-beta)<br/>[loggedOnUser](/graph/api/resources/intune-devices-loggedonuser?view=graph-rest-beta)<br/>[macOSFirewallApplication](/graph/api/resources/intune-deviceconfig-macosfirewallapplication?view=graph-rest-beta)<br/>[macOSLobChildApp](/graph/api/resources/intune-apps-macoslobchildapp?view=graph-rest-beta)<br/>[macOSMinimumOperatingSystem](/graph/api/resources/intune-apps-macosminimumoperatingsystem?view=graph-rest-beta)<br/>[windowsAppXAppAssignmentSettings](/graph/api/resources/intune-apps-windowsappxappassignmentsettings?view=graph-rest-beta)<br/>[windowsUniversalAppXAppAssignmentSettings](/graph/api/resources/intune-apps-windowsuniversalappxappassignmentsettings?view=graph-rest-beta)<br/>|
|Adição|beta|A ação [requestSignupUrl](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-requestsignupurl?view=graph-rest-beta) foi adicionada a [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) |
|Adição|beta|A ação [completeSignup](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-completesignup?view=graph-rest-beta) foi adicionada a [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) |
|Adição|beta|A ação [syncApps](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-syncapps?view=graph-rest-beta) foi adicionada a [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) |
|Adição|beta|A ação [unbind](/graph/api/intune-androidforwork-androidmanagedstoreaccountenterprisesettings-unbind?view=graph-rest-beta) foi adicionada a [androidManagedStoreAccountEnterpriseSettings](/graph/api/resources/intune-androidforwork-androidmanagedstoreaccountenterprisesettings?view=graph-rest-beta) |
|Adição|beta|A ação [revokeToken](/graph/api/intune-androidforwork-androiddeviceownerenrollmentprofile-revoketoken?view=graph-rest-beta) foi adicionada a [androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta) |
|Adição|beta|A ação [createToken](/graph/api/intune-androidforwork-androiddeviceownerenrollmentprofile-createtoken?view=graph-rest-beta) foi adicionada a [androidDeviceOwnerEnrollmentProfile](/graph/api/resources/intune-androidforwork-androiddeviceownerenrollmentprofile?view=graph-rest-beta) |
|Adição|beta|A ação [assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-beta) foi adicionada a [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) |
|Adição|beta|A ação [consentToDataSharing](/graph/api/intune-devices-datasharingconsent-consenttodatasharing?view=graph-rest-beta) foi adicionada a [dataSharingConsent](/graph/api/resources/intune-devices-datasharingconsent?view=graph-rest-beta) |
|Adição|beta|A função [getLoggedOnManagedDevices](/graph/api/intune-devices-user-getloggedonmanageddevices?view=graph-rest-beta) foi adicionada a [user](/graph/api/resources/intune-shared-user?view=graph-rest-beta) |
|Adição|beta|A função [exportDeviceAndAppManagementData](/graph/api/intune-onboarding-user-exportdeviceandappmanagementdata?view=graph-rest-beta) foi adicionada a [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) |
|Adição|beta|A função [exportDeviceAndAppManagementData](/graph/api/intune-onboarding-user-exportdeviceandappmanagementdata?view=graph-rest-beta) foi adicionada a [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) |
|Exclusão|beta|Foram removidas as seguintes entidades:<br/>**appleVolumePurchaseProgramToken**<br/>**mdmAppConfigGroupAssignment**<br/>**windows10KioskConfiguration**<br/>|
|Exclusão|beta|Remoção da ação [assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-beta) em [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) |
|Exclusão|beta|Remoção da ação [syncApps](/graph/api/intune-onboarding-applevolumepurchaseprogramtoken-syncapps?view=graph-rest-beta) em [appleVolumePurchaseProgramToken](/graph/api/resources/intune-onboarding-applevolumepurchaseprogramtoken?view=graph-rest-beta) |
|Adição|beta|A propriedade **workProfileBluetoothEnableContactSharing** foi adicionada à entidade [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade **intendedPurpose** foi adicionada à entidade [androidForWorkImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile?view=graph-rest-beta)|
|Adição|beta|A propriedade **intendedPurpose** foi adicionada à entidade [androidImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidimportedpfxcertificateprofile?view=graph-rest-beta)|
|Adição|beta|A propriedade **intendedPurpose** foi adicionada à entidade [iosImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-iosimportedpfxcertificateprofile?view=graph-rest-beta)|
|Adição|beta|A propriedade **encodedSettingXml** foi adicionada à entidade [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta)|
|Adição|beta|As propriedades **managedDeviceId** e **azureADDeviceId** foram adicionadas à entidade [managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-beta)|
|Adição|beta|A propriedade **usersLoggedOn** foi adicionada à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Exclusão|beta|Remoção da propriedade **lastLoggedOnUserId** da entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Adição|beta|A propriedade **lastModifiedDateTime** foi adicionada à entidade [managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-beta)|
|Adição|beta|A propriedade **isDependency** foi adicionada à entidade [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta)|
|Adição|beta|As propriedades **windowsEnabled**, **macEnabled**, **windowsDeviceBlockedOnMissingPartnerData** e **macDeviceBlockedOnMissingPartnerData** foram adicionadas à entidade [mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta)|
|Adição|beta|A propriedade **shouldUninstallOlderVersionsOfOffice** foi adicionada à entidade [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta)|
|Adição|beta|A propriedade **dataSharingConsentGranted** foi adicionada à entidade [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta)|
|Adição|beta|As propriedades **localSecurityOptionsBlockRemoteLogonWithBlankPassword**, **localSecurityOptionsAdministratorAccountName**, **localSecurityOptionsEnableGuestAccount**, **localSecurityOptionsGuestAccountName**, **localSecurityOptionsAllowUndockWithoutHavingToLogon**, **localSecurityOptionsBlockUsersInstallingPrinterDrivers**, **localSecurityOptionsBlockRemoteOpticalDriveAccess**, **localSecurityOptionsFormatAndEjectOfRemovableMediaAllowedUser**, **localSecurityOptionsMachineInactivityLimit**, **localSecurityOptionsDoNotRequireCtrlAltDel**, **localSecurityOptionsInformationDisplayedOnLockScreen**, **localSecurityOptionsHideLastSignedInUser**, **localSecurityOptionsHideUsernameAtSignIn**, **localSecurityOptionsLogOnMessageTitle**, **localSecurityOptionsLogOnMessageText**, **localSecurityOptionsAllowPKU2UAuthenticationRequests**, **localSecurityOptionsAllowRemoteCallsToSecurityAccountsManager**, **localSecurityOptionsClearVirtualMemoryPageFile**, **localSecurityOptionsAllowSystemToBeShutDownWithoutHavingToLogOn**, **localSecurityOptionsAllowUIAccessApplicationElevation**, **localSecurityOptionsVirtualizeFileAndRegistryWriteFailuresToPerUserLocations**, **localSecurityOptionsOnlyElevateSignedExecutables**, **localSecurityOptionsAdministratorElevationPromptBehavior**, **localSecurityOptionsStandardUserElevationPromptBehavior**, **localSecurityOptionsSwitchToSecureDesktopWhenPromptingForElevation**, **localSecurityOptionsDetectApplicationInstallationsAndPromptForElevation**, **localSecurityOptionsAllowUIAccessApplicationsForSecureLocations**, **localSecurityOptionsUseAdminApprovalMode**, **localSecurityOptionsUseAdminApprovalModeForAdministrators**, **deviceGuardLocalSystemAuthorityCredentialGuardSettings**, **deviceGuardEnableVirtualizationBasedSecurity** e **deviceGuardEnableSecureBootWithDMA** foram adicionadas à entidade [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Exclusão|beta|Remoção da propriedade **defenderPasswordProtectedEmailContentExecutionType** da entidade [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade **intendedPurpose** foi adicionada à entidade [windows10ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10importedpfxcertificateprofile?view=graph-rest-beta)|
|Exclusão|beta|Remoção das propriedades **printerNames**, **defaultPrinterName** e **blockAddingNewPrinter** da entidade [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade **certificateStore** foi adicionada à entidade [windows81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windows81scepcertificateprofile?view=graph-rest-beta)|
|Adição|beta|A propriedade **purchaseOrderIdentifier** foi adicionada à entidade [windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)|
|Alteração|beta|Foram alteradas as seguintes propriedades na entidade [windowsCertificateProfileBase](/graph/api/resources/intune-deviceconfig-windowscertificateprofilebase?view=graph-rest-beta):<br/>**subjectAlternativeNameType** de obrigatória para opcional<br/>|
|Adição|beta|As propriedades **advancedThreatProtectionOnboardingFilename** e **advancedThreatProtectionOffboardingFilename** foram adicionadas à entidade [windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade **intendedPurpose** foi adicionada à entidade [windowsPhone81ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile?view=graph-rest-beta)|
|Adição|beta|As propriedades **skipChecksBeforeRestart** e **updateWeeks** foram adicionadas à entidade [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade de navegação **managedEBookCategories** foi adicionada à entidade [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta)|
|Adição|beta|As propriedades de navegação **androidManagedStoreAccountEnterpriseSettings**, **androidManagedStoreAppConfigurationSchemas**, **androidDeviceOwnerEnrollmentProfiles**, **dataSharingConsents** e **deviceConfigurationUserStateSummaries** foram adicionadas à entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta)|
|Exclusão|beta|Remoção da propriedade de navegação **deviceSetupConfigurations** da entidade [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Exclusão|beta|Remoção da propriedade de navegação **groupAssignments** da entidade [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta)|
|Adição|beta|A propriedade de navegação **categories** foi adicionada à entidade [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta)|
|Adição|beta|A propriedade de navegação **containedApps** foi adicionada à entidade [microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-beta)|
|Adição|beta|A propriedade de navegação **containedApps** foi adicionada à entidade [mobileAppContent](/graph/api/resources/intune-apps-mobileappcontent?view=graph-rest-beta)|
|Adição|beta|Foi adicionada a propriedade de navegação **committedContainedApps** à entidade [windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta)|

### <a name="onedrive"></a>OneDrive
|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|v1.0|Foram adicionadas novas entidades:<br/>[baseItemVersion](/graph/api/resources/baseitemversion?view=graph-rest-1.0)<br/>[driveItemVersion](/graph/api/resources/driveitemversion?view=graph-rest-1.0)<br/>[listItemVersion](/graph/api/resources/listitemversion?view=graph-rest-1.0)<br/> |
|Adição|v1.0|Foram adicionados novos tipos complexos:<br/>[publicationFacet](/graph/api/resources/publicationfacet?view=graph-rest-1.0)<br/> |
|Adição|v1.0|Foi adicionada a propriedade <b>publication</b> à entidade [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) |
|Adição|v1.0|Foi adicionada a propriedade de navegação <b>versions</b> à entidade [driveItem](/graph/api/resources/driveitem?view=graph-rest-1.0) |
|Adição|v1.0|Foi adicionada a propriedade de navegação <b>versions</b> à entidade [listItem](/graph/api/resources/listitem?view=graph-rest-1.0) |
|Adição|v1.0|Foi adicionada a propriedade <b>root</b> à entidade [siteCollection](/graph/api/resources/sitecollection?view=graph-rest-1.0) |
|Adição|v1.0|Foi adicionada a ação [restoreVersion](/graph/api/driveitemversion-restore?view=graph-rest-1.0) à entidade [driveItemVersion](/graph/api/resources/driveitemversion?view=graph-rest-1.0) |
|Adição|v1.0|Foi adicionada a ação [restoreVersion](/graph/api/listitemversion-restore?view=graph-rest-1.0) à entidade [listItemVersion](/graph/api/resources/listitemversion?view=graph-rest-1.0) |


### <a name="onedrive"></a>OneDrive
|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|Beta|Foi adicionado um novo tipo complexo:<br/>[itemPreviewInfo](/graph/api/resources/itempreviewinfo?view=graph-rest-beta)<br/> |
|Adição|Beta|A propriedade <b>name</b> foi adicionada ao tipo complexo [contentTypeInfo](/graph/api/resources/contenttypeinfo?view=graph-rest-beta) |
|Adição|Beta|Foi adicionada a propriedade <b>objectType</b> ao tipo complexo [deleteAction](/graph/api/resources/deleteaction?view=graph-rest-beta) |
|Adição|Beta|Foi adicionada a propriedade <b>newName</b> ao tipo complexo [renameAction](/graph/api/resources/renameaction?view=graph-rest-beta) |
|Adição|Beta|Foi adicionada a propriedade <b>tenantId</b> ao tipo complexo [sharepointIds](/graph/api/resources/renameaction?view=graph-rest-beta) |
|Adição|Beta|Foi adicionada a propriedade <b>lastRecordedDateTime</b> ao tipo complexo [itemActivityTimeSet](/graph/api/resources/itemactivitytimeset?view=graph-rest-beta) |
|Adição|Beta|A ação [preview](/graph/api/driveitem-preview?view=graph-rest-beta) foi adicionada à entidade [driveItem](/graph/api/resources/driveitem?view=graph-rest-beta) |

### <a name="reports-apis"></a>APIs de relatórios

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
|Adição|beta|A propriedade **SiteId** foi adicionada à entidade [sharePointSiteUsageDetail](/graph/api/resources/sharepointsiteusagedetail?view=graph-rest-beta).|

### <a name="terms-of-use"></a>Termos de uso

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Os recursos [agreement](/graph/api/resources/agreement?view=graph-rest-beta) e [agreementAcceptance](/graph/api/resources/agreementacceptance?view=graph-rest-beta) foram adicionados. |
| Adição        | Beta        | As seguintes APIs para [agreement](/graph/api/resources/agreement?view=graph-rest-beta) foram adicionadas: [Criar](/graph/api/greement-post-agreements?view=graph-rest-beta), [Listar](/graph/api/agreement-list?view=graph-rest-beta), [Obter](/graph/api/agreement-get?view=graph-rest-beta), [Atualizar](/graph/api/agreement-update?view=graph-rest-beta), [Excluir](/graph/api/agreement-delete?view=graph-rest-beta). |
| Adição        | Beta        | Os relacionamentos [agreementAcceptance](/graph/api/resources/agreementacceptance?view=graph-rest-beta) foram adicionados ao recurso [user](/graph/api/resources/user?view=graph-rest-beta). |

## <a name="february-2018"></a>Fevereiro de 2018

### <a name="microsoft-intune-apis"></a>APIs do Microsoft Intune
|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|beta|Foram adicionadas novas entidades:<br/>[androidForWorkImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[androidImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-androidimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[importedWindowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentity?view=graph-rest-beta)<br/>[iosImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-iosimportedpfxcertificateprofile?view=graph-rest-beta)<br/>[windows10ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10importedpfxcertificateprofile?view=graph-rest-beta)<br/>[windows10KioskConfiguration](/graph/api/resources/intune-deviceconfig-windows10kioskconfiguration?view=graph-rest-beta)<br/>[windowsPhone81ImportedPFXCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81importedpfxcertificateprofile?view=graph-rest-beta)<br/>|
|Adição|beta|Foram adicionados novos tipos complexos:<br/>[importedWindowsAutopilotDeviceIdentityState](/graph/api/resources/intune-enrollment-importedwindowsautopilotdeviceidentitystate?view=graph-rest-beta)<br/>|
|Adição|beta|A função [managedDeviceEnrollmentFailureDetails](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuredetails?view=graph-rest-beta) foi adicionada ao [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) |
|Adição|beta|A função [managedDeviceEnrollmentFailureDetails](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuredetails?view=graph-rest-beta) foi adicionada ao [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) |
|Adição|beta|A função [managedDeviceEnrollmentFailureTrends](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmentfailuretrends?view=graph-rest-beta) foi adicionada ao [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) |
|Adição|beta|A função [managedDeviceEnrollmentTopFailures](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmenttopfailures?view=graph-rest-beta) foi adicionada ao [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) |
|Adição|beta|A função [managedDeviceEnrollmentTopFailures](/graph/api/intune-troubleshooting-reportroot-manageddeviceenrollmenttopfailures?view=graph-rest-beta) foi adicionada ao [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) |
|Alteração|beta|Foram removidas as propriedades **requireAppVerify**, **requireSafetyNetAttestationBasicIntegrity**, **requireSafetyNetAttestationCertifiedDevice**, **requireGooglePlayServices**, **requireUpToDateSecurityProviders** e **requireCompanyPortalAppIntegrity** da entidade [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta)|
|Alteração|beta|Foram removidas as propriedades **requireAppVerify**, **requireSafetyNetAttestationBasicIntegrity**, **requireSafetyNetAttestationCertifiedDevice**, **requireGooglePlayServices**, **requireUpToDateSecurityProviders** e **requireCompanyPortalAppIntegrity** da entidade [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta)|
|Alteração|beta|Foram removidas as propriedades **name**, **modifiedDateTime**, **totalEnrollmentCount** e **qrCode** da entidade [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta)|
|Alteração|beta|Foram removidas as propriedades **nonEapAuthenticationMethodForEapTtls**, **nonEapAuthenticationMethodForPeap** e **enableOuterIdentityPrivacy** da entidade [androidForWorkEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkenterprisewificonfiguration?view=graph-rest-beta)|
|Alteração|beta|A propriedade **workProfileBlockAddingAccounts** foi adicionada à entidade [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta)|
|Alteração|beta|Foram removidas as propriedades **blockCrossProfileCopyPaste** e **requireAppVerify** da entidade [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta)|
|Alteração|beta|A propriedade **deviceOwnerManagementEnabled** foi adicionada à entidade [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta)|
|Alteração|beta|Foi removida a propriedade **requireAppVerify** da entidade [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta)|
|Alteração|beta|A propriedade **exemptedAppPackages** foi adicionada à entidade [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta)|
|Alteração|beta|Foram adicionadas as propriedades **exemptedAppProtocols** e **exemptedAppPackages** à entidade [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)|
|Alteração|beta|A propriedade **exemptedAppProtocols** foi adicionada à entidade [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta)|
|Alteração|beta|A propriedade **lastLoggedOnUserId** foi adicionada à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Alteração|beta|A propriedade **isFrameworkFile** foi adicionada à entidade [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta)|
|Alteração|beta|A propriedade **targetedAppManagementLevels** foi adicionada à entidade [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta)|
|Alteração|beta|Foram adicionadas as propriedades **localSecurityOptionsBlockMicrosoftAccounts**, **localSecurityOptionsEnableAdministratorAccount**, **defenderPreventCredentialStealingType**, **defenderProcessCreationType**, **defenderUntrustedUSBProcessType**, **defenderUntrustedExecutableType**, **defenderPasswordProtectedEmailContentExecutionType**, **defenderAdvancedRansomewareProtectionType** e **applicationGuardAllowFileSaveOnHost** à entidade [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Alteração|beta|Foram adicionadas as propriedades **edgeFavoritesListLocation** e **edgeBlockEditFavorites** à entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Alteração|beta|Foram adicionadas as propriedades **printerNames**, **defaultPrinterName** e **blockAddingNewPrinter** à entidade [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta)|
|Alteração|beta|A propriedade de navegação **importedWindowsAutopilotDeviceIdentities** foi adicionada à entidade [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Alteração|beta|A propriedade **shareAPNSData** foi adicionada à entidade [adminConsent](/graph/api/resources/intune-devices-adminconsent?view=graph-rest-beta)|
|Alteração|beta|Foi removida a propriedade **collectFullIOSAppInventory** da entidade [adminConsent](/graph/api/resources/intune-devices-adminconsent?view=graph-rest-beta)|
|Alteração|beta|Foi removida a propriedade **deviceUsageType** do tipo complexo [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta)|


### <a name="planner-apis"></a>APIs do Planner

|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|Beta|Foram adicionados novos tipos complexos:<br/>[plannerPlanContext](/graph/api/resources/plannerplancontext?view=graph-rest-beta)<br/>[plannerPlanContextDetails](/graph/api/resources/plannerplancontextdetails?view=graph-rest-beta)<br/>[plannerPlanContextCollection](/graph/api/resources/plannerplancontextcollection?view=graph-rest-beta)<br/>[plannerPlanContextDetailsCollection](/graph/api/resources/plannerplancontextdetailscollection?view=graph-rest-beta)<br/>[plannerFavoritePlanReference](/graph/api/resources/plannerfavoriteplanreference?view=graph-rest-beta)<br/>[plannerRecentPlanReference](/graph/api/resources/plannerrecentplanreference?view=graph-rest-beta)<br/>[plannerFavoritePlanReferenceCollection](/graph/api/resources/plannerfavoriteplanreferencecollection?view=graph-rest-beta)<br/>[plannerRecentPlanReferenceCollection](/graph/api/resources/plannerrecentplanreferencecollection?view=graph-rest-beta)|
|Adição|Beta|As propriedades `favoritePlanReferences` e `recentPlanReferences` foram adicionadas à entidade [plannerUser](/graph/api/resources/planneruser?view=graph-rest-beta). |
|Adição|Beta|As propriedades de navegação `favoritePlans` e `recentPlans` foram adicionadas à entidade [plannerUser](/graph/api/resources/planneruser?view=graph-rest-beta). |
|Adição|Beta|A propriedade `contexts` foi adicionada à entidade [plannerPlan](/graph/api/resources/plannerplan?view=graph-rest-beta). |
|Adição|Beta|Foi adicionada propriedade `contextDetails` à entidade [plannerPlanDetails](/graph/api/resources/plannerplandetails?view=graph-rest-beta). |
|Adição|Beta|Foi adicionada a [consulta delta](/graph/api/planneruser-list-delta?view=graph-rest-beta) ao Planner |

### <a name="reports-apis"></a>APIs de relatórios
| Tipo de alteração | Versão | Descrição                              |
|:------------|:--------|:-----------------------------------------|
| Adição    | Beta    | A propriedade **activatedOnSharedComputer** foi adicionada à entidade [userActivationCounts](/graph/api/resources/useractivationcounts?view=graph-rest-beta).|
| Adição    | Beta    | A propriedade **sharedComputerActivation** foi adicionada à entidade [office365ActivationsUserCounts](/graph/api/resources/office365activationsusercounts?view=graph-rest-beta).|

## <a name="january-2018"></a>Janeiro de 2018

### <a name="education-apis"></a>APIs de educação

|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|Beta|Propriedades de navegação adicionais e o suporte para a filtragem foram adicionados à [API da lista de participação](/graph/api/resources/education-overview?view=graph-rest-beta).|

### <a name="json-batching"></a>Envio em lote JSON

|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|v1.0|O suporte a [processamento em lotes JSON](json-batching.md) foi adicionado. Limite interno de solicitações definido como 20.|
|Alteração|Beta|O limite interno de solicitações do [envio em lotes JSON](json-batching.md) foi aumentado de 5 para 20.|

### <a name="microsoft-intune-apis"></a>APIs do Microsoft Intune
|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|v1.0|Foram adicionadas novas entidades:<br/>[androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-1.0)<br/>[androidCustomConfiguration](/graph/api/resources/intune-deviceconfig-androidcustomconfiguration?view=graph-rest-1.0)<br/>[androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-1.0)<br/>[androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-1.0)<br/>[androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-1.0)<br/>[androidManagedAppRegistration](/graph/api/resources/intune-mam-androidmanagedappregistration?view=graph-rest-1.0)<br/>[androidStoreApp](/graph/api/resources/intune-apps-androidstoreapp?view=graph-rest-1.0)<br/>[appleDeviceFeaturesConfigurationBase](/graph/api/resources/intune-deviceconfig-appledevicefeaturesconfigurationbase?view=graph-rest-1.0)<br/>[applePushNotificationCertificate](/graph/api/resources/intune-devices-applepushnotificationcertificate?view=graph-rest-1.0)<br/>[defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-1.0)<br/>[detectedApp](/graph/api/resources/intune-devices-detectedapp?view=graph-rest-1.0)<br/>[deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-1.0)<br/>[deviceAndAppManagementRoleDefinition](/graph/api/resources/intune-rbac-deviceandappmanagementroledefinition?view=graph-rest-1.0)<br/>[deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-1.0)<br/>[deviceCategory](/graph/api/resources/intune-shared-devicecategory?view=graph-rest-1.0)<br/>[deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-1.0)<br/>[deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-1.0)<br/>[deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-1.0)<br/>[deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-1.0)<br/>[deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-1.0)<br/>[deviceCompliancePolicyDeviceStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary?view=graph-rest-1.0)<br/>[deviceCompliancePolicySettingStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary?view=graph-rest-1.0)<br/>[deviceCompliancePolicyState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicystate?view=graph-rest-1.0)<br/>[deviceComplianceScheduledActionForRule](/graph/api/resources/intune-deviceconfig-devicecompliancescheduledactionforrule?view=graph-rest-1.0)<br/>[deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-1.0)<br/>[deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-1.0)<br/>[deviceComplianceUserStatus](/graph/api/resources/intune-deviceconfig-devicecomplianceuserstatus?view=graph-rest-1.0)<br/>[deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0)<br/>[deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment?view=graph-rest-1.0)<br/>[deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-1.0)<br/>[deviceConfigurationDeviceStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatesummary?view=graph-rest-1.0)<br/>[deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-1.0)<br/>[deviceConfigurationState](/graph/api/resources/intune-deviceconfig-deviceconfigurationstate?view=graph-rest-1.0)<br/>[deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-1.0)<br/>[deviceConfigurationUserStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatus?view=graph-rest-1.0)<br/>[deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-1.0)<br/>[deviceEnrollmentLimitConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentlimitconfiguration?view=graph-rest-1.0)<br/>[deviceEnrollmentPlatformRestrictionsConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration?view=graph-rest-1.0)<br/>[deviceEnrollmentWindowsHelloForBusinessConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration?view=graph-rest-1.0)<br/>[deviceInstallState](/graph/api/resources/intune-books-deviceinstallstate?view=graph-rest-1.0)<br/>[deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-1.0)<br/>[deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-1.0)<br/>[deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-1.0)<br/>[deviceManagementTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingevent?view=graph-rest-1.0)<br/>[eBookInstallSummary](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-1.0)<br/>[editionUpgradeConfiguration](/graph/api/resources/intune-deviceconfig-editionupgradeconfiguration?view=graph-rest-1.0)<br/>[enrollmentConfigurationAssignment](/graph/api/resources/intune-onboarding-enrollmentconfigurationassignment?view=graph-rest-1.0)<br/>[enrollmentTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-enrollmenttroubleshootingevent?view=graph-rest-1.0)<br/>[iosCertificateProfile](/graph/api/resources/intune-deviceconfig-ioscertificateprofile?view=graph-rest-1.0)<br/>[iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-1.0)<br/>[iosCustomConfiguration](/graph/api/resources/intune-deviceconfig-ioscustomconfiguration?view=graph-rest-1.0)<br/>[iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-1.0)<br/>[iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-1.0)<br/>[iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-1.0)<br/>[iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-1.0)<br/>[iosManagedAppRegistration](/graph/api/resources/intune-mam-iosmanagedappregistration?view=graph-rest-1.0)<br/>[iosStoreApp](/graph/api/resources/intune-apps-iosstoreapp?view=graph-rest-1.0)<br/>[iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-1.0)<br/>[iosUpdateDeviceStatus](/graph/api/resources/intune-deviceconfig-iosupdatedevicestatus?view=graph-rest-1.0)<br/>[iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-1.0)<br/>[iosVppEBook](/graph/api/resources/intune-books-iosvppebook?view=graph-rest-1.0)<br/>[iosVppEBookAssignment](/graph/api/resources/intune-books-iosvppebookassignment?view=graph-rest-1.0)<br/>[localizedNotificationMessage](/graph/api/resources/intune-notification-localizednotificationmessage?view=graph-rest-1.0)<br/>[macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-1.0)<br/>[macOSCustomConfiguration](/graph/api/resources/intune-deviceconfig-macoscustomconfiguration?view=graph-rest-1.0)<br/>[macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration?view=graph-rest-1.0)<br/>[macOSGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-macosgeneraldeviceconfiguration?view=graph-rest-1.0)<br/>[macOSOfficeSuiteApp](/graph/api/resources/intune-apps-macosofficesuiteapp?view=graph-rest-1.0)<br/>[managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-1.0)<br/>[managedAndroidStoreApp](/graph/api/resources/intune-apps-managedandroidstoreapp?view=graph-rest-1.0)<br/>[managedApp](/graph/api/resources/intune-apps-managedapp?view=graph-rest-1.0)<br/>[managedAppConfiguration](/graph/api/resources/intune-mam-managedappconfiguration?view=graph-rest-1.0)<br/>[managedAppOperation](/graph/api/resources/intune-mam-managedappoperation?view=graph-rest-1.0)<br/>[managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-1.0)<br/>[managedAppPolicyDeploymentSummary](/graph/api/resources/intune-mam-managedapppolicydeploymentsummary?view=graph-rest-1.0)<br/>[managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-1.0)<br/>[managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-1.0)<br/>[managedAppStatus](/graph/api/resources/intune-mam-managedappstatus?view=graph-rest-1.0)<br/>[managedAppStatusRaw](/graph/api/resources/intune-mam-managedappstatusraw?view=graph-rest-1.0)<br/>[managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfigurationAssignment](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationassignment?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfigurationUserStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationuserstatus?view=graph-rest-1.0)<br/>[managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-1.0)<br/>[managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-1.0)<br/>[managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-1.0)<br/>[managedEBookAssignment](/graph/api/resources/intune-books-managedebookassignment?view=graph-rest-1.0)<br/>[managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-1.0)<br/>[managedIOSStoreApp](/graph/api/resources/intune-apps-managediosstoreapp?view=graph-rest-1.0)<br/>[managedMobileApp](/graph/api/resources/intune-mam-managedmobileapp?view=graph-rest-1.0)<br/>[managedMobileLobApp](/graph/api/resources/intune-apps-managedmobilelobapp?view=graph-rest-1.0)<br/>[mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam?view=graph-rest-1.0mwindowsinformationprotectionpolicy)<br/>[microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-1.0)<br/>[mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0)<br/>[mobileAppAssignment](/graph/api/resources/intune-apps-mobileappassignment?view=graph-rest-1.0)<br/>[mobileAppCategory](/graph/api/resources/intune-apps-mobileappcategory?view=graph-rest-1.0)<br/>[mobileAppContent](/graph/api/resources/intune-apps-mobileappcontent?view=graph-rest-1.0)<br/>[mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-1.0)<br/>[mobileLobApp](/graph/api/resources/intune-apps-mobilelobapp?view=graph-rest-1.0)<br/>[mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-1.0)<br/>[notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-1.0)<br/>[onPremisesConditionalAccessSettings](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-1.0)<br/>[remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-1.0)<br/>[resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-1.0)<br/>[roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-1.0)<br/>[roleDefinition](/graph/api/resources/intune-rbac-roledefinition?view=graph-rest-1.0)<br/>[settingStateDeviceSummary](/graph/api/resources/intune-deviceconfig-settingstatedevicesummary?view=graph-rest-1.0)<br/>[sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-1.0)<br/>[softwareUpdateStatusSummary](/graph/api/resources/intune-deviceconfig-softwareupdatestatussummary?view=graph-rest-1.0)<br/>[targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-1.0)<br/>targetedManagedAppPolicyAssignment<br/>[targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-1.0)<br/>[telecomExpenseManagementPartner](/graph/api/resources/intune-tem-telecomexpensemanagementpartner?view=graph-rest-1.0)<br/>[termsAndConditions](/graph/api/resources/intune-companyterms-termsandconditions?view=graph-rest-1.0)<br/>[termsAndConditionsAcceptanceStatus](/graph/api/resources/intune-companyterms-termsandconditionsacceptancestatus?view=graph-rest-1.0)<br/>[termsAndConditionsAssignment](/graph/api/resources/intune-companyterms-termsandconditionsassignment?view=graph-rest-1.0)<br/>[userInstallStateSummary](/graph/api/resources/intune-books-userinstallstatesummary?view=graph-rest-1.0)<br/>[webApp](/graph/api/resources/intune-apps-webapp?view=graph-rest-1.0)<br/>[windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-1.0)<br/>[windows10CustomConfiguration](/graph/api/resources/intune-deviceconfig-windows10customconfiguration?view=graph-rest-1.0)<br/>[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-1.0)<br/>[windows10EnterpriseModernAppManagementConfiguration](/graph/api/resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration?view=graph-rest-1.0)<br/>[windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-1.0)<br/>[windows10MobileCompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10mobilecompliancepolicy?view=graph-rest-1.0)<br/>[windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-1.0)<br/>[windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-1.0)<br/>[windows81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows81compliancepolicy?view=graph-rest-1.0)<br/>[windows81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows81generalconfiguration?view=graph-rest-1.0)<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-1.0)<br/>[windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-1.0)<br/>[windowsInformationProtectionAppLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionapplearningsummary?view=graph-rest-1.0)<br/>[windowsInformationProtectionAppLockerFile](/graph/api/resources/intune-mam-windowsinformationprotectionapplockerfile?view=graph-rest-1.0)<br/>[windowsInformationProtectionNetworkLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionnetworklearningsummary?view=graph-rest-1.0)<br/>[windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-1.0)<br/>[windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-1.0)<br/>[windowsPhone81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windowsphone81compliancepolicy?view=graph-rest-1.0)<br/>[windowsPhone81CustomConfiguration](/graph/api/resources/intune-deviceconfig-windowsphone81customconfiguration?view=graph-rest-1.0)<br/>[windowsPhone81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windowsphone81generalconfiguration?view=graph-rest-1.0)<br/>[windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-1.0)<br/>[windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-1.0)<br/>|
|Adição|v1.0|Foram adicionados novos tipos complexos:<br/>[allDevicesAssignmentTarget](/graph/api/resources/intune-shared-alldevicesassignmenttarget?view=graph-rest-1.0)<br/>[allLicensedUsersAssignmentTarget](/graph/api/resources/intune-shared-alllicensedusersassignmenttarget?view=graph-rest-1.0)<br/>[androidMinimumOperatingSystem](/graph/api/resources/intune-apps-androidminimumoperatingsystem?view=graph-rest-1.0)<br/>[androidMobileAppIdentifier](/graph/api/resources/intune-mam-androidmobileappidentifier?view=graph-rest-1.0)<br/>[appListItem](/graph/api/resources/intune-deviceconfig-applistitem?view=graph-rest-1.0)<br/>[bitLockerRemovableDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockerremovabledrivepolicy?view=graph-rest-1.0)<br/>[configurationManagerClientEnabledFeatures](/graph/api/resources/intune-devices-configurationmanagerclientenabledfeatures?view=graph-rest-1.0)<br/>[defenderDetectedMalwareActions](/graph/api/resources/intune-deviceconfig-defenderdetectedmalwareactions?view=graph-rest-1.0)<br/>[deleteUserFromSharedAppleDeviceActionResult](/graph/api/resources/intune-devices-deleteuserfromsharedappledeviceactionresult?view=graph-rest-1.0)<br/>[deviceActionResult](/graph/api/resources/intune-devices-deviceactionresult?view=graph-rest-1.0)<br/>[deviceAndAppManagementAssignmentTarget](/graph/api/resources/intune-shared-deviceandappmanagementassignmenttarget?view=graph-rest-1.0)<br/>[deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-1.0)<br/>[deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-1.0)<br/>[deviceEnrollmentPlatformRestriction](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestriction?view=graph-rest-1.0)<br/>[deviceExchangeAccessStateSummary](/graph/api/resources/intune-devices-deviceexchangeaccessstatesummary?view=graph-rest-1.0)<br/>[deviceGeoLocation](/graph/api/resources/intune-devices-devicegeolocation?view=graph-rest-1.0)<br/>[deviceHealthAttestationState](/graph/api/resources/intune-devices-devicehealthattestationstate?view=graph-rest-1.0)<br/>[deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-1.0)<br/>[deviceOperatingSystemSummary](/graph/api/resources/intune-devices-deviceoperatingsystemsummary?view=graph-rest-1.0)<br/>[edgeSearchEngine](/graph/api/resources/intune-deviceconfig-edgesearchengine?view=graph-rest-1.0)<br/>[edgeSearchEngineBase](/graph/api/resources/intune-deviceconfig-edgesearchenginebase?view=graph-rest-1.0)<br/>[edgeSearchEngineCustom](/graph/api/resources/intune-deviceconfig-edgesearchenginecustom?view=graph-rest-1.0)<br/>[exclusionGroupAssignmentTarget](/graph/api/resources/intune-shared-exclusiongroupassignmenttarget?view=graph-rest-1.0)<br/>[fileEncryptionInfo](/graph/api/resources/intune-apps-fileencryptioninfo?view=graph-rest-1.0)<br/>[groupAssignmentTarget](/graph/api/resources/intune-shared-groupassignmenttarget?view=graph-rest-1.0)<br/>[intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-1.0)<br/>[iosDeviceType](/graph/api/resources/intune-apps-iosdevicetype?view=graph-rest-1.0)<br/>[iosHomeScreenApp](/graph/api/resources/intune-deviceconfig-ioshomescreenapp?view=graph-rest-1.0)<br/>[iosHomeScreenFolder](/graph/api/resources/intune-deviceconfig-ioshomescreenfolder?view=graph-rest-1.0)<br/>[iosHomeScreenFolderPage](/graph/api/resources/intune-deviceconfig-ioshomescreenfolderpage?view=graph-rest-1.0)<br/>[iosHomeScreenItem](/graph/api/resources/intune-deviceconfig-ioshomescreenitem?view=graph-rest-1.0)<br/>[iosHomeScreenPage](/graph/api/resources/intune-deviceconfig-ioshomescreenpage?view=graph-rest-1.0)<br/>[iosLobAppAssignmentSettings](/graph/api/resources/intune-apps-ioslobappassignmentsettings?view=graph-rest-1.0)<br/>[iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-1.0)<br/>[iosMobileAppIdentifier](/graph/api/resources/intune-mam-iosmobileappidentifier?view=graph-rest-1.0)<br/>[iosNetworkUsageRule](/graph/api/resources/intune-deviceconfig-iosnetworkusagerule?view=graph-rest-1.0)<br/>[iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-1.0)<br/>[iosStoreAppAssignmentSettings](/graph/api/resources/intune-apps-iosstoreappassignmentsettings?view=graph-rest-1.0)<br/>[iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-1.0)<br/>[ipRange](/graph/api/resources/intune-mam-iprange?view=graph-rest-1.0)<br/>[iPv4Range](/graph/api/resources/intune-mam-ipv4range?view=graph-rest-1.0)<br/>[iPv6Range](/graph/api/resources/intune-mam-ipv6range?view=graph-rest-1.0)<br/>[keyValuePair](/graph/api/resources/intune-androidforwork-keyvaluepair?view=graph-rest-1.0)<br/>[locateDeviceActionResult](/graph/api/resources/intune-devices-locatedeviceactionresult?view=graph-rest-1.0)<br/>[managedAppDiagnosticStatus](/graph/api/resources/intune-mam-managedappdiagnosticstatus?view=graph-rest-1.0)<br/>[managedAppPolicyDeploymentSummaryPerApp](/graph/api/resources/intune-mam-managedapppolicydeploymentsummaryperapp?view=graph-rest-1.0)<br/>[mediaContentRatingAustralia](/graph/api/resources/intune-deviceconfig-mediacontentratingaustralia?view=graph-rest-1.0)<br/>[mediaContentRatingCanada](/graph/api/resources/intune-deviceconfig-mediacontentratingcanada?view=graph-rest-1.0)<br/>[mediaContentRatingFrance](/graph/api/resources/intune-deviceconfig-mediacontentratingfrance?view=graph-rest-1.0)<br/>[mediaContentRatingGermany](/graph/api/resources/intune-deviceconfig-mediacontentratinggermany?view=graph-rest-1.0)<br/>[mediaContentRatingIreland](/graph/api/resources/intune-deviceconfig-mediacontentratingireland?view=graph-rest-1.0)<br/>[mediaContentRatingJapan](/graph/api/resources/intune-deviceconfig-mediacontentratingjapan?view=graph-rest-1.0)<br/>[mediaContentRatingNewZealand](/graph/api/resources/intune-deviceconfig-mediacontentratingnewzealand?view=graph-rest-1.0)<br/>[mediaContentRatingUnitedKingdom](/graph/api/resources/intune-deviceconfig-mediacontentratingunitedkingdom?view=graph-rest-1.0)<br/>[mediaContentRatingUnitedStates](/graph/api/resources/intune-deviceconfig-mediacontentratingunitedstates?view=graph-rest-1.0)<br/>[microsoftStoreForBusinessAppAssignmentSettings](/graph/api/resources/intune-apps-microsoftstoreforbusinessappassignmentsettings?view=graph-rest-1.0)<br/>[mimeContent](/graph/api/resources/intune-shared-mimecontent?view=graph-rest-1.0)<br/>[mobileAppAssignmentSettings](/graph/api/resources/intune-apps-mobileappassignmentsettings?view=graph-rest-1.0)<br/>[mobileAppIdentifier](/graph/api/resources/intune-mam-mobileappidentifier?view=graph-rest-1.0)<br/>[omaSetting](/graph/api/resources/intune-deviceconfig-omasetting?view=graph-rest-1.0)<br/>[omaSettingBase64](/graph/api/resources/intune-deviceconfig-omasettingbase64?view=graph-rest-1.0)<br/>[omaSettingBoolean](/graph/api/resources/intune-deviceconfig-omasettingboolean?view=graph-rest-1.0)<br/>[omaSettingDateTime](/graph/api/resources/intune-deviceconfig-omasettingdatetime?view=graph-rest-1.0)<br/>[omaSettingFloatingPoint](/graph/api/resources/intune-deviceconfig-omasettingfloatingpoint?view=graph-rest-1.0)<br/>[omaSettingInteger](/graph/api/resources/intune-deviceconfig-omasettinginteger?view=graph-rest-1.0)<br/>[omaSettingString](/graph/api/resources/intune-deviceconfig-omasettingstring?view=graph-rest-1.0)<br/>[omaSettingStringXml](/graph/api/resources/intune-deviceconfig-omasettingstringxml?view=graph-rest-1.0)<br/>[proxiedDomain](/graph/api/resources/intune-mam-proxieddomain?view=graph-rest-1.0)<br/>[remoteLockActionResult](/graph/api/resources/intune-devices-remotelockactionresult?view=graph-rest-1.0)<br/>[resetPasscodeActionResult](/graph/api/resources/intune-devices-resetpasscodeactionresult?view=graph-rest-1.0)<br/>[resourceAction](/graph/api/resources/intune-rbac-resourceaction?view=graph-rest-1.0)<br/>[rgbColor](/graph/api/resources/intune-onboarding-rgbcolor?view=graph-rest-1.0)<br/>[rolePermission](/graph/api/resources/intune-rbac-rolepermission?view=graph-rest-1.0)<br/>[settingSource](/graph/api/resources/intune-deviceconfig-settingsource?view=graph-rest-1.0)<br/>[sharedPCAccountManagerPolicy](/graph/api/resources/intune-deviceconfig-sharedpcaccountmanagerpolicy?view=graph-rest-1.0)<br/>[updateWindowsDeviceAccountActionParameter](/graph/api/resources/intune-devices-updatewindowsdeviceaccountactionparameter?view=graph-rest-1.0)<br/>[vppLicensingType](/graph/api/resources/intune-apps-vpplicensingtype?view=graph-rest-1.0)<br/>[windows10NetworkProxyServer](/graph/api/resources/intune-deviceconfig-windows10networkproxyserver?view=graph-rest-1.0)<br/>[windowsDefenderScanActionResult](/graph/api/resources/intune-devices-windowsdefenderscanactionresult?view=graph-rest-1.0)<br/>[windowsDeviceAccount](/graph/api/resources/intune-devices-windowsdeviceaccount?view=graph-rest-1.0)<br/>[windowsDeviceADAccount](/graph/api/resources/intune-devices-windowsdeviceadaccount?view=graph-rest-1.0)<br/>[windowsDeviceAzureADAccount](/graph/api/resources/intune-devices-windowsdeviceazureadaccount?view=graph-rest-1.0)<br/>[windowsFirewallNetworkProfile](/graph/api/resources/intune-deviceconfig-windowsfirewallnetworkprofile?view=graph-rest-1.0)<br/>[windowsInformationProtectionApp](/graph/api/resources/intune-mam-windowsinformationprotectionapp?view=graph-rest-1.0)<br/>[windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-mam-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-1.0)<br/>[windowsInformationProtectionDesktopApp](/graph/api/resources/intune-mam-windowsinformationprotectiondesktopapp?view=graph-rest-1.0)<br/>[windowsInformationProtectionIPRangeCollection](/graph/api/resources/intune-mam-windowsinformationprotectioniprangecollection?view=graph-rest-1.0)<br/>[windowsInformationProtectionProxiedDomainCollection](/graph/api/resources/intune-mam-windowsinformationprotectionproxieddomaincollection?view=graph-rest-1.0)<br/>[windowsInformationProtectionResourceCollection](/graph/api/resources/intune-mam-windowsinformationprotectionresourcecollection?view=graph-rest-1.0)<br/>[windowsInformationProtectionStoreApp](/graph/api/resources/intune-mam-windowsinformationprotectionstoreapp?view=graph-rest-1.0)<br/>[windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-1.0)<br/>[windowsUpdateActiveHoursInstall](/graph/api/resources/intune-deviceconfig-windowsupdateactivehoursinstall?view=graph-rest-1.0)<br/>[windowsUpdateInstallScheduleType](/graph/api/resources/intune-deviceconfig-windowsupdateinstallscheduletype?view=graph-rest-1.0)<br/>[windowsUpdateScheduledInstall](/graph/api/resources/intune-deviceconfig-windowsupdatescheduledinstall?view=graph-rest-1.0)<br/>|
|Adição|v1.0|A ação [assign](/graph/api/intune-apps-mobileapp-assign?view=graph-rest-1.0) foi adicionada a [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-1.0) |
|Adição|v1.0|A ação [commit](/graph/api/intune-apps-mobileappcontentfile-commit?view=graph-rest-1.0) foi adicionada a [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-1.0) |
|Adição|v1.0|A ação [renewUpload](/graph/api/intune-apps-mobileappcontentfile-renewupload?view=graph-rest-1.0) foi adicionada a [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-1.0) |
|Adição|v1.0|A ação [retire](/graph/api/intune-devices-manageddevice-retire?view=graph-rest-1.0) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) |
|Adição|v1.0|A ação [wipe](/graph/api/intune-devices-manageddevice-wipe?view=graph-rest-1.0) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) |
|Adição|v1.0|A ação [resetPasscode](/graph/api/intune-devices-manageddevice-resetpasscode?view=graph-rest-1.0) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) |
|Adição|v1.0|A ação [remoteLock](/graph/api/intune-devices-manageddevice-remotelock?view=graph-rest-1.0) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) |
|Adição|v1.0|A ação [requestRemoteAssistance](/graph/api/intune-devices-manageddevice-requestremoteassistance?view=graph-rest-1.0) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) |
|Adição|v1.0|A ação [disableLostMode](/graph/api/intune-devices-manageddevice-disablelostmode?view=graph-rest-1.0) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) |
|Adição|v1.0|A ação [locateDevice](/graph/api/intune-devices-manageddevice-locatedevice?view=graph-rest-1.0) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) |
|Adição|v1.0|A ação [bypassActivationLock](/graph/api/intune-devices-manageddevice-bypassactivationlock?view=graph-rest-1.0) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) |
|Adição|v1.0|A ação [rebootNow](/graph/api/intune-devices-manageddevice-rebootnow?view=graph-rest-1.0) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) |
|Adição|v1.0|A ação [shutDown](/graph/api/intune-devices-manageddevice-shutdown?view=graph-rest-1.0) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) |
|Adição|v1.0|A ação [recoverPasscode](/graph/api/intune-devices-manageddevice-recoverpasscode?view=graph-rest-1.0) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) |
|Adição|v1.0|A ação [cleanWindowsDevice](/graph/api/intune-devices-manageddevice-cleanwindowsdevice?view=graph-rest-1.0) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) |
|Adição|v1.0|A ação [logoutSharedAppleDeviceActiveUser](/graph/api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser?view=graph-rest-1.0) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) |
|Adição|v1.0|A ação [deleteUserFromSharedAppleDevice](/graph/api/intune-devices-manageddevice-deleteuserfromsharedappledevice?view=graph-rest-1.0) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) |
|Adição|v1.0|A ação [syncDevice](/graph/api/intune-devices-manageddevice-syncdevice?view=graph-rest-1.0) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) |
|Adição|v1.0|A ação [windowsDefenderScan](/graph/api/intune-devices-manageddevice-windowsdefenderscan?view=graph-rest-1.0) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) |
|Adição|v1.0|A ação [windowsDefenderUpdateSignatures](/graph/api/intune-devices-manageddevice-windowsdefenderupdatesignatures?view=graph-rest-1.0) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) |
|Adição|v1.0|A ação [updateWindowsDeviceAccount](/graph/api/intune-devices-manageddevice-updatewindowsdeviceaccount?view=graph-rest-1.0) foi adicionada à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-1.0) |
|Adição|v1.0|A ação [removeAllDevicesFromManagement](/graph/api/intune-devices-user-removealldevicesfrommanagement?view=graph-rest-1.0) foi adicionada a [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) |
|Adição|v1.0|A ação [assign](/graph/api/intune-deviceconfig-deviceconfiguration-assign?view=graph-rest-1.0) foi adicionada a [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-1.0) |
|Adição|v1.0|A ação [assign](/graph/api/intune-deviceconfig-devicecompliancepolicy-assign?view=graph-rest-1.0) foi adicionada a [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-1.0) |
|Adição|v1.0|A ação [scheduleActionsForRules](/graph/api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules?view=graph-rest-1.0) foi adicionada a [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-1.0) |
|Adição|v1.0|A ação [setMobileDeviceManagementAuthority](/graph/api/intune-onboarding-organization-setmobiledevicemanagementauthority?view=graph-rest-1.0) foi adicionada a [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-1.0) |
|Adição|v1.0|A ação [syncMicrosoftStoreForBusinessApps](/graph/api/intune-onboarding-deviceappmanagement-syncmicrosoftstoreforbusinessapps?view=graph-rest-1.0) foi adicionada à entidade [deviceAppManagement](/graph/api/resources/intune-shared-deviceappmanagement?view=graph-rest-1.0) |
|Adição|v1.0|A ação [sync](/graph/api/intune-onboarding-devicemanagementexchangeconnector-sync?view=graph-rest-1.0) foi adicionada a [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-1.0) |
|Adição|v1.0|A ação [setPriority](/graph/api/intune-onboarding-deviceenrollmentconfiguration-setpriority?view=graph-rest-1.0) foi adicionada a [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-1.0) |
|Adição|v1.0|A ação [assign](/graph/api/intune-onboarding-deviceenrollmentconfiguration-assign?view=graph-rest-1.0) foi adicionada a [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-1.0) |
|Adição|v1.0|A ação [assign](/graph/api/intune-mam-targetedmanagedappprotection-assign?view=graph-rest-1.0) foi adicionada a [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-1.0) |
|Adição|v1.0|A ação [assign](/graph/api/intune-mam-targetedmanagedappconfiguration-assign?view=graph-rest-1.0) foi adicionada a [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-1.0) |
|Adição|v1.0|A ação [assign](/graph/api/intune-mam-windowsinformationprotection-assign?view=graph-rest-1.0) foi adicionada a [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-1.0) |
|Adição|v1.0|A ação [targetApps](/graph/api/intune-mam-managedapppolicy-targetapps?view=graph-rest-1.0) foi adicionada a [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-1.0) |
|Adição|v1.0|A ação [targetApps](/graph/api/intune-mam-managedappprotection-targetapps?view=graph-rest-1.0) foi adicionada a [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-1.0) |
|Adição|v1.0|A ação [targetApps](/graph/api/intune-mam-targetedmanagedappconfiguration-targetapps?view=graph-rest-1.0) foi adicionada a [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-1.0) |
|Adição|v1.0|A ação [wipeManagedAppRegistrationsByDeviceTag](/graph/api/intune-mam-user-wipemanagedappregistrationsbydevicetag?view=graph-rest-1.0) foi adicionada a [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) |
|Adição|v1.0|A ação [sendTestMessage](/graph/api/intune-notification-notificationmessagetemplate-sendtestmessage?view=graph-rest-1.0) foi adicionada a [notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-1.0) |
|Adição|v1.0|A ação [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-1.0) foi adicionada a [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-1.0) |
|Adição|v1.0|A ação [beginOnboarding](/graph/api/intune-remoteassistance-remoteassistancepartner-beginonboarding?view=graph-rest-1.0) foi adicionada a [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-1.0) |
|Adição|v1.0|A ação [disconnect](/graph/api/intune-remoteassistance-remoteassistancepartner-disconnect?view=graph-rest-1.0) foi adicionada a [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-1.0) |
|Adição|v1.0|A função [downloadApplePushNotificationCertificateSigningRequest](/graph/api/intune-devices-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest?view=graph-rest-1.0) foi adicionada a [applePushNotificationCertificate](/graph/api/resources/intune-devices-applepushnotificationcertificate?view=graph-rest-1.0) |
|Adição|v1.0|A função [deviceConfigurationUserActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationuseractivity?view=graph-rest-1.0) foi adicionada a [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-1.0) |
|Adição|v1.0|A função [deviceConfigurationDeviceActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationdeviceactivity?view=graph-rest-1.0) foi adicionada a [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-1.0) |
|Adição|v1.0|A função [verifyWindowsEnrollmentAutoDiscovery](/graph/api/intune-onboarding-devicemanagement-verifywindowsenrollmentautodiscovery?view=graph-rest-1.0) foi adicionada a [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-1.0) |
|Adição|v1.0|A função **getUserIdsWithFlaggedAppRegistration** foi adicionada à coleção [managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-1.0) |
|Adição|v1.0|A função [getManagedAppDiagnosticStatuses](/graph/api/intune-mam-user-getmanagedappdiagnosticstatuses?view=graph-rest-1.0) foi adicionada a [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) |
|Adição|v1.0|A função [getManagedAppPolicies](/graph/api/intune-mam-user-getmanagedapppolicies?view=graph-rest-1.0) foi adicionada a [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) |
|Adição|v1.0|A função [getEffectivePermissions](/graph/api/intune-rbac-devicemanagement-geteffectivepermissions?view=graph-rest-1.0) foi adicionada a [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-1.0) |
|Alteração|v1.0|A propriedade **mobileDeviceManagementAuthority** foi adicionada à entidade [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-1.0)|
|Alteração|v1.0|A propriedade **deviceEnrollmentLimit** foi adicionada à entidade [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0) |
|Alteração|v1.0|As propriedades de navegação **managedDevices**, **managedAppRegistrations** e **deviceManagementTroubleshootingEvents** foram adicionadas à entidade [user](/graph/api/resources/intune-shared-user?view=graph-rest-1.0)|
|||
|Adição|Beta|Foram adicionadas novas entidades:<br/>[deviceManagementScriptAssignment](/graph/api/resources/intune-devices-devicemanagementscriptassignment?view=graph-rest-beta)<br/>[iosCertificateProfile](/graph/api/resources/intune-deviceconfig-ioscertificateprofile?view=graph-rest-beta)<br/>[windowsInformationProtectionNetworkLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionnetworklearningsummary?view=graph-rest-beta)<br/>|
|Adição|Beta|Foram adicionados novos tipos complexos:<br/>[revokeAppleVppLicensesActionResult](/graph/api/resources/intune-devices-revokeapplevpplicensesactionresult?view=graph-rest-beta)<br/>[vppTokenRevokeLicensesActionResult](/graph/api/resources/intune-onboarding-vpptokenrevokelicensesactionresult?view=graph-rest-beta)<br/>|
|Adição|Beta|A ação [revokeToken](/graph/api/intune-androidforwork-androidforworkenrollmentprofile-revoketoken?view=graph-rest-beta) foi adicionada a [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) |
|Adição|Beta|A ação [assign](/graph/api/intune-apps-mobileapp-assign?view=graph-rest-beta) foi adicionada a [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) |
|Adição|Beta|A ação [assign](/graph/api/intune-devices-devicemanagementscript-assign?view=graph-rest-beta) foi adicionada a [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta) |
|Adição|Beta|A ação [revokeAppleVppLicenses](/graph/api/intune-devices-manageddevice-revokeapplevpplicenses?view=graph-rest-beta) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|Adição|Beta|A ação [assign](/graph/api/intune-deviceconfig-devicecompliancepolicy-assign?view=graph-rest-beta) foi adicionada a [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) |
|Adição|Beta|A ação [syncLicenses](/graph/api/intune-onboarding-vpptoken-revokelicenses?view=graph-rest-beta) foi adicionada à entidade [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) |
|Adição|Beta|A ação [wipeManagedAppRegistrationsByDeviceTag](/graph/api/intune-mam-user-wipemanagedappregistrationsbydevicetag?view=graph-rest-beta) foi adicionada a [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) |
|Adição|Beta|A ação [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-beta) foi adicionada a [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) |
|Adição|Beta|A função [getEffectiveDeviceEnrollmentConfigurations](/graph/api/intune-onboarding-user-geteffectivedeviceenrollmentconfigurations?view=graph-rest-beta) foi adicionada a [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta) |
|Exclusão|Beta|Foram removidas as seguintes entidades:<br/>**appReportingOverviewStatus**<br/>**complianceSettingStateSummary**<br/>**deviceConfigurationUserStateSummary**<br/>**eBookGroupAssignment**<br/>**eBookVppGroupAssignment**<br/>**mobileAppGroupAssignment**<br/>**mobileAppVppGroupAssignment**<br/>|
|Exclusão|Beta|Foram removidos os seguintes tipos complexos:<br/>**androidForWorkAppConfigurationExample**<br/>**androidForWorkAppConfigurationExampleJson**<br/>**appInstallationFailure**<br/>**appsComplianceListItem**<br/>**defaultDeviceEnrollmentRestrictions**<br/>**defaultDeviceEnrollmentWindowsHelloForBusinessSettings**<br/>**deviceEnrollmentPlatformRestrictions**<br/>|
|Alteração|Beta|As propriedades **securityRequireVerifyApps**, **securityRequireSafetyNetAttestationBasicIntegrity**, **securityRequireSafetyNetAttestationCertifiedDevice**, **securityRequireGooglePlayServices**, **securityRequireUpToDateSecurityProviders** e **securityRequireCompanyPortalAppIntegrity** foram adicionadas à entidade [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **packageId** foi adidionada à entidade [androidForWorkApp](/graph/api/resources/intune-apps-androidforworkapp?view=graph-rest-beta)|
|Alteração|Beta|Foi alterado o tipo das seguintes propriedades na entidade [androidForWorkAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationschema?view=graph-rest-beta):<br/>**exampleJson** de [androidForWorkAppConfigurationExample](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationexample?view=graph-rest-beta) para Binário<br/>|
|Alteração|Beta|As propriedades **securityRequireVerifyApps**, **securityRequireSafetyNetAttestationBasicIntegrity**, **securityRequireSafetyNetAttestationCertifiedDevice**, **securityRequireGooglePlayServices**, **securityRequireUpToDateSecurityProviders** e **securityRequireCompanyPortalAppIntegrity** foram adicionadas à entidade [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **displayName**, **lastModifiedDateTime**, **enrolledDeviceCount**, **qrCodeContent** and **qrCodeImage** foram adicionadas à entidade [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **isTokenActive** foi removida da entidade [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **innerAuthenticationProtocolForEapTtls**, **innerAuthenticationProtocolForPeap** e **outerIdentityPrivacyTemporaryValue** foram adicionadas à entidade [androidForWorkEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkenterprisewificonfiguration?view=graph-rest-beta).|
|Alteração|Beta|As propriedades **workProfileBlockCrossProfileCopyPaste** and **securityRequireVerifyApps** foram adicionadas à entidade [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **securityRequireVerifyApps** foi adicionada à entidade [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **packageId** e **identityVersion** foram adicionadas à entidade [androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **packageId** foi adidionada à entidade [androidStoreApp](/graph/api/resources/intune-apps-androidstoreapp?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **faceIdBlocked** foi adicionada à entidade [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **members** foi adicionada à entidade [deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **macOSRestriction** foi adicionada à entidade [deviceEnrollmentPlatformRestrictionsConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **whenPartnerDevicesWillBeRemovedDateTime** e **whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime** foram adicionadas à entidade [deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-beta)|
|Alteração|Beta|Foi alterado o tipo das seguintes propriedades na entidade [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta):<br/>**scriptContent** de Cadeia de caracteres para Binário<br/>|
|Alteração|Beta|A propriedade **smimeEnablePerMessageSwitch** foi adicionada à entidade [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **identityVersion** foi adicionada à entidade [iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **faceIdBlocked** foi adicionada à entidade [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **packageId** e **identityVersion** foram adicionadas à entidade [managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **azureADDeviceId** e **remoteAssistanceSessionErrorDetails** foram adicionadas à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **legacyAppConfiguration** foi removida da entidade [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **identityVersion** foi adicionada à entidade [managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **identityVersion** foi removida da entidade [managedMobileLobApp](/graph/api/resources/intune-apps-managedmobilelobapp?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **publishingState** foi adicionada à entidade [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **installState** foi adicionada à entidade [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **identityVersion** foi removida da entidade [mobileLobApp](/graph/api/resources/intune-apps-mobilelobapp?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **allowPartnerToCollectIOSApplicationMetadata** foi adicionada à entidade [mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **members** foi removida da entidade [roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **lastModifiedDateTime** foi adicionada à entidade [termsAndConditions](/graph/api/resources/intune-companyterms-termsandconditions?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **deviceThreatProtectionEnabled** e **deviceThreatProtectionRequiredSecurityLevel** foram adicionadas à entidade [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **minimumUpdateAutoInstallClassification** foi removida da entidade [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **privacyBlockPublishUserActivities** e **privacyBlockActivityFeed** foram adicionadas à entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **configurationAccountType** foi adicionada à entidade [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **trustedNetworkDomains** foi removida da entidade [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **minimumUpdateAutoInstallClassification** foi removida da entidade [windows81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows81compliancepolicy?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **identityVersion** foi adicionada à entidade [windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **daysWithoutContactBeforeUnenroll** foi adicionada à entidade [windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **identityVersion** foi adicionada à entidade [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **identityVersion** foi adicionada à entidade [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **identityVersion** foi adicionada à entidade [windowsPhoneXAP](/graph/api/resources/intune-apps-windowsphonexap?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **identityVersion** foi adicionada à entidade [windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **domainJoinConfiguration** foi adicionada à entidade [activeDirectoryWindowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **notificationMessageTemplate** foi removida da entidade [deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **groupAssignments** foi removida da entidade [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **windowsInformationProtectionNetworkLearningSummaries** foi adicionada à entidade [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **deviceConfigurationUserStateSummaries** foi removida da entidade [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Alteração|Beta|Foi alterado o tipo das seguintes propriedades na entidade [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta):<br/>**roleAssignments** da coleção [roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta) para a coleção [deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta)<br/>|
|Alteração|Beta|A propriedade de navegação **assignments** foi adicionada à entidade [deviceManagementScript](/graph/api/resources/intune-devices-devicemanagementscript?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **smimeEncryptionCertificate** foi adicionada à entidade [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta)|
|Alteração|Beta|Foi alterado o tipo das seguintes propriedades na entidade [iosEasEmailProfileConfiguration](/graph/api/resources/intune-deviceconfig-ioseasemailprofileconfiguration?view=graph-rest-beta):<br/>**smimeSigningCertificate** de [iosCertificateProfileBase](/graph/api/resources/intune-deviceconfig-ioscertificateprofilebase?view=graph-rest-beta) para [iosCertificateProfile](/graph/api/resources/intune-deviceconfig-ioscertificateprofile?view=graph-rest-beta)<br/>|
|Alteração|Beta|A propriedade de navegação **vppToken** foi removida da entidade [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **groupAssignments** foi removida da entidade [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **groupAssignments** foi removida da entidade [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta)|
|Alteração|Beta|As propriedades de navegação **depOnboardingSettings** e **appleVolumePurchaseProgramTokens** foram removidas da entidade [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **deviceEnrollmentConfigurations** foi adicionada à entidade [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta)|
|Alteração|Beta|Foram removidas as propriedades **windowsCommercialId** e **windowsCommercialIdLastModifiedTime** do tipo complexo [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **showDisplayNameNextToLogo** foi adicionada ao tipo complexo [intuneBrand](/graph/api/resources/intune-onboarding-intunebrand?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **deviceUsageType** foi adicionada ao tipo complexo [outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **supportsUserLicensing** e **supportsDeviceLicensing** foram adicionadaa ao tipo complexo [vppLicensingType](/graph/api/resources/intune-apps-vpplicensingtype?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **actionMessage** foi removida do tipo complexo [vppTokenActionResult](/graph/api/resources/intune-onboarding-vpptokenactionresult?view=graph-rest-beta)|

### <a name="reports-apis"></a>APIs de relatórios
| Tipo de alteração | Versão | Descrição                              |
|:------------|:--------|:-----------------------------------------|
| Adição    | v1.0    | As seguintes APIs foram adicionadas:<br>[getTeamsUserActivityUserDetail](/graph/api/reportroot-getteamsuseractivityuserdetail?view=graph-rest-1.0)<br>[getTeamsUserActivityCounts](/graph/api/reportroot-getteamsuseractivitycounts?view=graph-rest-1.0)<br>[getTeamsUserActivityUserCounts](/graph/api/reportroot-getteamsuseractivityusercounts?view=graph-rest-1.0)<br>[getTeamsDeviceUsageUserDetail](/graph/api/reportroot-getteamsdeviceusageuserdetail?view=graph-rest-1.0)<br>[getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts?view=graph-rest-1.0)<br>[getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getteamsdeviceusagedistributionusercounts?view=graph-rest-1.0) |

## <a name="december-2017"></a>Dezembro de 2017

### <a name="delta-query"></a>Consulta delta

| Tipo de alteração | Versão | Descrição                              |
|:------------|:--------|:-----------------------------------------|
| Alteração      | v1.0    | Foi adicionado um novo recurso de filtragem da consulta opcional (por ID) para [usuários](/graph/api/user-delta?view=graph-rest-1.0) e [grupos](/graph/api/group-delta?view=graph-rest-1.0). |

### <a name="microsoft-intune-apis"></a>APIs do Microsoft Intune

|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|Beta|Foram adicionadas novas entidades:<br/>[androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta)<br/>[deviceAndAppManagementRoleAssignment](/graph/api/resources/intune-rbac-deviceandappmanagementroleassignment?view=graph-rest-beta)<br/>[deviceAndAppManagementRoleDefinition](/graph/api/resources/intune-rbac-deviceandappmanagementroledefinition?view=graph-rest-beta)<br/>[macOSLobApp](/graph/api/resources/intune-apps-macoslobapp?view=graph-rest-beta)<br/>|
|Adição|Beta|Foram adicionados novos tipos complexos:<br/>[resourceAction](/graph/api/resources/intune-rbac-resourceaction?view=graph-rest-beta)<br/>[updateWindowsDeviceAccountActionParameter](/graph/api/resources/intune-devices-updatewindowsdeviceaccountactionparameter?view=graph-rest-beta)<br/>[vppTokenActionResult](/graph/api/resources/intune-onboarding-vpptokenactionresult?view=graph-rest-beta)<br/>[windowsDeviceAADAccount](/graph/api/resources/intune-devices-windowsdeviceaadaccount?view=graph-rest-beta)<br/>[windowsDeviceAccount](/graph/api/resources/intune-devices-windowsdeviceaccount?view=graph-rest-beta)<br/>[windowsDeviceADAccount](/graph/api/resources/intune-devices-windowsdeviceadaccount?view=graph-rest-beta)<br/>|
|Adição|Beta|A ação [revokeTokens](/graph/api/intune-androidforwork-androidforworkenrollmentprofile-revoketokens?view=graph-rest-beta) foi adicionada à entidade [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) |
|Adição|Beta|A ação [createTokens](/graph/api/intune-androidforwork-androidforworkenrollmentprofile-createtoken?view=graph-rest-beta) foi adicionada à entidade [androidForWorkEnrollmentProfile](/graph/api/resources/intune-androidforwork-androidforworkenrollmentprofile?view=graph-rest-beta) |
|Adição|Beta|A ação [wipe](/graph/api/intune-devices-manageddevice-wipe?view=graph-rest-beta) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|Adição|Beta|A ação [updateWindowsDeviceAccount](/graph/api/intune-devices-manageddevice-updatewindowsdeviceaccount?view=graph-rest-beta) foi adicionada à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|Adição|Beta|A ação [syncLicenses](/graph/api/intune-onboarding-vpptoken-revokelicenses?view=graph-rest-beta) foi adicionada à entidade [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) |
|Adição|Beta|A função [getDevicePasscode](/graph/api/intune-deviceconfig-devicecompliancepolicy-getdevicepasscode?view=graph-rest-beta) foi adicionada à coleção [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) |
|Adição|Beta|A função [getEffectivePermissions](/graph/api/intune-rbac-devicemanagement-geteffectivepermissions?view=graph-rest-beta) foi adicionada a [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta) |
|Exclusão|Beta|Foram removidas as seguintes entidades:<br/>**windowsStoreForBusinessApp**<br/>|
|Exclusão|Beta|Foram removidos os seguintes tipos complexos:<br/>**windowsStoreForBusinessAppAssignmentSettings**<br/>|
|Alteração|Beta|A propriedade **dateAndTimeBlockChanges** foi adicionada à entidade [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **enableAuthenticationViaCompanyPortal** foi removida da entidade [depEnrollmentProfile](/graph/api/resources/intune-corpenrollment-depenrollmentprofile?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **windowsStoreForBusinessLastSuccessfulSyncDateTime**, **isEnabledForWindowsStoreForBusiness**, **windowsStoreForBusinessLanguage** e **windowsStoreForBusinessLastCompletedApplicationSyncTime** foram removidas da entidade [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **maximumDepTokens** e **intuneAccountId** foram adicionadas à entidade [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **enableAuthenticationViaCompanyPortal** foi adicionada à entidade [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **managedDeviceName** e **partnerReportedThreatState** foram adicionadas à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **installProgressDisplayLevel** foi adicionada à entidade [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **resourceScopes** foi adicionada à entidade [roleAssignment](/graph/api/resources/intune-rbac-roleassignment?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **rolePermissions** e **isBuiltIn** foram adicionadas à entidade [roleDefinition](/graph/api/resources/intune-rbac-roledefinition?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **tokenActionResults** foi adicionada à entidade [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **minimumUpdateAutoInstallClassification** foi adicionada à entidade [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **defenderSecurityCenterDisableAppBrowserUI**, **defenderSecurityCenterDisableFamilyUI**, **defenderSecurityCenterDisableHealthUI**, **defenderSecurityCenterDisableNetworkUI**, **defenderSecurityCenterDisableVirusUI**, **defenderSecurityCenterOrganizationDisplayName**, **defenderSecurityCenterHelpEmail**, **defenderSecurityCenterHelpPhone**, **defenderSecurityCenterHelpURL**, ** defenderSecurityCenterNotificationsFromApp**, **defenderSecurityCenterITContactDisplay** e **applicationGuardAllowVirtualGPU** foram adicionadas à entidade [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **enableAutomaticRedeployment** e **authenticationAllowFIDODevice** foram adicionadas à entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **trustedNetworkDomains** foi adicionada à entidade [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **minimumUpdateAutoInstallClassification** foi adicionada à entidade [windows81CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows81compliancepolicy?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **androidForWorkEnrollmentProfiles** foi adicionada à entidade [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **healthAttestationSupportedStatus** foi adicionada ao tipo complexo [deviceHealthAttestationState](/graph/api/resources/intune-devices-devicehealthattestationstate?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **tpmSpecificationVersion**, **operatingSystemEdition**, **deviceFullQualifiedDomainName**, ** deviceGuardVirtualizationBasedSecurityHardwareRequirementState**, **deviceGuardVirtualizationBasedSecurityState** e ** deviceGuardLocalSystemAuthorityCredentialGuardState** foram adicionadas ao tipo complexo [hardwareInformation](/graph/api/resources/intune-devices-hardwareinformation?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **vpnConfigurationId** foi adicionada ao tipo complexo [iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **resourceActions** foi adicionada ao tipo complexo [rolePermission](/graph/api/resources/intune-rbac-rolepermission?view=graph-rest-beta)|

### <a name="reports-apis"></a>APIs de relatórios
| Tipo de alteração | Versão | Descrição                              |
|:------------|:--------|:-----------------------------------------|
| Adição    | v1.0    | As seguintes APIs foram adicionadas:<br>[getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-1.0)<br>[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-1.0)<br>[getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-1.0)<br>[getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-1.0)<br>[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-1.0)<br>[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-1.0)<br>[getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-1.0)<br>[getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-1.0)<br>[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-1.0)<br>[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-1.0)<br>[getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-1.0)<br>[getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-1.0)<br>[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-1.0)<br>[getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-1.0)<br>[getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-1.0)<br>[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-1.0)<br>[getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-1.0)<br>[getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-1.0)<br> [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-1.0)<br>[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-1.0)<br>[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-1.0)<br>[getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-1.0)<br>[getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-1.0)<br>[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-1.0)<br>[getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-1.0)<br>[getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-1.0)<br>[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-1.0)<br>[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-1.0)<br>[getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-1.0)<br>[getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-1.0)<br>[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-1.0)<br>[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-1.0)<br>[getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-1.0)<br>[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-1.0)<br>[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-1.0)<br>[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-1.0)<br>[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-1.0)<br>[getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-1.0)<br>[getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-1.0)<br>[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-1.0)<br>[getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-1.0)<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-1.0)<br>[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-1.0)<br>[getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-1.0)<br>[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-1.0)<br>[getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-1.0)<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-1.0)<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-1.0)<br>[getYammerActivityUserDetail](/graph/api/reportroot-getyammeractivityuserdetail?view=graph-rest-1.0)<br>[getYammerActivityCounts](/graph/api/reportroot-getyammeractivitycounts?view=graph-rest-1.0)<br>[getYammerActivityUserCounts](/graph/api/reportroot-getyammeractivityusercounts?view=graph-rest-1.0)<br>[getYammerDeviceUsageUserDetail](/graph/api/reportroot-getyammerdeviceusageuserdetail?view=graph-rest-1.0)<br>[getYammerDeviceUsageDistributionUserCounts](/graph/api/reportroot-getyammerdeviceusagedistributionusercounts?view=graph-rest-1.0)<br>[getYammerDeviceUsageUserCounts](/graph/api/reportroot-getyammerdeviceusageusercounts?view=graph-rest-1.0)<br>[getYammerGroupsActivityDetail](/graph/api/reportroot-getyammergroupsactivitydetail?view=graph-rest-1.0)<br>[getYammerGroupsActivityGroupCounts](/graph/api/reportroot-getyammergroupsactivitygroupcounts?view=graph-rest-1.0)<br>[getYammerGroupsActivityCounts](/graph/api/reportroot-getyammergroupsactivitycounts?view=graph-rest-1.0).|
| Adição    | Beta    | As seguintes APIs foram adicionadas:<br>[getTeamsUserActivityUserDetail](/graph/api/reportroot-getteamsuseractivityuserdetail?view=graph-rest-beta)<br>[getTeamsUserActivityCounts](/graph/api/reportroot-getteamsuseractivitycounts?view=graph-rest-beta)<br>[getTeamsUserActivityUserCounts](/graph/api/reportroot-getteamsuseractivityusercounts?view=graph-rest-beta)<br>[getTeamsDeviceUsageUserDetail](/graph/api/reportroot-getteamsdeviceusageuserdetail?view=graph-rest-beta)<br>[getTeamsDeviceUsageUserCounts](/graph/api/reportroot-getteamsdeviceusageusercounts?view=graph-rest-beta)<br>[getTeamsDeviceUsageDistributionUserCounts](/graph/api/reportroot-getteamsdeviceusagedistributionusercounts?view=graph-rest-beta) |

## <a name="november-2017"></a>Novembro de 2017

### <a name="azure-ad-synchronization-apis"></a>APIs de sincronização do Azure AD

| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Adição    | Beta    | Suporte adicional para a sincronização de identidade do Azure AD, incluindo os seguintes recursos:<br/>[Cargo](/graph/api/resources/synchronization-synchronizationjob?view=graph-rest-beta)<br/>[Esquema](/graph/api/resources/synchronization-synchronizationschema?view=graph-rest-beta)<br/>[Modelo](/graph/api/resources/synchronization-synchronizationtemplate?view=graph-rest-beta)<br/>Confira os tópicos de recursos para obter dados sobre os métodos disponíveis.|

### <a name="education-apis"></a>APIs de educação

|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|Beta|Suporte adicional para cenários de educação, incluindo os seguintes recursos:<br/>[Escolas](/graph/api/resources/educationschool?view=graph-rest-beta)<br/>[Aulas](/graph/api/resources/educationclass?view=graph-rest-beta)<br/>[Usuários](/graph/api/resources/educationuser?view=graph-rest-beta)<br/>[Atribuições](/graph/api/resources/educationassignment?view=graph-rest-beta)<br/>[Envios](/graph/api/resources/educationsubmission?view=graph-rest-beta)<br/>Confira os tópicos de recursos para obter dados sobre os métodos disponíveis.|

### <a name="microsoft-intune-apis"></a>APIs do Microsoft Intune
|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|Beta|Foram adicionadas novas entidades:<br/>[auditEvent](/graph/api/resources/intune-auditing-auditevent?view=graph-rest-beta)<br/>[deviceManagementTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-devicemanagementtroubleshootingevent?view=graph-rest-beta)<br/>[deviceSetupConfiguration](/graph/api/resources/intune-deviceconfig-devicesetupconfiguration?view=graph-rest-beta)<br/>[enrollmentTroubleshootingEvent](/graph/api/resources/intune-troubleshooting-enrollmenttroubleshootingevent?view=graph-rest-beta)<br/>[macOSOfficeSuiteApp](/graph/api/resources/intune-apps-macosofficesuiteapp?view=graph-rest-beta)<br/>[microsoftStoreForBusinessApp](/graph/api/resources/intune-apps-microsoftstoreforbusinessapp?view=graph-rest-beta)<br/>[ndesConnector](/graph/api/resources/intune-deviceconfig-ndesconnector?view=graph-rest-beta)<br/>|
|Adição|Beta|Foram adicionados novos tipos complexos:<br/>[auditActor](/graph/api/resources/intune-auditing-auditactor?view=graph-rest-beta)<br/>[auditProperty](/graph/api/resources/intune-auditing-auditproperty?view=graph-rest-beta)<br/>[auditResource](/graph/api/resources/intune-auditing-auditresource?view=graph-rest-beta)<br/>[bulkManagedDeviceActionResult](/graph/api/resources/intune-devices-bulkmanageddeviceactionresult?view=graph-rest-beta)<br/>[deviceProtectionOverview](/graph/api/resources/intune-devices-deviceprotectionoverview?view=graph-rest-beta)<br/>[microsoftStoreForBusinessAppAssignmentSettings](/graph/api/resources/intune-apps-microsoftstoreforbusinessappassignmentsettings?view=graph-rest-beta)<br/>[operatingSystemVersionRange](/graph/api/resources/intune-deviceconfig-operatingsystemversionrange?view=graph-rest-beta)<br/>[remoteLockActionResult](/graph/api/resources/intune-devices-remotelockactionresult?view=graph-rest-beta)<br/>|
|Adição|Beta|A ação executeAction foi adicionada à coleção [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|Adição|Beta|A ação [wipe](/graph/api/intune-devices-manageddevice-wipe?view=graph-rest-beta) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|Adição|Beta|A ação [shutDown](/graph/api/intune-devices-manageddevice-shutdown?view=graph-rest-beta) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
|Adição|Beta|A ação [assign](/graph/api/intune-deviceconfig-deviceconfiguration-assign?view=graph-rest-beta) foi adicionada a [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) |
|Adição|Beta|A ação [syncMicrosoftStoreForBusinessApps](/graph/api/intune-onboarding-deviceappmanagement-syncmicrosoftstoreforbusinessapps?view=graph-rest-beta) foi adicionada à entidade [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) |
|Adição|Beta|A ação setDefaultProfile foi adicionada à entidade [enrollmentProfile](/graph/api/resources/intune-corpenrollment-enrollmentprofile?view=graph-rest-beta) |
|Adição|Beta|A ação shareForSchoolDataSyncService foi adicionada à entidade [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) |
|Adição|Beta|A ação unshareForSchoolDataSyncService foi adicionada à entidade [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) |
|Adição|Beta|A função getAuditCategories foi adicionada à coleção [auditEvent](/graph/api/resources/intune-auditing-auditevent?view=graph-rest-beta) |
|Adição|Beta|A função getAuditActivityTypes foi adicionada à coleção [auditEvent](/graph/api/resources/intune-auditing-auditevent?view=graph-rest-beta) |
|Exclusão|Beta|Foram removidas as seguintes entidades:<br/>**mobileAppIdentifierDeployment**<br/>|
|Exclusão|Beta|Foram removidos os seguintes tipos complexos:<br/>**windowsInformationProtectionCloudResource**<br/>**windowsInformationProtectionCloudResourceCollection**<br/>|
|Alteração|Beta|As seguintes propriedades da entidade [androidDeviceComplianceLocalActionLockDeviceWithPasscode](/graph/api/resources/intune-deviceconfig-androiddevicecompliancelocalactionlockdevicewithpasscode?view=graph-rest-beta) foram alteradas:<br/>**passcode** de obrigatório para opcional<br/>|
|Alteração|Beta|As propriedades **microsoftStoreForBusinessLastSuccessfulSyncDateTime**, **isEnabledForMicrosoftStoreForBusiness**, **microsoftStoreForBusinessLanguage** e **microsoftStoreForBusinessLastCompletedApplicationSyncTime** foram adicionadas à entidade [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **target** foi adicionada à entidade [deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **deviceProtectionOverview** foi adicionada à entidade [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **exchangeAlias** e **exchangeOrganization** foram adicionadas à entidade [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **appStoreUrl** e **minimumSupportedOperatingSystem** foram adicionadas à entidade [managedAndroidStoreApp](/graph/api/resources/intune-apps-managedandroidstoreapp?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **remoteAssistanceSessionErrorString** foi adicionada à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **appStoreUrl**, **applicableDeviceType** e **minimumSupportedOperatingSystem** foram adicionadas à entidade [managedIOSStoreApp](/graph/api/resources/intune-apps-managediosstoreapp?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **notApplicableDeviceCount**, **pendingInstallDeviceCount**, **notApplicableUserCount** e **pendingInstallUserCount** foram adicionadas à entidade [mobileAppInstallSummary](/graph/api/resources/intune-apps-mobileappinstallsummary?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **targetedSecurityGroupIds**e **targetedSecurityGroupsCount** foram removidas da entidade [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **targetedSecurityGroupsCount** e **targetedSecurityGroupIds** foram removidas da entidade [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **validOperatingSystemBuildRanges** foi adicionada à entidade [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **activeFirewallRequired**, **uacRequired** e **validOperatingSystemBuildRanges** foram adicionadas à entidade [windows10MobileCompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10mobilecompliancepolicy?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **enableExpeditedTelemetryReporting** foi adicionada à entidade [windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **allowedApps**, **enterpriseCloudResources** e **targetedSecurityGroupIds** foram removidas da entidade [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **ignoreVersionDetection** foi adicionada à entidade [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **mobileAppIdentifierDeployments** foi removida da entidade [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **mobileAppIdentifierDeployments** foi removida da entidade [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **assignments** foi adicionada à entidade [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **deviceConfiguration** foi removida da entidade [deviceConfigurationAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationassignment?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **deviceConfiguration** foi adicionada à entidade [deviceConfigurationGroupAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationgroupassignment?view=graph-rest-beta)|
|Alteração|Beta|As propriedades de navegação **deviceSetupConfigurations**, **ndesConnectors**, **exchangeOnPremisesPolicies**, **conditionalAccessSettings**, **auditEvents** e **troubleshootingEvents** foram adicionadas à entidade [deviceManagement](/graph/api/resources/intune-androidforwork-devicemanagement?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **mobileAppIdentifierDeployments** foi removida da entidade [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **windowsProtectionState** foi adicionada à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Alteração|Beta|As propriedades de navegação **mobileAppIdentifierDeployments** e **targetedSecurityGroups** foram removidas da entidade [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **targetedSecurityGroups** foi removida da entidade [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **deviceManagementTroubleshootingEvents** foi adicionada è entidade [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **allowedAppLockerFiles** foi removida da entidade [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **windowsProtectionState** foi removida da entidade [windowsManagedDevice](/graph/api/resources/intune-devices-windowsmanageddevice?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **v11_0** foi adicionada ao tipo complexo [iosMinimumOperatingSystem](/graph/api/resources/intune-apps-iosminimumoperatingsystem?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **denied** foi adicionada ao tipo complexo [windowsInformationProtectionApp](/graph/api/resources/intune-mam-windowsinformationprotectionapp?view=graph-rest-beta)|

### <a name="reports-apis"></a>APIs de relatórios
| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Adição    | Beta    | Adicionado suporte JSON para as seguintes APIs:<br>[getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta)<br>[getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta)<br>[getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta)<br>[getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-beta)<br>[getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-beta)<br>[getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-beta)<br>[getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-beta)<br>[getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta)<br>[getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-beta)<br>[getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-beta)<br>[getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-beta)<br>[getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-beta)<br>[getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-beta)<br>[getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-beta)<br>[getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-beta)<br>[getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-beta)<br>[getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-beta)<br> [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-beta)<br>[getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-beta)<br>[getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-beta)<br>[getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-beta)<br>[getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-beta)<br>[getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-beta)<br>[getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-beta)<br>[getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-beta)<br>[getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-beta)<br>[getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-beta)<br>[getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-beta)<br>[getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-beta)<br>[getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-beta)<br>[getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-beta)<br>[getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta)<br>[getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-beta)<br>[getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-beta)<br>[getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-beta)<br>[getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-beta)<br>[getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-beta)<br>[getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-beta)<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-beta)<br>[getYammerActivityUserDetail](/graph/api/reportroot-getyammeractivityuserdetail?view=graph-rest-beta)<br>[getYammerActivityCounts](/graph/api/reportroot-getyammeractivitycounts?view=graph-rest-beta)<br>[getYammerActivityUserCounts](/graph/api/reportroot-getyammeractivityusercounts?view=graph-rest-beta)<br>[getYammerDeviceUsageUserDetail](/graph/api/reportroot-getyammerdeviceusageuserdetail?view=graph-rest-beta)<br>[getYammerDeviceUsageDistributionUserCounts](/graph/api/reportroot-getyammerdeviceusagedistributionusercounts?view=graph-rest-beta)<br>[getYammerDeviceUsageUserCounts](/graph/api/reportroot-getyammerdeviceusageusercounts?view=graph-rest-beta)<br>[getYammerGroupsActivityDetail](/graph/api/reportroot-getyammergroupsactivitydetail?view=graph-rest-beta)<br>[getYammerGroupsActivityGroupCounts](/graph/api/reportroot-getyammergroupsactivitygroupcounts?view=graph-rest-beta)<br>[getYammerGroupsActivityCounts](/graph/api/reportroot-getyammergroupsactivitycounts?view=graph-rest-beta). |

### <a name="webhooks"></a>Webhooks

| Tipo de alteração | Versão | Descrição                              |
|:------------|:--------|:-----------------------------------------|
| Alteração significativa | Beta e v1.0 | [Webhooks](/graph/api/resources/webhooks?view=graph-rest-1.0) [reduzidos ao comprimento máximo do tempo de expiração da assinatura](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type) para itens raiz da unidade. O novo valor é o tempo de expiração máximo com suporte para itens raiz da unidade. |

## <a name="october-2017"></a>Outubro de 2017

### <a name="azure-ad-apis"></a>APIs do Azure AD

| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
|Adição|Beta|A entidade [identityProvider](/graph/api/resources/identityprovider?view=graph-rest-beta) e as operações [create](/graph/api/identityprovider-post-identityproviders?view=graph-rest-beta), [list](/graph/api/identityprovider-list?view=graph-rest-beta), [get](/graph/api/identityprovider-get?view=graph-rest-beta), [update](/graph/api/identityprovider-update?view=graph-rest-beta) e [delete](/graph/api/identityprovider-delete?view=graph-rest-beta) foram adicionadas.|


### <a name="microsoft-intune-apis"></a>APIs do Microsoft Intune
|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|Beta|Foram adicionadas novas entidades:<br/>[androidDeviceComplianceLocalActionLockDeviceWithPasscode](/graph/api/resources/intune-deviceconfig-androiddevicecompliancelocalactionlockdevicewithpasscode?view=graph-rest-beta)<br/>[iosLobAppProvisioningConfigurationAssignment](/graph/api/resources/intune-apps-ioslobappprovisioningconfigurationassignment?view=graph-rest-beta)<br/>[iosVppEBookAssignment](/graph/api/resources/intune-books-iosvppebookassignment?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationAssignment](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationassignment?view=graph-rest-beta)<br/>[managedEBookAssignment](/graph/api/resources/intune-books-managedebookassignment?view=graph-rest-beta)<br/>[managedMobileApp](/graph/api/resources/intune-mam-managedmobileapp?view=graph-rest-beta)<br/>[mobileAppAssignment](/graph/api/resources/intune-apps-mobileappassignment?view=graph-rest-beta)<br/>[termsAndConditionsAssignment](/graph/api/resources/intune-companyterms-termsandconditionsassignment?view=graph-rest-beta)<br/>[vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta)<br/>[windows10PFXImportCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10pfximportcertificateprofile?view=graph-rest-beta)<br/>[windowsAssignedAccessProfile](/graph/api/resources/intune-deviceconfig-windowsassignedaccessprofile?view=graph-rest-beta)<br/>[windowsDomainJoinConfiguration](/graph/api/resources/intune-deviceconfig-windowsdomainjoinconfiguration?view=graph-rest-beta)<br/>|
|Adição|Beta|Foram adicionados novos tipos complexos:<br/>[iosLobAppAssignmentSettings](/graph/api/resources/intune-apps-ioslobappassignmentsettings?view=graph-rest-beta)<br/>[iosSingleSignOnSettings](/graph/api/resources/intune-deviceconfig-iossinglesignonsettings?view=graph-rest-beta)<br/>[iosStoreAppAssignmentSettings](/graph/api/resources/intune-apps-iosstoreappassignmentsettings?view=graph-rest-beta)<br/>[iosVppAppAssignmentSettings](/graph/api/resources/intune-apps-iosvppappassignmentsettings?view=graph-rest-beta)<br/>[mobileAppAssignmentSettings](/graph/api/resources/intune-apps-mobileappassignmentsettings?view=graph-rest-beta)<br/>[proxiedDomain](/graph/api/resources/intune-deviceconfig-proxieddomain?view=graph-rest-beta)<br/>[windowsInformationProtectionProxiedDomainCollection](/graph/api/resources/intune-mam-windowsinformationprotectionproxieddomaincollection?view=graph-rest-beta)<br/>[windowsStoreForBusinessAppAssignmentSettings](/graph/api/resources/intune-apps-windowsstoreforbusinessappassignmentsettings?view=graph-rest-beta)<br/>|
|Adição|Beta|A ação [assign](/graph/api/intune-apps-mobileapp-assign?view=graph-rest-beta) foi adicionada a [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) |
|Adição|Beta|A ação [assign](/graph/api/intune-apps-ioslobappprovisioningconfiguration-assign?view=graph-rest-beta) foi adicionada a [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) |
|Adição|Beta|A ação [assign](/graph/api/intune-apps-manageddevicemobileappconfiguration-assign?view=graph-rest-beta) foi adicionada a [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) |
|Adição|Beta|A ação [assign](/graph/api/intune-deviceconfig-devicecompliancepolicy-assign?view=graph-rest-beta) foi adicionada a [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) |
|Adição|Beta|A ação [assignedAccessMultiModeProfiles](/graph/api/intune-deviceconfig-deviceconfiguration-assignedaccessmultimodeprofiles?view=graph-rest-beta) foi adicionada a [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) |
|Adição|Beta|A ação [syncLicenses](/graph/api/intune-onboarding-vpptoken-synclicenses?view=graph-rest-beta) foi adicionada a [vppToken](/graph/api/resources/intune-onboarding-vpptoken?view=graph-rest-beta) |
|Adição|Beta|A ação [targetApps](/graph/api/intune-mam-managedapppolicy-targetapps?view=graph-rest-beta) foi adicionada a [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta) |
|Adição|Beta|A ação [targetApps](/graph/api/intune-mam-managedappprotection-targetapps?view=graph-rest-beta) foi adicionada a [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) |
|Adição|Beta|A ação [targetApps](/graph/api/intune-mam-targetedmanagedappconfiguration-targetapps?view=graph-rest-beta) foi adicionada a [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) |
|Adição|Beta|A ação [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-beta) foi adicionada a [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) |
|Exclusão|Beta|Foram removidas as seguintes entidades:<br/>**cloudPkiSubscription**<br/>|
|Exclusão|Beta|Foram removidos os seguintes tipos complexos:<br/>**cloudPkiAdministratorCredentials**<br/>**windowsNetworkIsolationCloudResource**<br/>**windowsNetworkIsolationCloudResourceCollection**<br/>**windowsNetworkIsolationIPRangeCollection**<br/>**windowsNetworkIsolationResourceCollection**<br/>|
|Alteração|Beta|A propriedade **gracePeriodInMinutes** foi adicionada à entidade [androidDeviceComplianceLocalActionBase](/graph/api/resources/intune-deviceconfig-androiddevicecompliancelocalactionbase?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **enableSplitTunneling** foi removida da entidade [androidForWorkVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkvpnconfiguration?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **versionName** e **versionCode** foram adicionadas à entidade [androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **minimumRequiredPatchVersion** e **minimumWarningPatchVersion** foram adicionadas à entidade [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **minimumRequiredPatchVersion** e **minimumWarningPatchVersion** foram adicionadas à entidade [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **target** foi adicionada à entidade [deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **singleSignOnSettings** foi adicionada à entidade [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **versionNumber** e **buildNumber** foram adicionadas à entidade [iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **bundleId** foi adicionada à entidade [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) |
|Alteração|Beta|A propriedade **preSharedKey** foi adicionada à entidade [iosWiFiConfiguration](/graph/api/resources/intune-deviceconfig-ioswificonfiguration?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **versionName** e **versionCode** foram adicionadas à entidade [managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **periodBeforePinReset** foi adicionada à entidade [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **subscriberCarrier**, **meid**, **totalStorageSpaceInBytes** e **freeStorageSpaceInBytes** foram adicionadas à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **enrollmentType** foi removida da entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **versionNumber** e **buildNumber** foram adicionadas à entidade [managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **displayVersion** foi adicionada à entidade [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **defaultDeviceEnrollmentRestrictions**, **defaultDeviceEnrollmentWindowsHelloForBusinessSettings** e **defaultDeviceEnrollmentLimit** foram removidas da entidade [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **isAssigned** foi adicionada à entidade [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **isAssigned** foi adicionada à entidade [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **activeFirewallRequired**, **uacRequired**, **defenderEnabled**, **defenderVersion**, **signatureOutOfDate** e **rtpEnabled** foram adicionadas à entidade [windows10CompliancePolicy](/graph/api/resources/intune-deviceconfig-windows10compliancepolicy?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **assignedAccessSingleModeUserName**, **assignedAccessSingleModeAppUserModelId**, **microsoftAccountSignInAssistantSettings**, **authenticationAllowSecondaryDevice**, **cryptographyAllowFipsAlgorithmPolicy**, **securityBlockAzureADJoinedDevicesAutoEncryption**, **systemTelemetryProxyServer**, **inkWorkspaceAccess**, **inkWorkspaceBlockSuggestedApps**, **defenderCloudBlockLevel** e **defenderCloudExtendedTimeout** foram adicionadas à entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **protectedApps**, **enterpriseProxiedDomains** e **isAssigned** foram adicionadas à entidade [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta)|
|Alteração|Beta|A propriedade **productVersion** foi adicionada à entidade [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **apps** foi adicionada à entidade [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **apps** foi adicionada à entidade [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **vppTokens** foi adicionada à entidade [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **assignments** foi adicionada à entidade [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **deviceCompliancePolicy** foi removida da entidade [deviceCompliancePolicyAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicyassignment?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **deviceCompliancePolicy** foi removida da entidade [deviceCompliancePolicyGroupAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicygroupassignment?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **identityCertificateForClientAuthentication** foi adicionada à entidade [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **assignments** foi adicionada à entidade [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **apps** foi adicionada à entidade [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **assignments** foi adicionada à entidade [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **assignments** foi adicionada à entidade [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **assignments** foi adicionada à entidade [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **apps** foi adicionada à entidade [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **assignments** foi adicionada à entidade [termsAndConditions](/graph/api/resources/intune-companyterms-termsandconditions?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **assignedAccessMultiModeProfiles** foi adicionada à entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta)|
|Alteração|Beta|A propriedade de navegação **protectedAppLockerFiles** foi adicionada à entidade [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta)|
|Alteração|Beta|As propriedades **port** e **forceTls** foram adicionadas ao tipo complexo [airPrintDestination](/graph/api/resources/intune-deviceconfig-airprintdestination?view=graph-rest-beta)|
|Alteração|Beta|O tipo das seguintes propriedades no tipo complexo [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta) foi alterado:<br/>**errorCode** de Int32 para Int64<br/>|
|Alteração|Beta|O tipo das seguintes propriedades no tipo complexo [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) foi alterado:<br/>**errorCode** de Int32 para Int64<br/>|
|Alteração|Beta|O tipo das seguintes propriedades no tipo complexo [windowsNetworkIsolationPolicy](/graph/api/resources/intune-deviceconfig-windowsnetworkisolationpolicy?view=graph-rest-beta) foi alterado:<br/>**enterpriseCloudResources** de [windowsNetworkIsolationCloudResourceCollection](/graph/api/resources/intune-deviceconfig-windowsnetworkisolationcloudresourcecollection?view=graph-rest-beta) para a coleção [proxiedDomain](/graph/api/resources/intune-deviceconfig-proxieddomain?view=graph-rest-beta)<br/>**enterpriseInternalProxyServers** de windowsNetworkIsolationResourceCollection para a coleção String<br/>**enterpriseIPRanges** de windowsNetworkIsolationIPRangeCollection para a coleção [ipRange](/graph/api/resources/intune-deviceconfig-iprange?view=graph-rest-beta)<br/>**enterpriseNetworkDomainNames** de windowsNetworkIsolationResourceCollection para a coleção String<br/>**enterpriseProxyServers** de windowsNetworkIsolationResourceCollection para a coleção String<br/>**neutralDomainResources** de windowsNetworkIsolationResourceCollection para a coleção String<br/>|

### <a name="microsoft-teams-apis"></a>APIs do Microsoft Teams

|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|Beta|Uma nova entidade [team](/graph/api/resources/team?view=graph-rest-beta) foi adicionada.|
|Adição|Beta|As operações [create](/graph/api/team-put-teams?view=graph-rest-beta), [get](/graph/api/team-get?view=graph-rest-beta) e [update](/graph/api/team-update?view=graph-rest-beta) foram adicionadas à entidade [team](/graph/api/resources/team?view=graph-rest-beta).|

### <a name="outlook-messages"></a>Mensagens do Outlook

| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Alteração          | v1.0 e beta | Esse aprimoramento do comportamento recai sobre a obtenção de uma pasta de emails compartilhada ou do conteúdo das mensagens desta pasta quando um usuário compartilhar uma pasta de email com o usuário conectado ou delegar ou não sua caixa de correio ao usuário conectado. Nesses casos, um aplicativo poderá especificar a identificação desse usuário ou nome da entidade de segurança do usuário para [obter essa pasta de emails compartilhada](/graph/api/mailfolder-get?view=graph-rest-1.0) ou [obter as mensagens desse calendário compartilhado](/graph/api/user-list-messages?view=graph-rest-1.0), desde que o usuário conectado tenha fornecido permissões delegadas ao aplicativo. |


### <a name="outlook-user-choices"></a>Opções de usuário do Outlook

| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
|Adição | Beta | A nova propriedade **workingHours** foi adicionada a [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta). Confira [tipo de recurso workingHours](/graph/api/resources/workinghours?view=graph-rest-beta) para saber mais sobre casos de uso com suporte.|
|Adição | Beta | Os seguintes tipos complexos foram adicionados: <br> [workingHours](/graph/api/resources/workinghours?view=graph-rest-beta) <br> [timeZoneBase](/graph/api/resources/timezonebase?view=graph-rest-beta) <br> [customTimeZone](/graph/api/resources/customtimezone?view=graph-rest-beta) <br> [standardTimeZoneOffset](/graph/api/resources/standardtimezoneoffset?view=graph-rest-beta) <br> [daylightTimeZoneOffset](/graph/api/resources/daylighttimezoneoffset?view=graph-rest-beta)|


### <a name="reports-apis"></a>APIs de relatórios
| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Alteração      | Beta    | As APIs [getEmailActivityUserDetail](/graph/api/reportroot-getemailactivityuserdetail?view=graph-rest-beta), [getEmailActivityCounts](/graph/api/reportroot-getemailactivitycounts?view=graph-rest-beta) e [getEmailActivityUserCounts](/graph/api/reportroot-getemailactivityusercounts?view=graph-rest-beta) foram adicionadas. Essas substituíram a API EmailActivity. |
| Alteração      | Beta    | As APIs [getEmailAppUsageUserDetail](/graph/api/reportroot-getemailappusageuserdetail?view=graph-rest-beta), [getEmailAppUsageAppsUserCounts](/graph/api/reportroot-getemailappusageappsusercounts?view=graph-rest-beta), [getEmailAppUsageUserCounts](/graph/api/reportroot-getemailappusageusercounts?view=graph-rest-beta) e [getEmailAppUsageVersionsUserCounts](/graph/api/reportroot-getemailappusageversionsusercounts?view=graph-rest-beta) foram adicionadas. Essas substituíram a API EmailAppUsage. |
| Alteração      | Beta    | As APIs [getMailboxUsageDetail](/graph/api/reportroot-getmailboxusagedetail?view=graph-rest-beta), [getMailboxUsageMailboxCounts](/graph/api/reportroot-getmailboxusagemailboxcounts?view=graph-rest-beta), [getMailboxUsageQuotaStatusMailboxCounts](/graph/api/reportroot-getmailboxusagequotastatusmailboxcounts?view=graph-rest-beta) e [getMailboxUsageStorage](/graph/api/reportroot-getmailboxusagestorage?view=graph-rest-beta) foram adicionadas. Elas substituíram a API MailboxUsage. |
| Alteração      | Beta    | As APIs [getOffice365ActivationsUserDetail](/graph/api/reportroot-getoffice365activationsuserdetail?view=graph-rest-beta), [getOffice365ActivationCounts](/graph/api/reportroot-getoffice365activationcounts?view=graph-rest-beta) e [getOffice365ActivationsUserCounts](/graph/api/reportroot-getoffice365activationsusercounts?view=graph-rest-beta) foram adicionadas. Essas substituíram a API Office365Activations. |
| Alteração      | Beta    | As APIs [getOffice365ActiveUserDetail](/graph/api/reportroot-getoffice365activeuserdetail?view=graph-rest-beta), [getOffice365ActiveUserCounts](/graph/api/reportroot-getoffice365activeusercounts?view=graph-rest-beta) e [getOffice365ServicesUserCounts](/graph/api/reportroot-getoffice365servicesusercounts?view=graph-rest-beta) foram adicionadas. Essas substituíram a API Office365ActiveUser. |
| Alteração      | Beta    | As APIs [getOffice365GroupsActivityDetail](/graph/api/reportroot-getoffice365groupsactivitydetail?view=graph-rest-beta), [getOffice365GroupsActivityCounts](/graph/api/reportroot-getoffice365groupsactivitycounts?view=graph-rest-beta),[getOffice365GroupsActivityGroupCounts](/graph/api/reportroot-getoffice365groupsactivitygroupcounts?view=graph-rest-beta), [getOffice365GroupsActivityStorage](/graph/api/reportroot-getoffice365groupsactivitystorage?view=graph-rest-beta) e [getOffice365GroupsActivityFileCounts](/graph/api/reportroot-getoffice365groupsactivityfilecounts?view=graph-rest-beta) foram adicionadas. Essas substituíram a API Office365GroupsActivity. |
| Alteração      | Beta    | As APIs [getOneDriveActivityUserDetail](/graph/api/reportroot-getonedriveactivityuserdetail?view=graph-rest-beta), [getOneDriveActivityUserCounts](/graph/api/reportroot-getonedriveactivityusercounts?view=graph-rest-beta) e [getOneDriveActivityFileCounts](/graph/api/reportroot-getonedriveactivityfilecounts?view=graph-rest-beta) foram adicionadas. Essas substituíram a API OneDriveActivity. |
| Alteração      | Beta    | As APIs [getOneDriveUsageAccountDetail](/graph/api/reportroot-getonedriveusageaccountdetail?view=graph-rest-beta), [getOneDriveUsageAccountCounts](/graph/api/reportroot-getonedriveusageaccountcounts?view=graph-rest-beta), [getOneDriveUsageFileCounts](/graph/api/reportroot-getonedriveusagefilecounts?view=graph-rest-beta) e [getOneDriveUsageStorage](/graph/api/reportroot-getonedriveusagestorage?view=graph-rest-beta) foram adicionadas. Essas substituíram a API OneDriveUsage. |
| Alteração      | Beta    | As APIs [getSharePointActivityUserDetail](/graph/api/reportroot-getsharepointactivityuserdetail?view=graph-rest-beta), [getSharePointActivityFileCounts](/graph/api/reportroot-getsharepointactivityfilecounts?view=graph-rest-beta), [getSharePointActivityUserCounts](/graph/api/reportroot-getsharepointactivityusercounts?view=graph-rest-beta) e [getSharePointActivityPages](/graph/api/reportroot-getsharepointactivitypages?view=graph-rest-beta) foram adicionadas. Essas substituíram a API SharePointActivity. |
| Alteração      | Beta    | As APIs [getSharePointSiteUsageDetail](/graph/api/reportroot-getsharepointsiteusagedetail?view=graph-rest-beta), [getSharePointSiteUsageFileCounts](/graph/api/reportroot-getsharepointsiteusagefilecounts?view=graph-rest-beta), [getSharePointSiteUsageSiteCounts](/graph/api/reportroot-getsharepointsiteusagesitecounts?view=graph-rest-beta), [getSharePointSiteUsageStorage](/graph/api/reportroot-getsharepointsiteusagestorage?view=graph-rest-beta) e [getSharePointSiteUsagePages](/graph/api/reportroot-getsharepointsiteusagepages?view=graph-rest-beta) foram adicionadas. Essas substituíram a API SharePointSiteUsage. |
| Alteração      | Beta    | As APIs [getSkypeForBusinessActivityUserDetail](/graph/api/reportroot-getskypeforbusinessactivityuserdetail?view=graph-rest-beta), [getSkypeForBusinessActivityCounts](/graph/api/reportroot-getskypeforbusinessactivitycounts?view=graph-rest-beta) e [getSkypeForBusinessActivityUserCounts](/graph/api/reportroot-getskypeforbusinessactivityusercounts?view=graph-rest-beta) foram adicionadas. Essas substituíram a API SfbActivity. |
| Alteração      | Beta    | As APIs [getSkypeForBusinessDeviceUsageUserDetail](/graph/api/reportroot-getskypeforbusinessdeviceusageuserdetail?view=graph-rest-beta), [getSkypeForBusinessDeviceUsageDistributionUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts?view=graph-rest-beta), e [getSkypeForBusinessDeviceUsageUserCounts](/graph/api/reportroot-getskypeforbusinessdeviceusageusercounts?view=graph-rest-beta) foram adicionadas. Essas substituíram a API SfbDeviceUsage. |
| Alteração      | Beta    | As APIs [getSkypeForBusinessOrganizerActivityCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivitycounts?view=graph-rest-beta), [getSkypeForBusinessOrganizerActivityUserCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityusercounts?view=graph-rest-beta) e [getSkypeForBusinessOrganizerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessorganizeractivityminutecounts?view=graph-rest-beta) foram adicionadas. Essas substituíram a API SfbOrganizerActivity. |
| Alteração      | Beta    | As APIs [getSkypeForBusinessParticipantActivityCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivitycounts?view=graph-rest-beta), [getSkypeForBusinessParticipantActivityUserCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityusercounts?view=graph-rest-beta) e [getSkypeForBusinessParticipantActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinessparticipantactivityminutecounts?view=graph-rest-beta) foram adicionadas. Essas substituíram a API SfbParticipantActivity. |
| Alteração      | Beta    | As APIs [getSkypeForBusinessPeerToPeerActivityCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivitycounts?view=graph-rest-beta), [getSkypeForBusinessPeerToPeerActivityUserCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityusercounts?view=graph-rest-beta) e [getSkypeForBusinessPeerToPeerActivityMinuteCounts](/graph/api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts?view=graph-rest-beta) foram adicionadas. Essas substituíram a API SfbP2PActivity. |
| Alteração      | Beta    | As APIs [getYammerActivityUserDetail](/graph/api/reportroot-getyammeractivityuserdetail?view=graph-rest-beta), [getYammerActivityCounts](/graph/api/reportroot-getyammeractivitycounts?view=graph-rest-beta) e [getYammerActivityUserCounts](/graph/api/reportroot-getyammeractivityusercounts?view=graph-rest-beta) foram adicionadas. Essas substituíram a API YammerActivity. |
| Alteração      | Beta    | As APIs [getYammerDeviceUsageUserDetail](/graph/api/reportroot-getyammerdeviceusageuserdetail?view=graph-rest-beta), [getYammerDeviceUsageDistributionUserCounts](/graph/api/reportroot-getyammerdeviceusagedistributionusercounts?view=graph-rest-beta) e [getYammerDeviceUsageUserCounts](/graph/api/reportroot-getyammerdeviceusageusercounts?view=graph-rest-beta) foram adicionadas. Essas substituíram a API YammerDeviceUsage. |
| Alteração      | Beta    | As APIs [getYammerGroupsActivityDetail](/graph/api/reportroot-getyammergroupsactivitydetail?view=graph-rest-beta), [getYammerGroupsActivityGroupCounts](/graph/api/reportroot-getyammergroupsactivitygroupcounts?view=graph-rest-beta) e [getYammerGroupsActivityCounts](/graph/api/reportroot-getyammergroupsactivitycounts?view=graph-rest-beta) foram adicionadas. Essas substituíram a API YammerGroupsActivity. |



## <a name="september-2017"></a>Setembro de 2017

### <a name="intune-apis"></a>APIs do Intune

| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Adição    | Beta    | Foram adicionadas novas entidades:<br/>[activeDirectoryWindowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-activedirectorywindowsautopilotdeploymentprofile?view=graph-rest-beta)<br/>[azureADWindowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-azureadwindowsautopilotdeploymentprofile?view=graph-rest-beta)<br/>[deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-beta)<br/>[deviceEnrollmentLimitConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentlimitconfiguration?view=graph-rest-beta)<br/>[deviceEnrollmentPlatformRestrictionsConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration?view=graph-rest-beta)<br/>[deviceEnrollmentWindowsHelloForBusinessConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration?view=graph-rest-beta)<br/>[deviceManagementPartner](/graph/api/resources/intune-onboarding-devicemanagementpartner?view=graph-rest-beta)<br/>[enrollmentConfigurationAssignment](/graph/api/resources/intune-onboarding-enrollmentconfigurationassignment?view=graph-rest-beta)<br/>[windows10EnrollmentCompletionPageConfiguration](/graph/api/resources/intune-onboarding-windows10enrollmentcompletionpageconfiguration?view=graph-rest-beta)<br/>[windows10NetworkBoundaryConfiguration](/graph/api/resources/intune-deviceconfig-windows10networkboundaryconfiguration?view=graph-rest-beta)<br/>[windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta)<br/>[windowsAutopilotDeviceIdentity](/graph/api/resources/intune-enrollment-windowsautopilotdeviceidentity?view=graph-rest-beta)<br/>[windowsAutopilotSettings](/graph/api/resources/intune-enrollment-windowsautopilotsettings?view=graph-rest-beta)<br/> |
| Adição    | Beta    | Foram adicionados novos tipos complexos:<br/>[adminConsent](/graph/api/resources/intune-devices-adminconsent?view=graph-rest-beta)<br/>[allDevicesAssignmentTarget](/graph/api/resources/intune-shared-alldevicesassignmenttarget?view=graph-rest-beta)<br/>[allLicensedUsersAssignmentTarget](/graph/api/resources/intune-shared-alllicensedusersassignmenttarget?view=graph-rest-beta)<br/>[deviceAndAppManagementAssignmentTarget](/graph/api/resources/intune-shared-deviceandappmanagementassignmenttarget?view=graph-rest-beta)<br/>[deviceEnrollmentPlatformRestriction](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestriction?view=graph-rest-beta)<br/>[deviceHealthAttestationState](/graph/api/resources/intune-devices-devicehealthattestationstate?view=graph-rest-beta)<br/>[exclusionGroupAssignmentTarget](/graph/api/resources/intune-shared-exclusiongroupassignmenttarget?view=graph-rest-beta)<br/>[groupAssignmentTarget](/graph/api/resources/intune-shared-groupassignmenttarget?view=graph-rest-beta)<br/>[outOfBoxExperienceSettings](/graph/api/resources/intune-enrollment-outofboxexperiencesettings?view=graph-rest-beta)<br/>[windowsFirewallNetworkProfile](/graph/api/resources/intune-deviceconfig-windowsfirewallnetworkprofile?view=graph-rest-beta)<br/>windowsNetworkIsolationCloudResource<br/>windowsNetworkIsolationCloudResourceCollection<br/>windowsNetworkIsolationIPRangeCollection<br/>[windowsNetworkIsolationPolicy](/graph/api/resources/intune-deviceconfig-windowsnetworkisolationpolicy?view=graph-rest-beta)<br/>windowsNetworkIsolationResourceCollection<br/> |
| Adição    | Beta    | A ação [sync](/graph/api/intune-enrollment-windowsautopilotsettings-sync?view=graph-rest-beta) em [windowsAutopilotSettings](/graph/api/resources/intune-enrollment-windowsautopilotsettings?view=graph-rest-beta) foi adicionada |
| Adição    | Beta    | A ação [assign](/graph/api/intune-enrollment-windowsautopilotdeploymentprofile-assign?view=graph-rest-beta) em [windowsAutopilotDeploymentProfile](/graph/api/resources/intune-enrollment-windowsautopilotdeploymentprofile?view=graph-rest-beta) foi adicionada |
| Adição    | Beta    | Foi adicionada a ação localActions a [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) |
| Adição    | Beta    | A ação [setPriority](/graph/api/intune-onboarding-deviceenrollmentconfiguration-setpriority?view=graph-rest-beta) foi adicionada a [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-beta) |
| Adição    | Beta    | A ação [assign](/graph/api/intune-onboarding-deviceenrollmentconfiguration-assign?view=graph-rest-beta) foi adicionada a [deviceEnrollmentConfiguration](/graph/api/resources/intune-onboarding-deviceenrollmentconfiguration?view=graph-rest-beta) |
| Adição    | Beta    | A ação uploadDepToken na coleção [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) foi adicionada |
| Adição    | Beta    | A ação syncWithAppleDeviceEnrollmentProgram action na coleção [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) foi adicionada |
| Adição    | Beta    | A ação updateMobileAppIdentifierDeployments em [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) foi adicionada |
| Adição    | Beta    | A ação assign foi adicionada a [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta) |
| Adição    | Beta    | A ação assign foi adicionada a [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) |
| Adição    | Beta    | A ação assign foi adicionada a [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) |
| Adição    | Beta    | A função getEncryptionPublicKey na coleção [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) foi adicionada |
| Alteração      | Beta    | As propriedades **requireSafetyNetAttestationBasicIntegrity**, **requireSafetyNetAttestationCertifiedDevice**, **requireGooglePlayServices**, **requireUpToDateSecurityProviders**, **requireCompanyPortalAppIntegrity** e **conditionStatementId** foram adicionadas à entidade [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **requireAppVerify**, **requireSafetyNetAttestationBasicIntegrity**, **requireSafetyNetAttestationCertifiedDevice**, **requireGooglePlayServices**, **requireUpToDateSecurityProviders** e **requireCompanyPortalAppIntegrity** foram adicionadas à entidade [androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **blockCrossProfileCopyPaste** e **requireAppVerify** foram adicionadas à entidade [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **kioskModeApps** e **requireAppVerify** foram adicionadas à entidade [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Remoção da propriedade **kioskModeManagedApps** da entidade [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Remoção das propriedades **cloudPkiProvider**, **createdDateTime**, **description**, **lastModifiedDateTime**, **displayName**, **syncStatus**, **lastSyncError**, **lastSyncDateTime**, **credentials**, **trustedRootCertificate** e **version** da entidade cloudPkiSubscription |
| Alteração      | Beta    | Remoção das propriedades **assignmentStatus**, **assignmentProgress** e **assignmentErrorMessage** da entidade [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **adminConsent** foi adicionada à entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **vppTokenOrganizationName**, **vppTokenAccountType** e **vppTokenAppleId** foram adicionadas à entidade [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **deviceEnrollmentType**, **wiFiMacAddress** e **deviceHealthAttestationState** foram adicionadas à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **legacyAppConfiguration** foi adicionada à entidade [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **notApplicableCount** foi adicionada à entidade [managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **notApplicableCount** foi adicionada à entidade [managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **firewallBlockStatefulFTP**, **firewallIdleTimeoutForSecurityAssociationInSeconds**, **firewallPreSharedKeyEncodingMethod**, **firewallIPSecExemptionsAllowNeighborDiscovery**, **firewallIPSecExemptionsAllowICMP**, **firewallIPSecExemptionsAllowRouterDiscovery**, **firewallIPSecExemptionsAllowDHCP**, **firewallCertificateRevocationListCheckMethod**, **firewallMergeKeyingModuleSettings**, **firewallPacketQueueingMethod**, **firewallProfileDomain**, **firewallProfilePublic**, **firewallProfilePrivate**, **defenderAttackSurfaceReductionExcludedPaths**, **defenderOfficeAppsOtherProcessInjectionType**, **defenderOfficeAppsExecutableContentCreationOrLaunchType**, **defenderOfficeAppsLaunchChildProcessType**, **defenderOfficeMacroCodeAllowWin32ImportsType**, **defenderScriptObfuscatedMacroCodeType**, **defenderScriptDownloadedPayloadExecutionType**, **defenderEmailContentExecutionType**, **defenderGuardMyFoldersType**, **defenderGuardedFoldersAllowedAppPaths**, **defenderAdditionalGuardedFolders**, **defenderNetworkProtectionType**, **defenderExploitProtectionXml**, **defenderExploitProtectionXmlFileName**, **defenderSecurityCenterBlockExploitProtectionOverride**, **appLockerApplicationControl**, **applicationGuardBlockClipboardSharing**, **applicationGuardAllowPrintToPDF**, **applicationGuardAllowPrintToXPS**, **applicationGuardAllowPrintToLocalPrinters**, **applicationGuardAllowPrintToNetworkPrinters** and **bitLockerDisableWarningForOtherDiskEncryption** foram adicionadas à entidade [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **displayAppListWithGdiDPIScalingTurnedOn**, **displayAppListWithGdiDPIScalingTurnedOff**, **messagingBlockSync**, **messagingBlockMMS** e **messagingBlockRichCommunicationServices** foram adicionadas à entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Remoção da propriedade **bluetoothDeviceName** da entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Remoção das propriedades **deviceAccountBlockExchangeServices**, **deviceAccountEmailAddress**, **deviceAccountExchangeServerAddress**, **deviceAccountRequirePasswordRotation** and **deviceAccountSessionInitiationProtocolAddress** da entidade [windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **localActions** foi adicionada à entidade [androidCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidcompliancepolicy?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades de navegação **windowsAutopilotSettings**, **windowsAutopilotDeviceIdentities**, **windowsAutopilotDeploymentProfiles**, **deviceEnrollmentConfigurations**, **deviceManagementPartners** e **depOnboardingSettings** foram adicionadas à entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) |
| Alteração      | Beta    | Remoção da propriedade de navegação **cloudPkiSubscriptions** da entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **assignments** foi adicionada à entidade [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **assignments** foi adicionada à entidade [targetedManagedAppProtection](/graph/api/resources/intune-mam-targetedmanagedappprotection?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **assignments** foi adicionada à entidade [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) |

### <a name="onedrive"></a>OneDrive

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | A propriedade **system** foi adicionada ao recurso [Drive][]. |
| Adição        | v1.0        | A relação **list** foi adicionada ao recurso [Drive][]. |
| Adição        | v1.0        | A relação **listItem** foi adicionada ao recurso [DriveItem][]. |
| Adição        | v1.0        | As relações **list** e **listItem** foram adicionadas ao recurso [SharedDriveItem][]. |
| Adição        | v1.0        | Foram adicionados novos tipos complexos: [FolderView][]  |
| Adição        | v1.0        | A propriedade **view** foi adicionada ao tipo complexo [Folder][]. |
| Adição        | v1.0        | A propriedade **driveType** foi adicionada ao tipo complexo [ItemReference][]. |
| Adição        | v1.0        | As propriedades **audioBitsPerSample**, **audioChannels**, **audioFormat**, **audioSamplesPerSecond**, **fourCC** e **frameRate** foram adicionadas ao tipo complexo [Video][]. |
| Adição        | beta        | A propriedade **system** foi adicionada ao recurso [Drive][Drive-beta]. |
| Adição        | beta        | A relação **activities** foi adicionada ao recurso [Drive][Drive-beta]. |
| Adição        | beta        | A propriedade **publication** foi adicionada ao recurso [DriveItem][DriveItem-beta]. |
| Adição        | beta        | As relações **activities** e **versions** foram adicionadas ao recurso [DriveItem][DriveItem-beta]. |
| Adição        | beta        | Foram adicionadas novas entidades: [DriveItemVersion][DriveItemVersion-beta], [ItemActivity][ItemActivity-beta]. |
| Adição        | beta        | Foram adicionados novos tipos complexos: [CommentAction][CommentAction-beta], [CreateAction][CreateAction-beta], [DeleteAction][DeleteAction-beta], [EditAction][EditAction-beta], [ItemActionSet][ItemActionSet-beta], [ItemActivityTimeSet][ItemActivityTimeSet-beta], [MentionAction][MentionAction-beta], [MoveAction][MoveAction-beta], [PublicationFacet][PublicationFacet-beta], [RenameAction][RenameAction-beta], [RestoreAction][RestoreAction-beta], [ShareAction][ShareAction-beta] e [VersionAction][VersionAction-beta]. |
| Adição        | beta        | A propriedade **driveType** foi adicionada ao tipo complexo [ItemReference][ItemReference-beta]. |
| Exclusão        | beta        | Remoção da propriedade **tenantId** do tipo complexo [SharepointIds][SharepointIds-beta]. |
| Adição        | v1.0        | As propriedades **audioBitsPerSample**, **audioChannels**, **audioFormat**, **audioSamplesPerSecond**, **fourCC** e **frameRate** foram adicionadas ao tipo complexo [Video][Video-beta]. |
| Adição        | beta        | As ações [CheckIn][CheckIn-beta] e [CheckOut][CheckOut-beta] foram adicionadas ao recurso [DriveItem][DriveItem-beta]. |
| Adição        | beta        | As propriedades **expirationDateTime**, **password**, **message** e **recipients** na ação [CreateLink][CreateLink-beta] foram adicionadas ao recurso [DriveItem][DriveItem-beta]. |

[Drive]: /graph/api/resources/drive?view=graph-rest-1.0
[DriveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[SharedDriveItem]: /graph/api/resources/shareddriveitem?view=graph-rest-1.0
[FolderView]: /graph/api/resources/folderview?view=graph-rest-1.0
[Folder]: /graph/api/resources/folder?view=graph-rest-1.0
[ItemReference]: /graph/api/resources/itemreference?view=graph-rest-1.0
[Video]: /graph/api/resources/video?view=graph-rest-1.0
[Drive-beta]: /graph/api/resources/drive?view=graph-rest-beta
[DriveItem-beta]: /graph/api/resources/driveitem?view=graph-rest-beta
[DriveItemVersion-beta]: /graph/api/resources/driveitemversion?view=graph-rest-beta
[ItemActivity-beta]: /graph/api/resources/itemactivity?view=graph-rest-beta
[CommentAction-beta]: /graph/api/resources/commentaction?view=graph-rest-beta
[CreateAction-beta]: /graph/api/resources/createaction?view=graph-rest-beta
[DeleteAction-beta]: /graph/api/resources/deleteaction?view=graph-rest-beta
[EditAction-beta]: /graph/api/resources/editaction?view=graph-rest-beta
[ItemActionSet-beta]: /graph/api/resources/itemactionset?view=graph-rest-beta
[ItemActivityTimeSet-beta]: /graph/api/resources/itemactivitytimeset?view=graph-rest-beta
[MentionAction-beta]: /graph/api/resources/mentionaction?view=graph-rest-beta
[MoveAction-beta]: /graph/api/resources/moveaction?view=graph-rest-beta
[PublicationFacet-beta]: /graph/api/resources/publicationfacet?view=graph-rest-beta
[RenameAction-beta]: /graph/api/resources/renameaction?view=graph-rest-beta
[RestoreAction-beta]: /graph/api/resources/restoreaction?view=graph-rest-beta
[ShareAction-beta]: /graph/api/resources/shareaction?view=graph-rest-beta
[VersionAction-beta]: /graph/api/resources/versionaction?view=graph-rest-beta
[ItemReference-beta]: /graph/api/resources/itemreference?view=graph-rest-beta
[SharepointIds-beta]: /graph/api/resources/sharepointids?view=graph-rest-beta
[Video-beta]: /graph/api/resources/video?view=graph-rest-beta
[CheckIn-beta]: /graph/api/driveitem-checkin?view=graph-rest-beta
[CheckOut-beta]: /graph/api/driveitem-checkout?view=graph-rest-beta
[CreateLink-beta]: /graph/api/driveitem-createlink?view=graph-rest-beta


### <a name="outlook-calendar"></a>Calendário do Outlook

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | Beta          | As funções [findRoomLists](/graph/api/user-findroomlists?view=graph-rest-beta) e [findRooms](/graph/api/user-findrooms?view=graph-rest-beta) foram adicionadas à entidade [user](/graph/api/resources/user?view=graph-rest-beta). |
| Adição        | Beta          | A propriedade **locations** foi adicionada à entidade [event](/graph/api/resources/event?view=graph-rest-beta) para dar suporte à organização de um evento em que os participantes podem participar de mais de um local. |
| Adição        | Beta          | A propriedade **locationType** foi adicionada ao tipo complexo [location](/graph/api/resources/location?view=graph-rest-beta). |
| Adição        | Beta          | As propriedades **uniqueId** e **uniqueIdType** foram adicionadas ao tipo complexo [location](/graph/api/resources/location?view=graph-rest-beta). Atualmente, essas propriedades são apenas para uso interno. |
| Alteração          | v1.0 e beta | Esse aprimoramento do comportamento recai sobre a obtenção de um calendário compartilhado ou do conteúdo dos eventos deste calendário quando um usuário compartilhar um calendário com o usuário conectado ou delegar ou não sua caixa de correio ao usuário conectado. Nesses casos, um aplicativo poderá especificar a identificação desse usuário ou nome da entidade de segurança do usuário para [obter esse calendário compartilhado](/graph/api/calendar-get?view=graph-rest-1.0) ou [obter os eventos desse calendário compartilhado](/graph/api/user-list-events?view=graph-rest-1.0), desde que o usuário conectado tenha fornecido permissões delegadas ao aplicativo. |

### <a name="outlook-contacts"></a>Contatos do Outlook

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Alteração          | v1.0 e beta | Esse aprimoramento do comportamento recai sobre a obtenção de uma pasta de contatos compartilhada ou do conteúdo dos contatos desta pasta quando um usuário compartilhar uma pasta de contatos com o usuário conectado ou delegar ou não sua caixa de correio ao usuário conectado. Nesses casos, um aplicativo poderá especificar a identificação desse usuário ou nome da entidade de segurança do usuário para [obter essa pasta de contatos compartilhada](/graph/api/contactfolder-get?view=graph-rest-1.0) ou [obter os contatos dessa pasta compartilhada](/graph/api/user-list-contacts?view=graph-rest-1.0), desde que o usuário conectado tenha fornecido permissões delegadas ao aplicativo. |

### <a name="outlook-mail"></a>Email do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | A propriedade **internetMessageHeaders** foi adicionada à entidade [message](/graph/api/resources/message?view=graph-rest-beta). |
| Adição        | Beta        | O tipo complexo [internetMessageHeader](/graph/api/resources/internetmessageheader?view=graph-rest-beta) foi adicionado. |
| Adição        | Beta        | A propriedade de navegação **messageRules** foi adicionada à entidade [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-beta). **messageRules** é uma coleção das instâncias [messageRule](/graph/api/resources/messagerule?view=graph-rest-beta). |
| Adição        | Beta        | A entidade [messageRule](/graph/api/resources/messagerule?view=graph-rest-beta) e os tipos complexos [messageRuleActions](/graph/api/resources/messageruleactions?view=graph-rest-beta), [messageRulePredicates](/graph/api/resources/messagerulepredicates?view=graph-rest-beta) e [sizeRange](/graph/api/resources/sizerange?view=graph-rest-beta) foram adicionados. |
| Adição        | Beta        | As seguintes operações CRUD às regras de mensagem foram adicionadas: [create](/graph/api/mailfolder-post-messagerules?view=graph-rest-beta), [list](/graph/api/mailfolder-list-messagerules?view=graph-rest-beta), [get](/graph/api/messagerule-get?view=graph-rest-beta), [update](/graph/api/messagerule-update?view=graph-rest-beta) e [delete](/graph/api/messagerule-delete?view=graph-rest-beta). |


### <a name="outlook-user-choices"></a>Opções de usuário do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | A nova propriedade de navegação **masterCategories** foi adicionada à entidade [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-beta). **masterCategories** é uma coleção de objetos [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-beta). |
| Adição        | Beta        | A entidade [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-beta) foi adicionada. |
| Adição        | Beta        | As seguintes operações CRUD para [outlookCategory](/graph/api/resources/outlookcategory?view=graph-rest-beta) foram adicionadas: [create](/graph/api/outlookuser-post-mastercategories?view=graph-rest-beta), [get](/graph/api/outlookcategory-get?view=graph-rest-beta), [update](/graph/api/outlookcategory-update?view=graph-rest-beta) e [delete](/graph/api/outlookcategory-delete?view=graph-rest-beta). |
| Adição        | Beta        | A nova função [supportedLanguages](/graph/api/outlookuser-supportedlanguages?view=graph-rest-beta) foi adicionada à entidade [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-beta). |
| Adição        | Beta        | A nova função [supportedTimeZones](/graph/api/outlookuser-supportedtimezones?view=graph-rest-beta) foi adicionada à entidade [outlookUser](/graph/api/resources/outlookuser?view=graph-rest-beta). |


### <a name="sharepoint-lists"></a>Listas do SharePoint

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Foram adicionadas novas entidades: [ColumnDefinition][], [ColumnLink][], [ContentType][], [List][], [ListItem][]. |
| Adição        | v1.0        | As relações **columns**, **contentTypes**, **items** e **lists** foram adicionadas ao recurso [Site][]. |
| Adição        | v1.0        | Foram adicionados novos tipos complexos: [BooleanColumn][], [CalculatedColumn][], [ChoiceColumn][], [ContentTypeInfo][], [ContentTypeOrder][], [CurrencyColumn][], [DateTimeColumn][], [DefaultColumnValue][], [ListInfo][], [LookupColumn][], [NumberColumn][], [PersonOrGroupColumn][], [SystemFacet][], [TextColumn][]. |
| Adição        | beta        | Foram adicionadas novas entidades: [BaseItemVersion][BaseItemVersion-beta], [ColumnLink][ColumnLink-beta], [ContentType][ContentType-beta], [ListItemVersion][ListItemVersion-beta], |
| Adição        | beta        | As propriedades **columnGroup**, **currency**, **defaultValue** e **displayName** foram adicionadas à [ColumnDefinition][ColumnDefinition-beta]. |
| Adição        | beta        | As propriedades **displayName** e **system** foram adicionadas ao recurso [List][List-beta]. |
| Adição        | beta        | As relações **activities** e **contentTypes** foram adicionadas ao recurso [List][List-beta]. |
| Adição        | beta        | As propriedade **contentType** foram adicionadas ao recurso [ListItem][ListItem-beta]. |
| Adição        | beta        | As relações **activities** e **versions** foram adicionadas ao recurso [ListItem][ListItem-beta]. |
| Adição        | beta        | A relação **contentTypes** foi adicionada ao recurso [Site][Site-beta]. |
| Adição        | beta        | A propriedade **outputType** foi adicionada ao tipo [BooleanColumn][BooleanColumn-beta]. |
| Adição        | beta        | Foram adicionados novos tipos complexos: [ContentTypeInfo][ContentTypeInfo-beta], [ContentTypeOrder][ContentTypeOrder-beta], [CurrencyColumn][CurrencyColumn-beta] e [SystemFacet][SystemFacet-beta]. |
| Adição        | beta        | A propriedade **contentTypesEnabled** foi adicionada ao tipo complexo [ListInfo][ListInfo-beta]. |
| Adição        | beta        | A propriedade **allowUnlimitedLength** foi adicionada ao tipo complexo [LookupColumn][LookupColumn-beta]. |
| Alteração          | beta        | Renomeação da propriedade **allowMultipleValue** para **allowMultipleValues** no tipo complexo [LookupColumn][LookupColumn-beta]. |
| Alteração          | beta        | Renomeação da propriedade **chooseFrom** para **chooseFromType** no tipo complexo [PersonOrGroupColumn][PersonOrGroupColumn-beta]. |
| Exclusão        | beta        | Remoção da propriedade **locale** no tipo complexo [NumberColumn][NumberColumn-beta]. |
| Exclusão        | beta        | Remoção da propriedade **enforceUniqueValues** do tipo complexo [PersonOrGroupColumn][PersonOrGroupColumn-beta]. |

[BaseItemVersion-beta]: /graph/api/resources/baseitemversion?view=graph-rest-beta
[BooleanColumn-beta]:  /graph/api/resources/booleanColumn?view=graph-rest-beta
[BooleanColumn]: /graph/api/resources/booleancolumn?view=graph-rest-1.0
[CalculatedColumn]: /graph/api/resources/calculatedcolumn?view=graph-rest-1.0
[ChoiceColumn]: /graph/api/resources/choicecolumn?view=graph-rest-1.0
[ColumnDefinition-beta]: /graph/api/resources/columndefinition?view=graph-rest-beta
[ColumnDefinition]: /graph/api/resources/columndefinition?view=graph-rest-1.0
[ColumnLink-beta]: /graph/api/resources/columnlink?view=graph-rest-beta
[ColumnLink]: /graph/api/resources/columnlink?view=graph-rest-1.0
[ContentType-beta]: /graph/api/resources/contenttype?view=graph-rest-beta
[ContentType]: /graph/api/resources/contenttype?view=graph-rest-1.0
[ContentTypeInfo-beta]: /graph/api/resources/contenttypeinfo?view=graph-rest-beta
[ContentTypeInfo]: /graph/api/resources/contenttypeinfo?view=graph-rest-1.0
[ContentTypeOrder-beta]: /graph/api/resources/contenttypeorder?view=graph-rest-beta
[ContentTypeOrder]: /graph/api/resources/contenttypeorder?view=graph-rest-1.0
[CurrencyColumn-beta]: /graph/api/resources/currencycolumn?view=graph-rest-beta
[CurrencyColumn]: /graph/api/resources/currencycolumn?view=graph-rest-1.0
[DateTimeColumn]: /graph/api/resources/datetimecolumn?view=graph-rest-1.0
[DefaultColumnValue]: /graph/api/resources/defaultcolumnvalue?view=graph-rest-1.0
[List-beta]: /graph/api/resources/list?view=graph-rest-beta
[List]: /graph/api/resources/list?view=graph-rest-1.0
[ListInfo-beta]: /graph/api/resources/listinfo?view=graph-rest-beta
[ListInfo]: /graph/api/resources/listinfo?view=graph-rest-1.0
[ListItem-beta]: /graph/api/resources/listitem?view=graph-rest-beta
[ListItem]: /graph/api/resources/listitem?view=graph-rest-1.0
[ListItemVersion-beta]: /graph/api/resources/listitemversion?view=graph-rest-beta
[LookupColumn-beta]: /graph/api/resources/lookupcolumn?view=graph-rest-beta
[LookupColumn]: /graph/api/resources/lookupcolumn?view=graph-rest-1.0
[NumberColumn-beta]: /graph/api/resources/numbercolumn?view=graph-rest-beta
[NumberColumn]: /graph/api/resources/numbercolumn?view=graph-rest-1.0
[PersonOrGroupColumn-beta]: /graph/api/resources/personorgroupcolumn?view=graph-rest-beta
[PersonOrGroupColumn]: /graph/api/resources/personorgroupcolumn?view=graph-rest-1.0
[Site-beta]: /graph/api/resources/site?view=graph-rest-beta
[Site]: /graph/api/resources/site?view=graph-rest-1.0
[SystemFacet-beta]: /graph/api/resources/systemfacet?view=graph-rest-beta
[SystemFacet]: /graph/api/resources/systemfacet?view=graph-rest-1.0
[TextColumn]: /graph/api/resources/textcolumn?view=graph-rest-1.0


### <a name="sharepoint-sites"></a>Sites do SharePoint

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | beta        | As propriedades **dataLocationCode** e **root** foram adicionadas ao tipo complexo [SiteCollection][SiteCollection-beta]. |

[SiteCollection-beta]: /graph/api/resources/sitecollection?view=graph-rest-beta


## <a name="august-2017"></a>Agosto de 2017

### <a name="group-lifecycle-policy"></a>Política de ciclo de vida de grupo

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Adicionada a entidade [groupLifecyclePolicy](/graph/api/resources/grouplifecyclepolicy?view=graph-rest-beta). |
| Adição        | Beta        | Adicionadas as seguintes APIs de política de ciclo de vida de grupo: [criar](/graph/api/grouplifecyclepolicy-post-grouplifecyclepolicies?view=graph-rest-beta), [listar](/graph/api/grouplifecyclepolicy-list?view=graph-rest-beta), [obter](/graph/api/grouplifecyclepolicy-get?view=graph-rest-beta), [atualizar](/graph/api/grouplifecyclepolicy-update?view=graph-rest-beta), [excluir](/graph/api/grouplifecyclepolicy-delete?view=graph-rest-beta), [adicionar grupo](/graph/api/grouplifecyclepolicy-addgroup?view=graph-rest-beta), [remover grupo](/graph/api/grouplifecyclepolicy-removegroup?view=graph-rest-beta) e [renovar um grupo](/graph/api/grouplifecyclepolicy-renewgroup?view=graph-rest-beta). |
| Adição        | Beta        | Adicionada a função [Listar groupLifecylePolicies](/graph/api/group-list-grouplifecyclepolicies?view=graph-rest-beta) à entidade [grupo](/graph/api/resources/group?view=graph-rest-beta). |

### <a name="intune-apis"></a>APIs do Intune
| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Adição    | Beta    | Foi adicionada uma nova entidade:<br/>[windowsPrivacyDataAccessControlItem](/graph/api/resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem?view=graph-rest-beta)<br/> |
| Adição    | Beta    | Foram adicionados novos tipos complexos:<br/>[configurationManagerClientEnabledFeatures](/graph/api/resources/intune-devices-configurationmanagerclientenabledfeatures?view=graph-rest-beta)<br/>[windowsDefenderScanActionResult](/graph/api/resources/intune-devices-windowsdefenderscanactionresult?view=graph-rest-beta)<br/> |
| Adição    | Beta    | A ação [windowsDefenderScan](/graph/api/intune-devices-manageddevice-windowsdefenderscan?view=graph-rest-beta) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Adição    | Beta    | A ação [windowsDefenderUpdateSignatures](/graph/api/intune-devices-manageddevice-windowsdefenderupdatesignatures?view=graph-rest-beta) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Adição    | Beta    | A ação [windowsPrivacyAccessControls](/graph/api/intune-deviceconfig-deviceconfiguration-windowsprivacyaccesscontrols?view=graph-rest-beta) foi adicionada a [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **automaticallyUpdateApps** e **countryOrRegion** à entidade [appleVolumePurchaseProgramToken](/graph/api/resources/intune-apps-applevolumepurchaseprogramtoken?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **enableAuthenticationViaCompanyPortal** foi adicionada à entidade [depEnrollmentProfile](/graph/api/resources/intune-corpenrollment-depenrollmentprofile?view=graph-rest-beta) |
| Alteração      | Beta    | Adicionada a propriedade **notificationMessageCCList** à entidade [deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **notApplicableCount** foi adicionada à entidade [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **notApplicableCount** foi adicionada à entidade [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **notApplicableCount** foi adicionada à entidade [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **notApplicableCount** foi adicionada à entidade [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **configurationManagerClientEnabledFeatures** foi adicionada à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Alteração      | Beta    | Foi removida a propriedade **intuneBrand** da entidade [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **smartScreenEnableInShell**, **smartScreenBlockOverrideForFiles**, **applicationGuardEnabled**, **applicationGuardBlockFileTransfer**, **applicationGuardBlockNonEnterpriseContent**, **applicationGuardAllowPersistence** e **applicationGuardForceAuditing** à entidade [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **searchBlockDiacritics**, **searchDisableAutoLanguageDetection**, **searchDisableIndexingEncryptedItems**, **searchEnableRemoteQueries**, **searchDisableUseLocation**, **searchDisableIndexerBackoff**, **searchDisableIndexingRemovableDrive**, **searchEnableAutomaticIndexSizeManangement**, **smartScreenEnableAppInstallControl** e **privacyAdvertisingId** à entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foi removida a propriedade **settingsDeviceName** da entidade [windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foi removida a propriedade **restartMode** da entidade [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **detectedApps** e **managedDevices** à entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **privacyAccessControls** foi adicionada à entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **secureByDefault** foi adicionada ao tipo complexo [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **restartMode** foi adicionada ao tipo complexo [windowsUpdateScheduledInstall](/graph/api/resources/intune-deviceconfig-windowsupdatescheduledinstall?view=graph-rest-beta) |

### <a name="onenote"></a>OneNote

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0 e Beta | Adicionou a propriedade de navegação [onenote](/graph/api/resources/onenote?view=graph-rest-1.0) a **site**. |
| Adição        | Beta          | Adicionou os parâmetros de destino *siteCollectionId* e *siteId* para as operações de cópia. Por exemplo: [CopyNotebook](/graph/api/notebook-copynotebook?view=graph-rest-1.0). |

### <a name="people"></a>Pessoas

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Adicionada a [API de Pessoas](/graph/api/resources/person?view=graph-rest-1.0) à versão 1.0. Para obter dados sobre a API de Pessoas, confira [Obter informações relevantes sobre as pessoas](people-example.md). |
| Adição        | v1.0        | A permissão People.Read.All foi adicionada. Para saber mais, confira [Permissões](permissions-reference.md). |
| Adição        | v1.0        | O recurso [personType](/graph/api/resources/persontype?view=graph-rest-1.0) foi adicionado. |
| Alteração          | v1.0        | O recurso [scoredEmailAddress](/graph/api/resources/scoredemailaddress?view=graph-rest-1.0) substituiu o recurso **rankedEmailAddress**. |
| Alteração          | v1.0        | O recurso [person](/graph/api/resources/person?view=graph-rest-1.0) foi atualizado da seguinte maneira:<ul><li>A propriedade **scoredEmailAddresses** (uma coleção do tipo [scoredEmailAddress](/graph/api/resources/scoredemailaddress?view=graph-rest-1.0)) substituiu a propriedade **emailAddresses**</li><li>A propriedade **jobTitle** substituiu a propriedade **title**</li><li>As propriedades **sources** e **mailboxType** foram removidas</li><li>A propriedade **personType** agora é do tipo [personType](/graph/api/resources/persontype?view=graph-rest-1.0) em vez do tipo cadeia de caracteres e substitui a funcionalidade das propriedades **sources** e **mailboxType** anteriores</li><li>A propriedade **imAddress** foi adicionada</li></ul> |
| Exclusão        | v1.0        | O recurso **personDataSource** foi removido. |

### <a name="user"></a>Usuário

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | beta        | Adicionada propriedade **employeeId** ao [usuário](/graph/api/resources/user?view=graph-rest-beta) |

## <a name="july-2017"></a>Julho de 2017

### <a name="group-settings"></a>Configurações de grupo

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Adicionado suporte para as configurações de grupo.<br/>Novos tipos de recurso: [groupSetting](/graph/api/resources/groupsetting?view=graph-rest-1.0), [groupSettingTemplate](/graph/api/resources/groupsettingtemplate?view=graph-rest-1.0), [settingValue](/graph/api/resources/settingvalue?view=graph-rest-1.0) e [settingTemplateValue](/graph/api/resources/settingtemplatevalue?view=graph-rest-1.0) |
| Alteração          | v1.0        | Adicionou a propriedade **classification** e a propriedade de navegação **settings** ao [group](/graph/api/resources/group?view=graph-rest-1.0) |

### <a name="intune-apis"></a>APIs do Intune

| Change&nbsp;type | Versão | Descrição                              |
| :--------------- | :------ | :--------------------------------------- |
| Adição         | Beta    | A ação [assign](/graph/api/intune-apps-iosmobileappconfiguration-assign?view=graph-rest-beta) foi adicionada a [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta) |
| Adição         | Beta    | A ação [syncDevice](/graph/api/intune-devices-manageddevice-syncdevice?view=graph-rest-beta) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Alteração           | Beta    | Foram adicionadas as propriedades **appsInstallAllowList**, **appsLaunchBlockList** e **appsHideList** à entidade [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) |
| Alteração           | Beta    | A propriedade **disableAppEncryptionIfDeviceEncryptionIsEnabled** foi adicionada à entidade [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) |
| Alteração           | Beta    | A propriedade **disableAppEncryptionIfDeviceEncryptionIsEnabled** foi adicionada à entidade [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) |
| Alteração           | Beta    | A propriedade **complianceGracePeriodExpirationDateTime** foi adicionada à entidade [deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-beta) |
| Alteração           | Beta    | A propriedade **complianceGracePeriodExpirationDateTime** foi adicionada à entidade [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta) |
| Alteração           | Beta    | A propriedade **complianceGracePeriodExpirationDateTime** foi adicionada à entidade [deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-beta) |
| Alteração           | Beta    | A propriedade **subscriptions** foi adicionada à entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) |
| Alteração           | Beta    | A propriedade **version** foi adicionada à entidade [deviceManagementExchangeConnector](/graph/api/resources/intune-onboarding-devicemanagementexchangeconnector?view=graph-rest-beta) |
| Alteração           | Beta    | A propriedade **utcTimeOffsetInMinutes** foi adicionada à entidade [iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-beta) |
| Alteração           | Beta    | A propriedade **complianceGracePeriodExpirationDateTime** foi adicionada à entidade [iosUpdateDeviceStatus](/graph/api/resources/intune-deviceconfig-iosupdatedevicestatus?view=graph-rest-beta) |
| Alteração           | Beta    | A propriedade **preSharedKey** foi adicionada à entidade [macOSWiFiConfiguration](/graph/api/resources/intune-deviceconfig-macoswificonfiguration?view=graph-rest-beta) |
| Alteração           | Beta    | Foram adicionadas as propriedades **phoneNumber**, **androidSecurityPatchLevel** e **userDisplayName** à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Alteração           | Beta    | Foram adicionadas as propriedades **userName**, **deviceModel**, **platform** e **complianceGracePeriodExpirationDateTime** à entidade [managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta) |
| Alteração           | Beta    | A propriedade **userPrincipalName** foi adicionada à entidade [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) |
| Alteração           | Beta    | A propriedade **overrideDefaultRule** foi adicionada à entidade [onPremisesConditionalAccessSettings](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-beta) |
| Alteração           | Beta    | A propriedade **userPrincipalName** foi adicionada à entidade [userAppInstallStatus](/graph/api/resources/intune-apps-userappinstallstatus?view=graph-rest-beta) |
| Alteração           | Beta    | Foram adicionadas as propriedades **connectAppBlockAutoLaunch**, **deviceAccountBlockExchangeServices**, **deviceAccountEmailAddress**, **deviceAccountExchangeServerAddress**, **deviceAccountRequirePasswordRotation**, **deviceAccountSessionInitiationProtocolAddress**, **settingsBlockMyMeetingsAndFiles**, **settingsBlockSessionResume**, **settingsBlockSigninSuggestions**, **settingsDefaultVolume**, **settingsScreenTimeoutInMinutes**, **settingsSessionTimeoutInMinutes** e **settingsSleepTimeoutInMinutes** à entidade [windows10TeamGeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10teamgeneralconfiguration?view=graph-rest-beta) |
| Alteração           | Beta    | A propriedade de navegação **deploymentSummary** foi adicionada à entidade [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) |
| Alteração           | Beta    | Foram adicionadas as propriedades **settingName**, **userId**, **userName**, **userEmail** e **currentValue** ao tipo complexo [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta) |
| Alteração           | Beta    | As propriedades **settingName**, **userId**, **userName**, **userEmail** e **currentValue** foram adicionadas ao tipo complexo [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) |
| Alteração           | Beta    | A propriedade **unknownCount** foi adicionada ao tipo complexo [deviceOperatingSystemSummary](/graph/api/resources/intune-devices-deviceoperatingsystemsummary?view=graph-rest-beta) |



## <a name="june-2017"></a>Junho de 2017

### <a name="project-rome"></a>Project Rome

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Adicionados os seguintes recursos e APIs:<br/>[Atividades](/graph/api/resources/projectrome-activity?view=graph-rest-beta)<br/>[Criar ou substituir uma atividade](/graph/api/projectrome-put-activity?view=graph-rest-beta)<br/>[Excluir uma atividade](/graph/api/projectrome-delete-activity?view=graph-rest-beta)<br/>[Item do histórico](/graph/api/resources/projectrome-historyitem?view=graph-rest-beta)<br/>[Criar ou substituir um item do histórico](/graph/api/projectrome-put-historyitem?view=graph-rest-beta)<br/>[Excluir um item do histórico](/graph/api/projectrome-delete-historyitem?view=graph-rest-beta) |

### <a name="outlook-calendar"></a>Calendário do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Foram promovidas as seguintes 4 propriedades de [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) para v1.0: **canEdit**, **canShare**, **canViewPrivateItems** e **owner**. |


### <a name="intune-apis"></a>APIs do Intune

| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Adição    | Beta    | Foram adicionadas novas entidades:<br/>[defaultDeviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-defaultdevicecompliancepolicy?view=graph-rest-beta)<br/>[deviceConfigurationUserStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatesummary?view=graph-rest-beta)<br/>[deviceManagementScriptDeviceState](/graph/api/resources/intune-devicefe-devicemanagementscriptdevicestate?view=graph-rest-beta)<br/>[deviceManagementScriptRunSummary](/graph/api/resources/intune-devicefe-devicemanagementscriptrunsummary?view=graph-rest-beta)<br/>[deviceManagementScriptUserState](/graph/api/resources/intune-devicefe-devicemanagementscriptuserstate?view=graph-rest-beta)<br/>[iosUpdateDeviceStatus](/graph/api/resources/intune-deviceconfig-iosupdatedevicestatus?view=graph-rest-beta)<br/>[windowsManagedDevice](/graph/api/resources/intune-devicefe-windowsmanageddevice?view=graph-rest-beta)<br/>[windowsManagementAppHealthState](/graph/api/resources/intune-devicefe-windowsmanagementapphealthstate?view=graph-rest-beta)<br/>[windowsManagementAppHealthSummary](/graph/api/resources/intune-devicefe-windowsmanagementapphealthsummary?view=graph-rest-beta)<br/> |
| Adição    | Beta    | Foram adicionados novos tipos complexos:<br/>[bitLockerFixedDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockerfixeddrivepolicy?view=graph-rest-beta)<br/>[bitLockerRecoveryOptions](/graph/api/resources/intune-deviceconfig-bitlockerrecoveryoptions?view=graph-rest-beta)<br/>[bitLockerRemovableDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockerremovabledrivepolicy?view=graph-rest-beta)<br/>[deleteUserFromSharedAppleDeviceActionResult](/graph/api/resources/intune-devicefe-deleteuserfromsharedappledeviceactionresult?view=graph-rest-beta)<br/>[iosNetworkUsageRule](/graph/api/resources/intune-deviceconfig-iosnetworkusagerule?view=graph-rest-beta)<br/> |
| Exclusão    | Beta    | Foram removidas as seguintes entidades:<br/>**deviceManagementScriptState**<br/> |
| Exclusão    | Beta    | Foi removida a ação wipeByDeviceTag em [user](/graph/api/resources/intune-devicefe-user?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **innerAuthenticationProtocolForEapTtls**, **innerAuthenticationProtocolForPeap** e **outerIdentityPrivacyTemporaryValue** à entidade [androidEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidenterprisewificonfiguration?view=graph-rest-beta). |
| Alteração      | Beta    | Foram removidas as propriedades **nonEapAuthenticationMethodForEapTtls**, **nonEapAuthenticationMethodForPeap** e **enableOuterIdentityPrivacy** da entidade [androidEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidenterprisewificonfiguration?view=graph-rest-beta). |
| Alteração      | Beta    | A propriedade **deployedAppCount** foi adicionada à entidade [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as propriedades **instanceDisplayName** e **settingPlatform** da entidade [complianceSettingStateSummary](/graph/api/resources/compliancesettingstatesummary?view=graph-rest-beta). |
| Alteração      | Beta    | A propriedade **deployedAppCount** foi adicionada à entidade [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) |
| Alteração      | Beta    | Adicionada a propriedade **excludeGroup** à entidade [deviceCompliancePolicyGroupAssignment](/graph/api/resources/intune-deviceconfig-devicecompliancepolicygroupassignment?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as propriedades **instanceDisplayName** e **settingPlatform** da entidade [deviceCompliancePolicySettingStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary?view=graph-rest-beta) |
| Alteração      | Beta    | Foi removida a propriedade **devicePlatform** da entidade [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **assignmentStatus**, **assignmentProgress** e **assignmentErrorMessage** à entidade [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta)  |
| Alteração      | Beta    | A propriedade **intuneBrand** foi adicionada à entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **enforceSignatureCheck** e **fileName** à entidade [deviceManagementScript](/graph/api/resources/intune-devicefe-devicemanagementscript?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **innerAuthenticationProtocolForEapTtls** e **outerIdentityPrivacyTemporaryValue** à entidade [iosEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-iosenterprisewificonfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as propriedades **nonEapAuthenticationMethodForEapTtls** e **enableOuterIdentityPrivacy** da entidade [iosEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-iosenterprisewificonfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **classroomAppForceUnpromptedScreenObservation**, **keyboardBlockDictation**, **networkUsageRules** e **wiFiConnectOnlyToConfiguredNetworks** à entidade [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **deployedAppCount** foi adicionada à entidade [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **preSharedKey** foi adicionada à entidade [iosWiFiConfiguration](/graph/api/resources/intune-deviceconfig-ioswificonfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **innerAuthenticationProtocolForEapTtls** e **outerIdentityPrivacyTemporaryValue** à entidade [macOSEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-macosenterprisewificonfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as propriedades **nonEapAuthenticationMethodForEapTtls** e **enableOuterIdentityPrivacy** da entidade [macOSEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-macosenterprisewificonfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as entidades **lastModifiedTime** e **deployedAppCount** da entidade [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **serialNumber** foi adicionada à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Alteração      | Beta    | Foi removida a propriedade **managementAgents** da entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **deployedAppCount** foi adicionada à entidade [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **bitLockerFixedDrivePolicy** e **bitLockerRemovableDrivePolicy** à entidade [windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **enterpriseCloudPrintDiscoveryEndPoint**, **enterpriseCloudPrintOAuthAuthority**, **enterpriseCloudPrintOAuthClientIdentifier**, **enterpriseCloudPrintResourceIdentifier**, **enterpriseCloudPrintDiscoveryMaxLimit**, **enterpriseCloudPrintMopriaDiscoveryResourceIdentifier**, **edgeBlockAddressBarDropdown**, **edgeBlockCompatibilityList**, **edgeClearBrowsingDataOnExit**, **edgeAllowStartPagesModification**, **edgeDisableFirstRunPage**, **edgeBlockLiveTileDataCollection** e **edgeSyncFavoritesWithInternetExplorer** à entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **availableVersion** foi adicionada à entidade [windowsManagementApp](/graph/api/resources/intune-devicefe-windowsmanagementapp?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as propriedades **onboardingStatus**, **deployedVersion** e **lastModifiedTime** da entidade [windowsManagementApp](/graph/api/resources/intune-devicefe-windowsmanagementapp?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **packageIdentityName** foi adicionada à entidade [windowsStoreForBusinessApp](/graph/api/resources/intune-apps-windowsstoreforbusinessapp?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **mobileAppIdentifierDeployments** e **deploymentSummary** à entidade [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **mobileAppIdentifierDeployments** foi adicionada à entidade [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **deviceConfigurationUserStateSummaries** e **iosUpdateStatuses** à entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) |
| Alteração      | Beta    | Foi removida a propriedade de navegação **complianceSettingStateSummaries** da entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **runSummary**, **deviceRunStates** e **userRunStates** à entidade [deviceManagementScript](/graph/api/resources/intune-devicefe-devicemanagementscript?view=graph-rest-beta) |
| Alteração      | Beta    | Foi removida a propriedade de navegação **runStates** da entidade [deviceManagementScript](/graph/api/resources/intune-devicefe-devicemanagementscript?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **mobileAppIdentifierDeployments** e **deploymentSummary** à entidade [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as propriedades de navegação **mobileAppIdentifierDeployments** e **deploymentSummary** da entidade [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **mobileAppIdentifierDeployments** e **deploymentSummary** à entidade [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **healthSummary** e **healthStates** à entidade [windowsManagementApp](/graph/api/resources/intune-devicefe-windowsmanagementapp?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **applicationId**, **appName**, **platformId**, **userFailures** e **deviceFailures** ao tipo complexo [appInstallationFailure](/graph/api/resources/intune-apps-appinstallationfailure?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **encryptionMethod**, **startupAuthenticationRequired**, **startupAuthenticationBlockWithoutTpmChip**, **startupAuthenticationTpmUsage**, **startupAuthenticationTpmPinUsage**, **startupAuthenticationTpmKeyUsage**, **startupAuthenticationTpmPinAndKeyUsage**, **recoveryOptions** e **prebootRecoveryEnableMessageAndUrl** ao tipo complexo [bitLockerSystemDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockersyst?view=graph-rest-betarivepolicy) |
| Alteração      | Beta    | Foram removidas as propriedades **settingName**, **userId**, **userName**, **userEmail** e **currentValue** do tipo complexo [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as propriedades **settingName**, **userId**, **userName**, **userEmail** e **currentValue** do tipo complexo [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **windowsCommercialId** e **windowsCommercialIdLastModifiedTime** ao tipo complexo [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **address** foi adicionada ao tipo complexo [vpnServer](/graph/api/resources/intune-deviceconfig-vpnserver?view=graph-rest-beta) |


## <a name="may-2017"></a>Maio de 2017

### <a name="application-api-changes"></a>Alterações da API do aplicativo

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | Atualização da API do aplicativo. Este é o primeiro conjunto de alterações incluindo renomeação de propriedade e restruturação da entidade [application](/graph/api/resources/application?view=graph-rest-beta).<br/>**Novas entidades:** [api](/graph/api/resources/api?view=graph-rest-beta]), [informationalUrl](/graph/api/resources/informationalurl?view=graph-rest-beta), [installedClient](/graph/api/resources/installedclient?view=graph-rest-beta), [permissionScope](/graph/api/resources/permissionscope?view=graph-rest-beta), [preauthorizedApplication](/graph/api/resources/preauthorizedapplication?view=graph-rest-beta) e [web](/graph/api/resources/web?view=graph-rest-beta).<br/>**Propriedades removidas:** addIns, appRoles, availableToOtherOrganizations, knownClientApplications, oauth2AllowUrlPathMatching e recordConsentConditions.<br/>**Propriedades renomeadas:** appId agora é id, identifierUris agora é applicationAliases, availableToOtherTenants agora é orgRestrictions, mainLogo agora é logo, oauth2Permissions agora é publishedPermissionsScopes, publicClient agora é allowPublicClient e replyUrls agora é redirectUrls.<br/>**Novas propriedades:** tags. |

### <a name="remove-deprecated-planner-api"></a>Remover a API do Planner descontinuada
| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Exclusão        | Beta        | Foram removidas as seguintes entidades:<br/>**task**<br/>**plan**<br/>**bucket**<br/>**taskDetails**<br/>**planDetails**<br/>**taskBoardTaskFormat**<br/>**planTaskBoard** |

### <a name="project-rome"></a>Project Rome

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Adicionou suporte ao Project Rome, incluindo [obter uma lista de dispositivos](/graph/api/user-list-devices?view=graph-rest-beta), [enviar um comando para um dispositivo](/graph/api/send-device-command?view=graph-rest-beta) e [verificar o status de um comando](/graph/api/get-device-command-status?view=graph-rest-beta). |
| Adição        | Beta        | Suporte adicionado para [atividades](/graph/api/resources/projectrome-activity?view=graph-rest-beta) e [historyItems](/graph/api/resources/projectrome-historyitem?view=graph-rest-beta) de usuário, inclusive [operação upsert para atividade](/graph/api/projectrome-put-activity?view=graph-rest-beta) e [operação upsert para historyItem](/graph/api/projectrome-put-historyitem?view=graph-rest-beta). |

### <a name="administrative-units-property-changes"></a>Alterações de propriedade de unidades administrativas

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | Alterou o tipo de propriedade roleMemberInfo para [identity](/graph/api/resources/identity?view=graph-rest-1.0) para a entidade [scopedRoleMembership](/graph/api/resources/scopedrolemembership?view=graph-rest-beta) |
| Alteração          | Beta        | Alterou a propriedade de navegação de scopedAdministratorOf para scopedRoleMemberOf para a entidade [user](/graph/api/resources/user?view=graph-rest-beta) |
| Alteração          | Beta        | Alterou a propriedade de navegação de scopedAdministrators para scopedRoleMembers para a entidade [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta) |
| Alteração          | Beta        | Alterou a propriedade de navegação de scopedAdministrators para scopedMembers para a entidade [directoryRole](/graph/api/resources/directoryrole?view=graph-rest-beta) |

### <a name="add-users-and-groups-webhook-support-in-preview"></a>Adicionar usuários e grupos de suporte do webhook na visualização

|**Tipo de alteração**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
| Alteração        | Beta       | Adicionou suporte aos [webhooks](/graph/api/resources/webhooks?view=graph-rest-beta) para usuários e grupos.

### <a name="add-delta-query-to-v10"></a>Adicionar a consulta delta para v1.0

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Adicionar o suporte à função delta para v1.0. Adicionar às seguintes entidades para realizar [consulta delta](delta-query-overview.md):<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>Confira os seguintes exemplos:<br/>[Obter as alterações incrementais para grupos](delta-query-groups.md)<br/>[Obter as alterações incrementais para as mensagens em uma pasta](delta-query-messages.md)<br/>[Obter as alterações incrementais para usuários](delta-query-users.md) |
| Alteração          | Beta        | Adicionar um novo recurso de filtragem de consulta opcional (por ID) para [users](/graph/api/user-delta?view=graph-rest-beta) e [groups](/graph/api/group-delta?view=graph-rest-beta). |

### <a name="added-user-resource-support-for-deleted-items"></a>Foi adicionado suporte a recursos de usuário para os itens excluídos

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Adicionou suporte para a [restauração e a exclusão permanente de usuários](/graph/api/resources/directory?view=graph-rest-beta). |

### <a name="added-onpremisesprovisioningerror"></a>Adicionou OnPremisesProvisioningError

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | beta        | Nova entidade: [OnPremisesProvisioningError](/graph/api/resources/onpremisesprovisioningerror?view=graph-rest-beta) |
| Alteração          | beta        | Adicionou a propriedade OnPremisesProvisioningError para [user](/graph/api/resources/user?view=graph-rest-beta), [group](/graph/api/resources/group?view=graph-rest-beta) e [orgcontact](/graph/api/resources/orgcontact?view=graph-rest-beta) |

### <a name="added-deleteddatetime-property"></a>Adicionou a propriedade deletedDateTime

|**Tipo de alteração**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Alteração|beta|Adicionou a propriedade deletedDateTime à entidade [user](/graph/api/resources/user?view=graph-rest-beta).
|Alteração|beta|Adicionou a propriedade deletedDateTime à entidade [group](/graph/api/resources/group?view=graph-rest-beta).
|Alteração|beta|Adicionou a propriedade deletedDateTime à entidade [application](/graph/api/resources/application?view=graph-rest-beta).

### <a name="added-domain-operations-to-v10"></a>Adicionou operações de domínio para v1.0

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Operações adicionadas a [domains](/graph/api/resources/domain?view=graph-rest-1.0).<br/>Novas entidades:</br>[domain](/graph/api/resources/domain?view=graph-rest-1.0)<br/>[domainDnsRecord](/graph/api/resources/domaindnsrecord?view=graph-rest-1.0)<br/>[domainDnsCnameRecord](/graph/api/resources/domaindnscnamerecord?view=graph-rest-1.0)<br/>[domainDnsMxRecord](/graph/api/resources/domaindnsmxrecord?view=graph-rest-1.0)<br/>[domainDnsSrvRecord](/graph/api/resources/domaindnssrvrecord?view=graph-rest-1.0)<br/>[domainDnsTxtRecord](/graph/api/resources/domaindnstxtrecord?view=graph-rest-1.0)<br/>[domainDnsUnavailableRecord](/graph/api/resources/domaindnsunavailablerecord?view=graph-rest-1.0)<br/>Novas ações:</br>[verify](/graph/api/domain-verify?view=graph-rest-1.0) |

### <a name="added-contracts-to-v10"></a>Adicionou contratos para v1.0

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Nova entidade:</br>[contract](/graph/api/resources/contract?view=graph-rest-1.0) |

### <a name="added-licensedetails-to-v10"></a>Adicionou licenseDetails para v1.0

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Nova entidade:</br>[licenseDetails](/graph/api/resources/licensedetails?view=graph-rest-1.0) |
| Alteração          | v1.0        | Nova propriedade de navegação [licensedetails](/graph/api/user-list-licensedetails?view=graph-rest-1.0) em [users](/graph/api/resources/user?view=graph-rest-1.0) |


### <a name="drive-api"></a>API de Unidade

|**Tipo de alteração**|**Versão**|**Descrição**|
|:--------------|:----------|:--------------|
| Adição | v1.0 | Adicionou o tipo de recurso **baseItem**, consistindo em propriedades básicas de **driveItem**.
| Adição | v1.0 e Beta | Adicionou a propriedade **sourceItemId** à **thumbnail**. <br/> Adicionou a propriedade **siteUrl** à **sharepointIds**. <br/> Adicionou as propriedades **sharedBy** e **sharedDateTime** à **shared**. <br/> Adicionou a propriedade **shared** à **remoteItem**. <br/> Adicionou a propriedade **sharepointIds** à **drive** e **itemReference**. <br/> Adicionou **lastAccessedDateTime** à **fileSystemInfo**. <br/> Adicionou as propriedades de navegação **driveItem** e **site** à **sharedDriveItem**. <br/> Adicionou a propriedade **parentReference** à **baseItem**.
| Alteração | v1.0 e Beta | Alterou **driveItem** e **sharedDriveItem** para herdar de **baseItem**. <br/> Marcou **identity** como um Tipo Aberto.
| Alteração | Beta | Adicionou as propriedades **configuratorUrl** e **webHtml** à **sharingLink**. <br/> Adicionou o tipo de recurso **folderView** e a propriedade **view** ao tipo de recurso **folder**. <br/> Adicionou a propriedade de navegação **listItem** à **driveItem**. <br/> Adicionou a propriedade de navegação **list** à **drive**.


### <a name="extensions-open-extensions"></a>Extensões (extensões abertas)

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0          | Suporte para [openTypeExtension](/graph/api/resources/opentypeextension?view=graph-rest-1.0) nos seguintes recursos – [device](/graph/api/resources/device?view=graph-rest-1.0), [group](/graph/api/resources/group?view=graph-rest-1.0),[organization](/graph/api/resources/organization?view=graph-rest-1.0), [user](/graph/api/resources/user?view=graph-rest-1.0). |
| Adição        | v1.0 e beta | Quando o usuário está conectado com uma conta pessoal da Microsoft, suporte para extensões abertas nos seguintes recursos – evento, postagem, grupo, mensagem, contato e usuário. (É um adicional para estes recursos, além do dispositivo, grupo, organização e usuário, suporte a extensões abertas quando o usuário entra usando uma conta corporativa ou de estudante.) |
| Adição        | v1.0 e beta | Suporte para `$expand` para [obter extensões abertas](/graph/api/opentypeextension-get?view=graph-rest-1.0) nos seguintes recursos: [device](/graph/api/resources/device?view=graph-rest-1.0), [group](/graph/api/resources/group?view=graph-rest-1.0),[organization](/graph/api/resources/organization?view=graph-rest-1.0), [post](/graph/api/resources/post?view=graph-rest-1.0), [user](/graph/api/resources/user?view=graph-rest-1.0). |
| Adição        | Beta          | Suporte para `$expand` para [obter extensões abertas](/graph/api/opentypeextension-get?view=graph-rest-1.0) na [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta). |


### <a name="extensions-schema-extensions"></a>Extensões (extensões de esquema)

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0          | Novo recurso [schemaExtension](/graph/api/resources/schemaextension?view=graph-rest-1.0) e métodos CRUD para gerenciar definições de extensão para os seguintes recursos: [contact](/graph/api/resources/contact?view=graph-rest-1.0), [device](/graph/api/resources/device?view=graph-rest-1.0), [event](/graph/api/resources/event?view=graph-rest-1.0), [group](/graph/api/resources/group?view=graph-rest-1.0), [message](/graph/api/resources/message?view=graph-rest-1.0), [organization](/graph/api/resources/organization?view=graph-rest-1.0), [post](/graph/api/resources/post?view=graph-rest-1.0), [user](/graph/api/resources/user?view=graph-rest-1.0). Observe que seu suporte para [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta) ainda está limitado à versão beta como antes. |
| Adição        | v1.0          | Os métodos POST, GET e PATCH existentes dos seguintes recursos: [contact](/graph/api/resources/contact?view=graph-rest-1.0), [device](/graph/api/resources/device?view=graph-rest-1.0), [event](/graph/api/resources/event?view=graph-rest-1.0), [group](/graph/api/resources/group?view=graph-rest-1.0), [message](/graph/api/resources/message?view=graph-rest-1.0), [organization](/graph/api/resources/organization?view=graph-rest-1.0), [post](/graph/api/resources/post?view=graph-rest-1.0), [user](/graph/api/resources/user?view=graph-rest-1.0) – agora suportam a adição, obtenção e carregamento ou exclusão de dados personalizados armazenados como extensões de esquema nas instâncias de recursos correspondentes. |
| Adição        | v1.0 e beta | Agora, você pode usar o `$filter` para pesquisar instâncias de recursos com propriedades que correspondam a valores de propriedade de extensão específicos, como nome de extensão. Confira este [exemplo](extensibility-schema-groups.md#5-get-a-group-and-its-extension-data) para obter detalhes. |
| Alteração          | v1.0 e beta | [Excluir um esquema de definição de extensões](/graph/api/schemaextension-delete?view=graph-rest-1.0) não afeta mais o acesso a dados personalizados que foram adicionados com base nessa definição. |
| Alteração          | v1.0 e beta | Agora você pode definir um tipo complexo de extensão de esquema como nulo, para remover uma extensão de esquema de uma instância de recurso. |


### <a name="group"></a>Group

|**Tipo de alteração**|**Versão**|**Descrição**|
|:--------------|:----------|:--------------|
| Adição | v1.0 e beta | Foram adicionadas as propriedades de navegação **drives** e **sites** a **group**.

### <a name="insights-apis"></a>APIs de informações

|**Tipo de alteração**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Adição|Beta|A [API compartilhada](/graph/api/resources/insights-shared?view=graph-rest-beta) foi adicionada.<br />Novos recursos:<br />[sharingDetail](/graph/api/resources/insights-sharingdetail?view=graph-rest-beta) <br />[insightIdentity](/graph/api/resources/insights-insightidentity?view=graph-rest-beta) <br />
|Adição|Beta|A [API usada](/graph/api/resources/insights-used?view=graph-rest-beta) foi adicionada.<br />Novos recursos:<br />[usageDetails](/graph/api/resources/insights-usagedetails?view=graph-rest-beta) <br />
|Alteração|Beta|Propriedade Novo **Tipo**no:<br />recurso [resourceVisualization](/graph/api/resources/insights-resourcevisualization?view=graph-rest-beta). <br />
|Exclusão|Beta|Foram removidas as seguintes entidades:<br/>**workingWith**<br/>**trendingAround**<br/>|

### <a name="intune-apis"></a>APIs do Intune

| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Adição    | Beta    | Foram adicionadas novas entidades:<br/>[androidForWorkMobileAppConfiguration](/graph/api/resources/intune-apps-androidforworkmobileappconfiguration?view=graph-rest-beta)<br/>[cartToClassAssociation](/graph/api/resources/intune-deviceconfig-carttoclassassociation?view=graph-rest-beta)<br/>[deviceCompliancePolicySettingStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary?view=graph-rest-beta)<br/>[eBookInstallSummary](/graph/api/resources/intune-books-ebookinstallsummary?view=graph-rest-beta)<br/>[eBookVppGroupAssignment](/graph/api/resources/intune-books-ebookvppgroupassignment?view=graph-rest-beta)<br/>[iosUpdateConfiguration](/graph/api/resources/intune-deviceconfig-iosupdateconfiguration?view=graph-rest-beta)<br/>[remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-beta)<br/>[windows10EndpointProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10endpointprotectionconfiguration?view=graph-rest-beta)<br/>[windowsDeviceMalwareState](/graph/api/resources/intune-endpointprotection-windowsdevicemalwarestate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppLearningSummary](/graph/api/resources/intune-wip-windowsinformationprotectionapplearningsummary?view=graph-rest-beta)<br/>[windowsMalwareInformation](/graph/api/resources/intune-endpointprotection-windowsmalwareinformation?view=graph-rest-beta)<br/>[windowsProtectionState](/graph/api/resources/intune-endpointprotection-windowsprotectionstate?view=graph-rest-beta)<br/> |
| Adição    | Beta    | Foram adicionados novos tipos complexos:<br/>[androidPermissionAction](/graph/api/resources/intune-apps-androidpermissionaction?view=graph-rest-beta)<br/>[bitLockerSystemDrivePolicy](/graph/api/resources/intune-deviceconfig-bitlockersyst?view=graph-rest-betarivepolicy)<br/>[defenderDetectedMalwareActions](/graph/api/resources/intune-deviceconfig-defenderdetectedmalwareactions?view=graph-rest-beta)<br/>[settingSource](/graph/api/resources/intune-deviceconfig-settingsource?view=graph-rest-beta)<br/> |
| Adição    | Beta    | A ação [assign](/graph/api/intune-books-managedebook-assign?view=graph-rest-beta) foi adicionada a [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) |
| Adição    | Beta    | A ação [beginOnboarding](/graph/api/intune-remoteassistance-remoteassistancepartner-beginonboarding?view=graph-rest-beta) foi adicionada a [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-beta) |
| Adição    | Beta    | A ação [disconnect](/graph/api/intune-remoteassistance-remoteassistancepartner-disconnect?view=graph-rest-beta) foi adicionada a [remoteAssistancePartner](/graph/api/resources/intune-remoteassistance-remoteassistancepartner?view=graph-rest-beta) |
| Exclusão    | Beta    | Foram removidas as seguintes entidades:<br/>**outlookTask**<br/>**outlookTaskFolder**<br/>**outlookTaskGroup**<br/>**outlookUser**<br/>**windowsManagementAppHealthState**<br/> |
| Exclusão    | Beta    | Foram removidos os seguintes tipos complexos:<br/>**applePushNotificationCertificateSetting**<br/>**eventCreationOptions**<br/> |
| Alteração      | Beta    | As propriedades **workProfilePasswordBlockFingerprintUnlock**, **workProfilePasswordBlockTrustAgents**, **workProfilePasswordExpirationDays**, **workProfilePasswordMinimumLength**, **workProfilePasswordMinutesOfInactivityBeforeScreenTimeout**, **workProfilePasswordPreviousPasswordBlockCount**, **workProfilePasswordSignInFailureCountBeforeFactoryReset**, **workProfilePasswordRequiredType** e **workProfileRequirePassword** foram adicionadas à entidade [androidForWorkGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **subjectAlternativeNameFormatString** foi adicionada à entidade [androidForWorkPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **subjectNameFormatString** e **subjectAlternativeNameFormatString** foram adicionadas à entidade [androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **kioskModeManagedApps** foi adicionada à entidade [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **kioskModeManagedAppId** foi removida da entidade [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **subjectAlternativeNameFormatString** foi adicionada à entidade [androidPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidpkcscertificateprofile?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **subjectNameFormatString** e **subjectAlternativeNameFormatString** foram adicionadas à entidade [androidScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidscepcertificateprofile?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **hexColor** foi removida da entidade [calendar](/graph/api/resources/calendar?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **setting** e **platformType** foram adicionadas à entidade [complianceSettingStateSummary](/graph/api/resources/intune-deviceconfig-compliancesettingstatesummary?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **windowsManagementAppEnabled** foi removida da entidade [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **userName**, **deviceModel** e **platform** foram adicionadas à entidade [deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **userPrincipalName** e **deviceModel** foram adicionadas à entidade [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **platformType**, **setting**, **userId** e **userEmail** foram adicionadas à entidade [deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **inGracePeriodCount** foi adicionada à entidade [deviceCompliancePolicyDeviceStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **userName**, **deviceModel** e **platform** foram adicionadas à entidade [deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **creationOptions** foi removida da entidade [event](/graph/api/resources/event?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **isDelegated** foi removida da entidade [eventMessage](/graph/api/resources/eventmessage?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **unseenConversationsCount** e **unseenMessagesCount** foram removidas da entidade [group](/graph/api/resources/group?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **settingXml** e **settings** foram adicionadas à entidade [iosMobileAppConfiguration](/graph/api/resources/intune-apps-iosmobileappconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **subjectAlternativeNameFormatString** foi adicionada à entidade [iosPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-iospkcscertificateprofile?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **subjectAlternativeNameFormatString** foi adicionada à entidade [iosScepCertificateProfile](/graph/api/resources/intune-deviceconfig-iosscepcertificateprofile?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **systemIntegrityProtectionEnabled** foi adicionada à entidade [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **subjectAlternativeNameFormatString** foi adicionada à entidade [macOSScepCertificateProfile](/graph/api/resources/intune-deviceconfig-macosscepcertificateprofile?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **complianceGracePeriodExpirationDateTime**, **userPrincipalName** e **imei** foram adicionadas à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **settingXml** e **settings** foram removidas da entidade [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **useSharedComputerActivation**, **updateChannel**, **officePlatformArchitecture** e **localesToInstall** foram adicionadas à entidade [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **applePushNotificationCertificateSetting** foi removida da entidade [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades a seguir foram alteradas na entidade [post](/graph/api/resources/post?view=graph-rest-beta):<br/>**sender** de opcional para obrigatório<br/> |
| Alteração      | Beta    | As propriedades **compliantUserCount**, **nonCompliantUserCount**, **remediatedUserCount**, **errorUserCount**, **unknownUserCount**, **conflictUserCount** e **notApplicableUserCount** foram adicionadas à entidade [softwareUpdateStatusSummary](/graph/api/resources/intune-deviceconfig-softwareupdatestatussummary?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **bluetoothAllowedServices**, **bluetoothBlockPrePairing**, **cellularData**, **defenderDetectedMalwareActions**, **defenderPotentiallyUnwantedAppAction**, **lockScreenAllowTimeoutConfiguration**, **lockScreenBlockCortana**, **lockScreenBlockToastNotifications**, **lockScreenTimeoutInSeconds**, **passwordBlockSimple**, **privacyAutoAcceptPairingAndConsentPrompts**, **privacyBlockInputPersonalization**, **startMenuHideChangeAccountSettings**, **startMenuHideHibernate**, **startMenuHideLock**, **startMenuHideShutDown**, **startMenuHideSignOut**, **startMenuHideSleep**, **startMenuHideSwitchAccount**, **settingsBlockAppsPage**, **settingsBlockGamingPage**, **windowsSpotlightBlockConsumerSpecificFeatures**, **windowsSpotlightBlocked**, **windowsSpotlightBlockOnActionCenter**, **windowsSpotlightBlockTailoredExperiences**, **windowsSpotlightBlockThirdPartyNotifications**, **windowsSpotlightBlockWelcomeExperience**, **windowsSpotlightBlockWindowsTips**, **windowsSpotlightConfigureOnLockScreen** e **connectedDevicesServiceBlocked** foram adicionadas à entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **automaticUpdateMode**, **automaticUpdateSchedule**, **automaticUpdateTime**, **prereleaseFeatures**, **experienceBlockWindowsSpotlight**, **experienceBlockWindowsTips** e **experienceBlockConsumerSpecificFeatures** foram removidas da entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **subjectAlternativeNameFormatString** foi adicionada à entidade [windows10PkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-windows10pkcscertificateprofile?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **subjectNameFormatString** e **subjectAlternativeNameFormatString** foram adicionadas à entidade [windows81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windows81scepcertificateprofile?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **indexingEncryptedStoresOrItemsBlocked** e **smbAutoEncryptedFileExtensions** foram adicionadas à entidade [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) |
| Alteração      | Beta    | As seguintes propriedades foram alteradas na entidade [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta):<br/>**rightsManagementServicesTemplateId** de obrigatório para opcional<br/> |
| Alteração      | Beta    | As seguintes propriedades foram alteradas na entidade [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta):<br/>**productCode** de obrigatório para opcional<br/> |
| Alteração      | Beta    | As propriedades **subjectNameFormatString** e **subjectAlternativeNameFormatString** foram adicionadas à entidade [windowsPhone81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81scepcertificateprofile?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **mobileAppConfigurations** foi adicionada à entidade [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades de navegação **cartToClassAssociations**, **deviceCompliancePolicySettingStateSummaries**, **remoteAssistancePartners**, **windowsInformationProtectionAppLearningSummaries** e **windowsMalwareInformation** foram adicionadas à entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **eBook** foi adicionada à entidade [eBookGroupAssignment](/graph/api/resources/intune-books-ebookgroupassignment?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **windowsProtectionState** foi adicionada à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **installSummary** foi adicionada à entidade [managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **outlook** foi removida da entidade [user](/graph/api/resources/intune-deviceconfig-user?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **healthStates** foi removida da entidade [windowsManagementApp](/graph/api/resources/intune-deviceconfig-windowsmanagementapp?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **androidForWorkRestrictions** foi adicionada ao tipo complexo [defaultDeviceEnrollmentRestrictions](/graph/api/resources/intune-onboarding-defaultdeviceenrollmentrestrictions?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **userPrincipalName** e **sources** foram adicionadas ao tipo complexo [deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **userPrincipalName** e **sources** foram adicionadas ao tipo complexo [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **settingName**, **userId**, **userName**, **userEmail** e **currentValue** foram adicionadas ao tipo complexo [deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **archiveFolder** foi removida do tipo complexo [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-beta) |


### <a name="outlook-calendar"></a>Calendário do Outlook

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0 e beta | Para **findMeetingTimes**, adicionou o novo valor de enumeração **unrestricted** que você especifica como a propriedade **activityDomain**, parte do parâmetro **timeConstraint**. Isso permite que **findMeetingTimes** procure os horários apropriados para o tipo de atividade que você está agendando. Confira detalhes na seção [corpo da solicitação](/graph/api/user-findmeetingtimes?view=graph-rest-1.0#request-body). |
| Adição        | Beta          | Suporte para obter um corpo de **event** em um texto sem formatação, como alternativa ao formato HTML padrão. Confira os eventos [get](/graph/api/event-get?view=graph-rest-beta) e [list](/graph/api/user-list-events?view=graph-rest-beta) para obter detalhes. |

### <a name="outlook-mail"></a>Email do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | Suporte para obter um corpo de **message** em um texto sem formatação, como alternativa ao formato HTML padrão. Confira os eventos [get](/graph/api/message-get?view=graph-rest-beta) e [list](/graph/api/user-list-messages?view=graph-rest-beta) para obter detalhes. |


### <a name="outlook-tasks"></a>Tarefas do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Nova propriedade de navegação do **outlook** adicionado a [user](/graph/api/resources/user?view=graph-rest-beta), para acessar tarefas do Outlook. |
| Adição        | Beta        | Novas entidades: [outlookuser](/graph/api/resources/outlookuser?view=graph-rest-beta), [outlookTaskGroup](/graph/api/resources/outlooktaskgroup?view=graph-rest-beta), [outlookTaskFolder](/graph/api/resources/outlooktaskfolder?view=graph-rest-beta) e [outlookTask](/graph/api/resources/outlooktask?view=graph-rest-beta), e seus métodos suportam a organização e o acesso a tarefas do Outlook. |
| Adição        | Beta        | As tarefas do Outlook suportam anexos (recursos [attachment](/graph/api/resources/attachment?view=graph-rest-beta), [fileAttachment](/graph/api/resources/fileattachment?view=graph-rest-beta), [itemAttachment](/graph/api/resources/itemattachment?view=graph-rest-beta) e [referenceAttachment](/graph/api/resources/referenceattachment?view=graph-rest-beta)). |
| Adição        | Beta        | As tarefas do Outlook suportam [propriedades estendidas](/graph/api/resources/extended-properties-overview?view=graph-rest-beta) (recursos [singleValueLegacyExtendedProperty](/graph/api/resources/singlevaluelegacyextendedproperty?view=graph-rest-beta) e [multiValueLegacyExtendedProperty](/graph/api/resources/multivaluelegacyextendedproperty?view=graph-rest-beta)). |

### <a name="planner-apis"></a>APIs do Planner

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Adicionou a [API do Planner](/graph/api/resources/planner-overview?view=graph-rest-1.0).<br />Novos recursos:<br />[plannerPlan](/graph/api/resources/plannerplan?view=graph-rest-1.0) <br />[plannerTask](/graph/api/resources/plannertask?view=graph-rest-1.0) <br />[plannerPlanDetails](/graph/api/resources/plannerplandetails?view=graph-rest-1.0) <br />[plannerTaskDetails](/graph/api/resources/plannertaskdetails?view=graph-rest-1.0) <br />[plannerBucket](/graph/api/resources/plannerbucket?view=graph-rest-1.0) <br />[plannerAssignedToTaskBoardTaskFormat](/graph/api/resources/plannerassignedtotaskboardtaskformat?view=graph-rest-1.0) <br />[plannerBucketTaskBoardTaskFormat](/graph/api/resources/plannerbuckettaskboardtaskformat?view=graph-rest-1.0) <br />[plannerProgressTaskBoardTaskFormat](/graph/api/resources/plannerprogresstaskboardtaskformat?view=graph-rest-1.0) |

### <a name="sharepoint-sites"></a>Sites do SharePoint

|**Tipo de alteração**|**Versão**|**Descrição**|
|:--------------|:----------|:--------------|
| Adição      | v1.0      | O recurso de sites está disponível no ponto de extremidade v1.0.<br/> Adicionou os tipos de recursos **site** e **siteCollection**.
| Alteração        | beta      | O formato do identificador para o recurso **site** foi alterado. Esta é uma mudança inovadora na API beta.
| Removido       | beta      | A entidade do **sharePoint** foi removida da API beta. A funcionalidade agora está disponível a partir do conjunto de **sites**.

### <a name="sharepoint-lists"></a>Listas do SharePoint

|**Tipo de alteração**|**Versão**|**Descrição**|
|:--------------|:----------|:--------------|
| Alteração | beta | Removeu as propriedades de navegação **sharepoint**. Agora, os sites são acessados diretamente por meio da propriedade de navegação **sites**. <br/> Removeu o recurso **fieldDefinition**. Ele foi substituído por **columnDefinition**. <br/> Removeu as propriedades **siteCollectionId** e **siteId** de **site**. Use **sharepointIds** em vez disso. <br/> Removeu a propriedade **listItemId** de **listItem**. Use **sharepointIds** em vez disso. <br/> Renomeou a propriedade **columnSet** em **listItem** para **fields**. <br/> Alterou os recursos **site** para usar o nome de host do SharePoint como parte de seu ID.
| Adição | beta | Adicionou os tipos de recursos **booleanColumn**, **calculatedColumn**, **choiceColumn**, **dateTimeColumn**, **lookupColumn**, **numberColumn**, **personOrGroupColumn** e **textColumn**. <br/> Adicionou a propriedade **displayName** a **site**. <br/> Adicionou a propriedade de navegação **columns** à **site**. <br/> Adicionou as propriedades de navegação **list** e **listItem** à **sharedDriveItem**. <br/> Adicionou a propriedade **sharepointIds** à **list**, **listItem** e **site**. <br/> Adicionou o tipo de recurso **columnDefinition**.




## <a name="april-2017"></a>Abril de 2017

### <a name="administrative-units-property-changes"></a>Alterações de propriedade de unidades administrativas

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | As APIs das unidades administrativas serão atualizadas na visualização (beta). O primeiro conjunto de alterações será aplicado em 3 de maio de 2017. As alterações incluem a seguinte renomeação de propriedade:<br />Tipo complexo - **roleMemberInfo** para o tipo complexo **identity** da entidade scopedRoleMembership<br />Propriedade de navegação - **scopedAdministratorOf** para **scopedRoleMemberOf** da entidade do usuário<br />Propriedade de navegação - **scopedAdministrators** para **scopedRoleMembers** da entidade administrativeUnit<br />Propriedade de navegação - **scopedAdministrators** para **scopedMembers** da entidade directoryRole |

### <a name="application-and-serviceprincipal-api-changes"></a>Alterações do aplicativo e da API servicePrincipal

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | As APIs de [aplicativo](/graph/api/resources/application?view=graph-rest-beta) e [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) serão atualizadas na visualização (beta). O primeiro conjunto de alterações será aplicado em 15 de maio de 2017. As alterações incluem a renomeação e a reestruturação de propriedade. Algumas propriedades (como funções de aplicativos e suplementos) não estarão disponíveis até que as alterações sejam concluídas. As alterações serão lançadas na Visualização (beta) antes do lançamento da versão 1.0. |

### <a name="added-preview-support-for-cloud-solution-provider-developers"></a>Foi adicionado o suporte à visualização para desenvolvedores de Provedor de Soluções na Nuvem

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foram adicionados novos recursos de visualização para permitir que os aplicativos previamente consentidos do Provedor de Soluções na Nuvem chamem o Microsoft Graph, descrito em um novo [tópico de autorização](auth-cloudsolutionprovider.md). |

### <a name="added-onpremises-properties-to-user-entity"></a>Adicionadas propriedades onPremises à entidade do usuário

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foram adicionadas novas propriedades onPremises, onPremisesDomainName, OnPremisesSamAccountName e onPremisesUserPrincipalName à entidade do [usuário](/graph/api/resources/user?view=graph-rest-beta). |

### <a name="new-planner-apis-and-an-update-to-the-group-visibility-property"></a>Novas APIs do Planner e uma atualização da propriedade de visibilidade do grupo

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | Foi adicionado o **HiddenMembership** como um valor adicional para a propriedade de visibilidade para a entidade de [Grupo](/graph/api/resources/group?view=graph-rest-beta) |
| Adição        | Beta        | Foi adicionada uma nova [API do Planner](/graph/api/resources/planner-overview?view=graph-rest-beta).<br />Novos recursos:<br />[plannerPlan](/graph/api/resources/plannerplan?view=graph-rest-beta) <br />[plannerTask](/graph/api/resources/plannertask?view=graph-rest-beta) <br />[plannerPlanDetails](/graph/api/resources/plannerplandetails?view=graph-rest-beta) <br />[plannerTaskDetails](/graph/api/resources/plannertaskdetails?view=graph-rest-beta) <br />[plannerBucket](/graph/api/resources/plannerbucket?view=graph-rest-beta) <br />[plannerAssignedToTaskBoardTaskFormat](/graph/api/resources/plannerassignedtotaskboardtaskformat?view=graph-rest-beta) <br />[plannerBucketTaskBoardTaskFormat](/graph/api/resources/plannerbuckettaskboardtaskformat?view=graph-rest-beta) <br />[plannerProgressTaskBoardTaskFormat](/graph/api/resources/plannerprogresstaskboardtaskformat?view=graph-rest-beta) |

### <a name="intune-apis"></a>APIs do Intune
| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foram adicionadas novas entidades:<br/>[androidForWorkCompliancePolicy](/graph/api/resources/intune-deviceconfig-androidforworkcompliancepolicy?view=graph-rest-beta)<br/>[deviceComplianceSettingState](/graph/api/resources/intune-deviceconfig-devicecompliancesettingstate?view=graph-rest-beta)<br/>[deviceInstallState](/graph/api/resources/intune-books-deviceinstallstate?view=graph-rest-beta)<br/>[deviceManagementScript](/graph/api/resources/intune-deviceconfig-devicemanagementscript?view=graph-rest-beta)<br/>[deviceManagementScriptGroupAssignment](/graph/api/resources/intune-deviceconfig-devicemanagementscriptgroupassignment?view=graph-rest-beta)<br/>[deviceManagementScriptState](/graph/api/resources/intune-deviceconfig-devicemanagementscriptstate?view=graph-rest-beta)<br/>[eBookGroupAssignment](/graph/api/resources/intune-books-ebookgroupassignment?view=graph-rest-beta)<br/>[iosVppEBook](/graph/api/resources/intune-books-iosvppebook?view=graph-rest-beta)<br/>[managedEBook](/graph/api/resources/intune-books-managedebook?view=graph-rest-beta)<br/>[userInstallStateSummary](/graph/api/resources/intune-books-userinstallstatesummary?view=graph-rest-beta)<br/>[windowsManagementApp](/graph/api/resources/intune-deviceconfig-windowsmanagementapp?view=graph-rest-beta)<br/>[windowsManagementAppHealthState](/graph/api/resources/intune-deviceconfig-windowsmanagementapphealthstate?view=graph-rest-beta)<br/> |
| Adição        | Beta        | Foram adicionados novos tipos complexos:<br/>[dailySchedule](/graph/api/resources/intune-deviceconfig-dailyschedule?view=graph-rest-beta)<br/>[hourlySchedule](/graph/api/resources/intune-deviceconfig-hourlyschedule?view=graph-rest-beta)<br/>[iosBookmark](/graph/api/resources/intune-deviceconfig-iosbookmark?view=graph-rest-beta)<br/>[iosWebContentFilterAutoFilter](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterautofilter?view=graph-rest-beta)<br/>[iosWebContentFilterBase](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterbase?view=graph-rest-beta)<br/>[iosWebContentFilterSpecificWebsitesAccess](/graph/api/resources/intune-deviceconfig-ioswebcontentfilterspecificwebsitesaccess?view=graph-rest-beta)<br/>[runSchedule](/graph/api/resources/intune-deviceconfig-runschedule?view=graph-rest-beta)<br/>[sharedAppleDeviceUser](/graph/api/resources/intune-deviceconfig-sharedappledeviceuser?view=graph-rest-beta)<br/>[windows10NetworkProxyServer](/graph/api/resources/intune-deviceconfig-windows10networkproxyserver?view=graph-rest-beta)<br/> |
| Adição        | Beta        | A ação [requestRemoteAssistance](/graph/api/intune-devices-manageddevice-requestremoteassistance?view=graph-rest-beta) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Adição        | Beta        | A ação [cleanWindowsDevice](/graph/api/intune-devices-manageddevice-cleanwindowsdevice?view=graph-rest-beta) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Adição        | Beta        | A ação [logoutSharedAppleDeviceActiveUser](/graph/api/intune-devices-manageddevice-logoutsharedappledeviceactiveuser?view=graph-rest-beta) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Adição        | Beta        | A ação [deleteUserFromSharedAppleDevice](/graph/api/intune-devices-manageddevice-deleteuserfromsharedappledevice?view=graph-rest-beta) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Adição        | Beta        | A ação [assign](/graph/api/intune-deviceconfig-devicemanagementscript-assign?view=graph-rest-beta) foi adicionada a [deviceManagementScript](/graph/api/resources/intune-deviceconfig-devicemanagementscript?view=graph-rest-beta) |
| Adição        | Beta        | A ação [syncLicenses](/graph/api/intune-onboarding-applevolumepurchaseprogramtoken-synclicenses?view=graph-rest-beta) foi adicionada a [appleVolumePurchaseProgramToken](/graph/api/resources/intune-apps-applevolumepurchaseprogramtoken?view=graph-rest-beta) |
| Adição        | Beta        | A função **getTopMobileApps** foi adicionada à coleção [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) |
| Adição        | Beta        | A função [downloadApplePushNotificationCertificateSigningRequest](/graph/api/intune-deviceconfig-applepushnotificationcertificate-downloadapplepushnotificationcertificatesigningrequest?view=graph-rest-beta) foi adicionada a [applePushNotificationCertificate](/graph/api/resources/intune-deviceconfig-applepushnotificationcertificate?view=graph-rest-beta) |
| Adição        | Beta        | A função [getDeviceComplianceSettingStates](/graph/api/intune-deviceconfig-devicemanagement-getdevicecompliancesettingstates?view=graph-rest-beta) foi adicionada a [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) |
| Adição        | Beta        | A função [deviceConfigurationUserActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationuseractivity?view=graph-rest-beta) foi adicionada a [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) |
| Adição        | Beta        | A função [deviceConfigurationDeviceActivity](/graph/api/intune-deviceconfig-reportroot-deviceconfigurationdeviceactivity?view=graph-rest-beta) foi adicionada a [reportRoot](/graph/api/resources/intune-deviceconfig-reportroot?view=graph-rest-beta) |
| Exclusão        | Beta        | Foram removidos os seguintes tipos complexos:<br/>**enterpriseCloudResource**<br/>**windowsInformationProtectionAppRule**<br/>**windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate**<br/>**windowsInformationProtectionAppRuleDesktopTemplate**<br/>**windowsInformationProtectionAppRuleStoreAppTemplate**<br/>**windowsInformationProtectionAppRuleTemplate**<br/>**windowsInformationProtectionCorporateNetworkLocation**<br/>**windowsInformationProtectionProtectedLocation**<br/>**windowsInformationProtectionProtectedLocationEnterpriseCloudResources**<br/>**windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames**<br/>**windowsInformationProtectionProtectedLocationEnterpriseProxyServers**<br/>**windowsInformationProtectionProtectedLocationNeutralResources**<br/> |
| Alteração          | Beta        | A propriedade **deviceSharingAllowed** foi adicionada à entidade [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) |
| Alteração          | Beta        | Foi removida a propriedade **deviceSharingBlocked** à entidade [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) |
| Alteração          | Beta        | A propriedade **minimumRequiredSdkVersion** foi adicionada à entidade [defaultManagedAppProtection](/graph/api/resources/intune-mam-defaultmanagedappprotection?view=graph-rest-beta) |
| Alteração          | Beta        | A propriedade **windowsManagementAppEnabled** foi adicionada à entidade [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) |
| Alteração          | Beta        | Adicionada a propriedade **notificationTemplateId** à entidade [deviceComplianceActionItem](/graph/api/resources/intune-deviceconfig-devicecomplianceactionitem?view=graph-rest-beta) |
| Alteração          | Beta        | A propriedade **excludeGroup** foi adicionada à entidade [deviceConfigurationGroupAssignment](/graph/api/resources/intune-deviceconfig-deviceconfigurationgroupassignment?view=graph-rest-beta) |
| Alteração          | Beta        | Foram alteradas as seguintes propriedades na entidade [iosCustomConfiguration](/graph/api/resources/intune-deviceconfig-ioscustomconfiguration?view=graph-rest-beta):<br/>**payloadFileName** de obrigatório para opcional<br/> |
| Alteração          | Beta        | A propriedade **contentFilterSettings** foi adicionada à entidade [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta) |
| Alteração          | Beta        | Adicionadas as propriedades **cellularBlockPersonalHotspot** e **passcodeBlockFingerprintModification** à entidade [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) |
| Alteração          | Beta        | A propriedade **minimumRequiredSdkVersion** foi adicionada à entidade [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) |
| Alteração          | Beta        | Foram alteradas as seguintes propriedades na entidade [macOSCustomConfiguration](/graph/api/resources/intune-deviceconfig-macoscustomconfiguration?view=graph-rest-beta):<br/>**payloadFileName** de obrigatório para opcional<br/> |
| Alteração          | Beta        | Foram adicionadas as propriedades **disableAppPinIfDevicePinIsSet**, **minimumRequiredOsVersion**, **minimumWarningOsVersion**, **minimumRequiredAppVersion** e **minimumWarningAppVersion** à entidade [managedAppProtection](/graph/api/resources/intune-mam-managedappprotection?view=graph-rest-beta) |
| Alteração          | Beta        | Foram adicionadas as propriedades **remoteAssistanceSessionUrl**, **isEncrypted**, **modelo** e **fabricante** à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Alteração          | Beta        | As propriedades a seguir foram alteradas na entidade [getMobileAppCount](/graph/api/intune-apps-mobileapp-getmobileappcount?view=graph-rest-beta):<br/>**bindingParameter** de **mobileApp** para uma **collection** de *mobileApp*<br/>**status** de um GUID para uma Cadeia de caracteres<br/> |
| Alteração          | Beta        | A propriedade **vpnConfigurationId** foi adicionada à entidade [mobileAppGroupAssignment](/graph/api/resources/intune-apps-mobileappgroupassignment?view=graph-rest-beta) |
| Alteração          | Beta        | Foi removida a propriedade **fromEmailAddress** da entidade [notificationMessageTemplate](/graph/api/resources/intune-deviceconfig-notificationmessagetemplate?view=graph-rest-beta) |
| Alteração          | Beta        | A propriedade **excludedApps** foi adicionada à entidade [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) |
| Alteração          | Beta        | Foi removida a propriedade **excludedOfficeApps** da entidade [officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta) |
| Alteração          | Beta        | A propriedade **enabled** foi adicionada à entidade [sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta) |
| Alteração          | Beta        | Foram adicionadas as propriedades **networkProxyApplySettingsDeviceWide**, **networkProxyDisableAutoDetect**, **networkProxyAutomaticConfigurationUrl**, **networkProxyServer**, **bluetoothDeviceName**, **wiFiScanInterval**, **wirelessDisplayBlockProjectionToThisDevice**, **wirelessDisplayBlockUserInputFromReceiver**, **wirelessDisplayRequirePinForPairing**, **experienceBlockDeviceDiscovery**, **experienceBlockErrorDialogWhenNoSIM**, **experienceBlockTaskSwitcher**, ** startMenuPinnedFolderDocuments**, **startMenuPinnedFolderDownloads**, **startMenuPinnedFolderFileExplorer**, **startMenuPinnedFolderHomeGroup**, **startMenuPinnedFolderMusic**, **startMenuPinnedFolderNetwork**, **startMenuPinnedFolderPersonalFolder**, **startMenuPinnedFolderPictures**, **startMenuPinnedFolderSettings**, **startMenuPinnedFolderVideos**, **startMenuAppListVisibility**, **startMenuHideFrequentlyUsedApps**, ** startMenuHideRecentJumpLists**, **startMenuHideRecentlyAddedApps**, **startMenuHideRestartOptions**, **startMenuHideUserTile**, **startMenuHidePowerButton**, **startMenuLayoutEdgeAssetsXml**, **personalizationDesktopImageUrl** e **personalizationLockScreenImageUrl** à entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) |
| Alteração          | Beta        | Foi alterado o tipo das seguintes propriedades na entidade [windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta):<br/>**productCode** do Guid para a cadeia de caracteres<br/> |
| Alteração          | Beta        | Foram alteradas as seguintes propriedades na entidade [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta):<br/>**phoneProductIdentifier** de obrigatório para opcional<br/>**phonePublisherId** de obrigatório para opcional<br/> |
| Alteração          | Beta        | Foram alteradas as seguintes propriedades na entidade [windowsPhone81AppXBundle](/graph/api/resources/intune-apps-windowsphone81appxbundle?view=graph-rest-beta):<br/>**appXPackageInformationList** de obrigatório para opcional<br/> |
| Alteração          | Beta        | Foram adicionadas as propriedades **productKey** e **licenseType** à entidade [windowsStoreForBusinessApp](/graph/api/resources/intune-apps-windowsstoreforbusinessapp?view=graph-rest-beta) |
| Alteração          | Beta        | A propriedade **previewBuildSetting** foi adicionada à entidade [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) |
| Alteração          | Beta        | Foram adicionadas as propriedades de navegação **windowsManagementApp** e **managedEBooks** à entidade [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) |
| Alteração          | Beta        | Foram adicionadas as propriedades de navegação **deviceManagementScripts**, **managedDeviceOverview** e **cloudPkiSubscriptions** à entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) |
| Alteração          | Beta        | Foram adicionadas as propriedades **osMinimumVersion** e **osMaximumVersion** ao tipo complexo [deviceEnrollmentPlatformRestrictions](/graph/api/resources/intune-onboarding-deviceenrollmentplatformrestrictions?view=graph-rest-beta) |
| Alteração          | Beta        | Foram adicionadas as propriedades **isSharedDevice** e **sharedDeviceCachedUsers** ao tipo complexo [hardwareInformation](/graph/api/resources/intune-deviceconfig-hardwareinformation?view=graph-rest-beta) |
| Alteração          | Beta        | Foram alteradas as seguintes propriedades no tipo complexo [omaSettingBase64](/graph/api/resources/intune-deviceconfig-omasettingbase64?view=graph-rest-beta):<br/>**fileName** de obrigatório para opcional<br/> |
| Alteração          | Beta        | Foram alteradas as seguintes propriedades no tipo complexo [omaSettingStringXml](/graph/api/resources/intune-deviceconfig-omasettingstringxml?view=graph-rest-beta):<br/>**fileName** de obrigatório para opcional<br/> |

## <a name="march-2017"></a>Março de 2017

### <a name="intune-apis"></a>APIs do Intune

| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Adição    | Beta    | Foram adicionadas novas entidades:<br/>[androidForWorkApp](/graph/api/resources/intune-apps-androidforworkapp?view=graph-rest-beta)<br/>[androidForWorkAppConfigurationSchema](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationschema?view=graph-rest-beta)<br/>[androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta)<br/>[androidForWorkVpnConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkvpnconfiguration?view=graph-rest-beta)<br/>[applePushNotificationCertificate](/graph/api/resources/intune-deviceconfig-applepushnotificationcertificate?view=graph-rest-beta)<br/>[complianceSettingStateSummary](/graph/api/resources/intune-deviceconfig-compliancesettingstatesummary?view=graph-rest-beta)<br/>[deviceCompliancePolicyDeviceStateSummary](/graph/api/resources/intune-deviceconfig-devicecompliancepolicydevicestatesummary?view=graph-rest-beta)<br/>[deviceCompliancePolicyState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicystate?view=graph-rest-beta)<br/>[deviceConfigurationDeviceStateSummary](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatesummary?view=graph-rest-beta)<br/>[deviceConfigurationState](/graph/api/resources/intune-deviceconfig-deviceconfigurationstate?view=graph-rest-beta)<br/>[enterpriseCodeSigningCertificate](/graph/api/resources/intune-apps-enterprisecodesigningcertificate?view=graph-rest-beta)<br/>[iosEduDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosedudeviceconfiguration?view=graph-rest-beta)<br/>[managedDeviceCertificateState](/graph/api/resources/intune-devices-manageddevicecertificatestate?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationDeviceSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicesummary?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationUserSummary](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationusersummary?view=graph-rest-beta)<br/>[mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam?view=graph-rest-betamwindowsinformationprotectionpolicy)<br/>[mobileAppInstallSummary](/graph/api/resources/intune-apps-mobileappinstallsummary?view=graph-rest-beta)<br/>[mobileAppProvisioningConfigGroupAssignment](/graph/api/resources/intune-apps-mobileappprovisioningconfiggroupassignment?view=graph-rest-beta)<br/>[mobileThreatDefenseConnector](/graph/api/resources/intune-onboarding-mobilethreatdefenseconnector?view=graph-rest-beta)<br/>[officeSuiteApp](/graph/api/resources/intune-apps-officesuiteapp?view=graph-rest-beta)<br/>[settingStateDeviceSummary](/graph/api/resources/intune-deviceconfig-settingstatedevicesummary?view=graph-rest-beta)<br/>[softwareUpdateStatusSummary](/graph/api/resources/intune-deviceconfig-softwareupdatestatussummary?view=graph-rest-beta)<br/>[symantecCodeSigningCertificate](/graph/api/resources/intune-apps-symanteccodesigningcertificate?view=graph-rest-beta)<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windowsdefenderadvancedthreatprotectionconfiguration?view=graph-rest-beta)<br/>[windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta)<br/>[windowsInformationProtectionAppLockerFile](/graph/api/resources/intune-mam-windowsinformationprotectionapplockerfile?view=graph-rest-beta)<br/>[windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-beta)<br/>[windowsMobileMSI](/graph/api/resources/intune-apps-windowsmobilemsi?view=graph-rest-beta)<br/> |
| Adição    | Beta    | Foram adicionados novos tipos complexos:<br/>[androidForWorkAppConfigurationExample](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationexample?view=graph-rest-beta)<br/>[androidForWorkAppConfigurationExampleJson](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationexamplejson?view=graph-rest-beta)<br/>[androidForWorkAppConfigurationSchemaItem](/graph/api/resources/intune-androidforwork-androidforworkappconfigurationschemaitem?view=graph-rest-beta)<br/>[deviceCompliancePolicySettingState](/graph/api/resources/intune-deviceconfig-devicecompliancepolicysettingstate?view=graph-rest-beta)<br/>[deviceConfigurationSettingState](/graph/api/resources/intune-deviceconfig-deviceconfigurationsettingstate?view=graph-rest-beta)<br/>[deviceExchangeAccessStateSummary](/graph/api/resources/intune-deviceconfig-deviceexchangeaccessstatesummary?view=graph-rest-beta)<br/>[edgeSearchEngine](/graph/api/resources/intune-deviceconfig-edgesearchengine?view=graph-rest-beta)<br/>[edgeSearchEngineBase](/graph/api/resources/intune-deviceconfig-edgesearchenginebase?view=graph-rest-beta)<br/>[edgeSearchEngineCustom](/graph/api/resources/intune-deviceconfig-edgesearchenginecustom?view=graph-rest-beta)<br/>[excludedApps](/graph/api/resources/intune-apps-excludedapps?view=graph-rest-beta)<br/>[iosEduCertificateSettings](/graph/api/resources/intune-deviceconfig-ioseducertificatesettings?view=graph-rest-beta)<br/>[ipRange](/graph/api/resources/intune-deviceconfig-iprange?view=graph-rest-beta)<br/>[windowsInformationProtectionApp](/graph/api/resources/intune-mam-windowsinformationprotectionapp?view=graph-rest-beta)<br/>[windowsInformationProtectionCloudResource](/graph/api/resources/intune-mam-windowsinformationprotectioncloudresource?view=graph-rest-beta)<br/>[windowsInformationProtectionCloudResourceCollection](/graph/api/resources/intune-mam-windowsinformationprotectioncloudresourcecollection?view=graph-rest-beta)<br/>[windowsInformationProtectionDesktopApp](/graph/api/resources/intune-mam-windowsinformationprotectiondesktopapp?view=graph-rest-beta)<br/>[windowsInformationProtectionIPRangeCollection](/graph/api/resources/intune-mam-windowsinformationprotectioniprangecollection?view=graph-rest-beta)<br/>[windowsInformationProtectionResourceCollection](/graph/api/resources/intune-mam-windowsinformationprotectionresourcecollection?view=graph-rest-beta)<br/>[windowsInformationProtectionStoreApp](/graph/api/resources/intune-mam-windowsinformationprotectionstoreapp?view=graph-rest-beta)<br/> |
| Adição    | Beta    | A ação [requestSignupUrl](/graph/api/intune-androidforwork-androidforworksettings-requestsignupurl?view=graph-rest-beta) foi adicionada a [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) |
| Adição    | Beta    | A ação [completeSignup](/graph/api/intune-androidforwork-androidforworksettings-completesignup?view=graph-rest-beta) foi adicionada a [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) |
| Adição    | Beta    | A ação [syncApps](/graph/api/intune-androidforwork-androidforworksettings-syncapps?view=graph-rest-beta) foi adicionada a [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) |
| Adição    | Beta    | A ação [unbind](/graph/api/intune-androidforwork-androidforworksettings-unbind?view=graph-rest-beta) foi adicionada a [androidForWorkSettings](/graph/api/resources/intune-androidforwork-androidforworksettings?view=graph-rest-beta) |
| Adição    | Beta    | A ação [assign](/graph/api/intune-apps-ioslobappprovisioningconfiguration-assign?view=graph-rest-beta) foi adicionada a [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) |
| Adição    | Beta    | A ação [recoverPasscode](/graph/api/intune-devices-manageddevice-recoverpasscode?view=graph-rest-beta) foi adicionada a [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Adição    | Beta    | A ação [removeApplePushNotificationCertificate](/graph/api/intune-onboarding-organization-removeapplepushnotificationcertificate?view=graph-rest-beta) foi adicionada a [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) |
| Adição    | Beta    | A ação [updateMobileAppIdentifierDeployments](/graph/api/intune-mam-iosmanagedappprotection-updatemobileappidentifierdeployments?view=graph-rest-beta) foi adicionada a [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) |
| Adição    | Beta    | A ação [updateMobileAppIdentifierDeployments](/graph/api/intune-mam-androidmanagedappprotection-updatemobileappidentifierdeployments?view=graph-rest-beta) foi adicionada a [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) |
| Adição    | Beta    | A ação [updateMobileAppIdentifierDeployments](/graph/api/intune-mam-targetedmanagedappconfiguration-updatemobileappidentifierdeployments?view=graph-rest-beta) foi adicionada a [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) |
| Adição    | Beta    | A ação [updateTargetedSecurityGroups](/graph/api/intune-mam-iosmanagedappprotection-updatetargetedsecuritygroups?view=graph-rest-beta) foi adicionada a [iosManagedAppProtection](/graph/api/resources/intune-mam-iosmanagedappprotection?view=graph-rest-beta) |
| Adição    | Beta    | A ação [updateTargetedSecurityGroups](/graph/api/intune-mam-androidmanagedappprotection-updatetargetedsecuritygroups?view=graph-rest-beta) foi adicionada a [androidManagedAppProtection](/graph/api/resources/intune-mam-androidmanagedappprotection?view=graph-rest-beta) |
| Adição    | Beta    | A ação [updateTargetedSecurityGroups](/graph/api/intune-mam-windowsinformationprotection-updatetargetedsecuritygroups?view=graph-rest-beta) foi adicionada a [windowsInformationProtection](/graph/api/resources/intune-mam-windowsinformationprotection?view=graph-rest-beta) |
| Adição    | Beta    | A ação [updateTargetedSecurityGroups](/graph/api/intune-mam-windowsinformationprotection-updatetargetedsecuritygroups?view=graph-rest-beta) foi adicionada a [windowsInformationProtectionPolicy](/graph/api/resources/intune-mam-windowsinformationprotectionpolicy?view=graph-rest-beta) |
| Adição    | Beta    | A ação [updateTargetedSecurityGroups](/graph/api/intune-mam?view=graph-rest-betamwindowsinformationprotectionpolicy-updatetargetedsecuritygroups) foi adicionada a [mdmWindowsInformationProtectionPolicy](/graph/api/resources/intune-mam?view=graph-rest-betamwindowsinformationprotectionpolicy) |
| Adição    | Beta    | A ação [wipeManagedAppRegistrationByDeviceTag](/graph/api/intune-mam-user-wipemanagedappregistrationbydevicetag?view=graph-rest-beta) foi adicionada a [user](/graph/api/resources/intune-deviceconfig-user?view=graph-rest-beta) |
| Adição    | Beta    | A função [getTopMobileApps](/graph/api/intune-apps-mobileapp-gettopmobileapps?view=graph-rest-beta) foi adicionada a [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) |
| Adição    | Beta    | A função [verifyWindowsEnrollmentAutoDiscovery](/graph/api/intune-corpenrollment-devicemanagement-verifywindowsenrollmentautodiscovery?view=graph-rest-beta) foi adicionada a [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) |
| Exclusão    | Beta    | Foram removidas as seguintes entidades:<br/>**appProvisioningConfigGroupAssignment**<br/>**defaultManagedAppConfiguration**<br/>**enterpriseCertificate**<br/>**managedDeviceMobileAppProvisioningConfigurationDeviceStatus**<br/>**symantecCertificate**<br/>**windows10WindowsInformationProtectionConfiguration**<br/> |
| Exclusão    | Beta    | Foram removidos os seguintes tipos complexos:<br/>**mobileAppInstallSummary**<br/>**windowsArchitecture**<br/>**windowsDeviceType**<br/> |
| Alteração      | Beta    | A propriedade **webBrowserBlockPopups** foi adicionada à entidade [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foi removida a propriedade **webBrowserAllowPopups** da entidade [androidGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-androidgeneraldeviceconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **appIdentifier** foi adicionada à entidade [androidStoreApp](/graph/api/resources/intune-apps-androidstoreapp?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as propriedades **applicationCount**, **failedApplicationCount** e **appInstallFailures** da entidade [appReportingOverviewStatus](/graph/api/resources/appreportingoverviewstatus?view=graph-rest-beta) |
| Alteração      | Beta    | As propriedades **sharedIPadMaximumUserCount** e **enableSharedIPad** foram adicionadas à entidade [depEnrollmentProfile](/graph/api/resources/intune-corpenrollment-depenrollmentprofile?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **shareTokenWithSchoolDataSyncService** e **lastSyncErrorCode** à entidade [depOnboardingSetting](/graph/api/resources/intune-onboarding-deponboardingsetting?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** e **configurationVersion** à entidade [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as propriedades **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** e **policyRevision** da entidade [deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** e **configurationVersion** à entidade [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as propriedades **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** e **policyRevision** da entidade [deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** e **configurationVersion** à entidade [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as propriedades **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** e **policyRevision** da entidade [deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** e **configurationVersion** à entidade [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as propriedades **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** e **policyRevision** da entidade [deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **subscriptionState** foi adicionada à entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **managedEmailProfileRequired** foi adicionada à entidade [iosCompliancePolicy](/graph/api/resources/intune-deviceconfig-ioscompliancepolicy?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **appsSingleAppModeList** foi adicionada à entidade [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foi removida a propriedade **appsSingleAppModeBundleIds** da entidade [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **expirationDateTime** foi adicionada à entidade [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foi removida a propriedade **expiration** da entidade [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **passwordMinimumCharacterSetCount**, **osMinimumVersion**, **osMaximumVersion**, **deviceThreatProtectionEnabled**, **deviceThreatProtectionRequiredSecurityLevel** e **storageRequireEncryption** à entidade [macOSCompliancePolicy](/graph/api/resources/intune-deviceconfig-macoscompliancepolicy?view=graph-rest-beta) |
| Alteração      | Beta    | Foi removida a propriedade **manifest** da entidade [managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **isSupervised**, **exchangeLastSuccessfulSyncDateTime**, **exchangeAccessState** e **exchangeAccessStateReason** à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **deviceExchangeAccessStateSummary** foi adicionada à entidade [managedDeviceOverview](/graph/api/resources/intune-devices-manageddeviceoverview?view=graph-rest-beta) |
| Alteração      | Beta    | Foi removida a propriedade **manifest** da entidade [managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta) |
| Alteração      | Beta    | Foi removida a propriedade **installSummary** da entidade [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **uploadState** foi adicionada à entidade [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta) |
| Alteração      | Beta    | Foram alteradas as seguintes propriedades na entidade [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta):<br/>**azureStorageUriExpirationDateTime** de obrigatório para opcional<br/> |
| Alteração      | Beta    | Foram adicionadas as propriedades **initiatedByUserPrincipalName**, **deviceOwnerUserPrincipalName**, **deviceIMEI** e **actionState** à entidade [remoteActionAudit](/graph/api/resources/intune-deviceconfig-remoteactionaudit?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **oneDriveDisableFileSync**, **safeSearchFilter**, **edgeSearchEngine**, **settingsBlockSettingsApp**, **settingsBlockSystemPage**, **settingsBlockDevicesPage**, **settingsBlockNetworkInternetPage**, **settingsBlockPersonalizationPage**, **settingsBlockAccountsPage**, **settingsBlockTimeLanguagePage**, **settingsBlockEaseOfAccessPage**, **settingsBlockPrivacyPage**, **settingsBlockUpdateSecurityPage**, ** experienceBlockWindowsSpotlight**, **experienceBlockWindowsTips**, **experienceBlockConsumerSpecificFeatures**, **startMenuLayoutXml**, **startMenuMode**, **logonBlockFastUserSwitching** e **startBlockUnpinningAppsFromTaskbar** à entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **allowPrinting**, **allowScreenCapture** e **allowTextSuggestion** à entidade [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as propriedades **blockPrinting**, **blockScreenCapture** e **blockTextSuggestion** da entidade [windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **identityName** foi adicionada à entidade [windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta) |
| Alteração      | Beta    | Foi alterado o tipo das seguintes propriedades na entidade [windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta):<br/>**applicableArchitectures** de [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta) para cadeia de caracteres<br/> |
| Alteração      | Beta    | A propriedade **identityName** foi adicionada à entidade [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta) |
| Alteração      | Beta    | Foi alterado o tipo das seguintes propriedades na entidade [windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta):<br/>**applicableArchitectures** de [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta) para cadeia de caracteres<br/> |
| Alteração      | Beta    | Foram adicionadas as propriedades **identityName**, **identityPublisherHash** e **identityResourceIdentifier** à entidade [windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta) |
| Alteração      | Beta    | Foi alterado o tipo das seguintes propriedades na entidade [windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta):<br/>**applicableArchitectures** de [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta) para cadeia de caracteres<br/>**applicableDeviceTypes** de [windowsDeviceType](/graph/api/resources/windowsdevicetype?view=graph-rest-beta) para a cadeia de caracteres<br/> |
| Alteração      | Beta    | A propriedade **restartMode** foi adicionada à entidade [windowsUpdateForBusinessConfiguration](/graph/api/resources/intune-deviceconfig-windowsupdateforbusinessconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **managedDeviceCertificateStates** foi adicionada à entidade [androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **managedDeviceCertificateStates** foi adicionada à entidade [androidScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidscepcertificateprofile?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **enterpriseCodeSigningCertificates**, **symantecCodeSigningCertificate**, **sideLoadingKeys**, **managedAppPolicies**, **iosManagedAppProtections**, **androidManagedAppProtections**, **defaultManagedAppProtections**, **targetedManagedAppConfigurations**, **mdmWindowsInformationProtectionPolicies**, **windowsInformationProtectionPolicies**, **managedAppRegistrations** e **managedAppStatuses** à entidade [deviceAppManagement ](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as propriedades de navegação **appReportingOverview**, **enterpriseCerts** e **symantecCert** da entidade [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **deviceSettingStateSummaries** foi adicionada à entidade [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **deviceSettingStateSummaries** foi adicionada à entidade [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **termsAndConditions**, **androidForWorkSettings**, **androidForWorkAppConfigurationSchemas**, **applePushNotificationCertificate**, **softwareUpdateStatusSummary**, **deviceCompliancePolicyDeviceStateSummary**, **complianceSettingStateSummaries**, **deviceConfigurationDeviceStateSummaries** e **mobileThreatDefenseConnectors** à entidade [deviceManagement](/graph/api/resources/intune-shared-devicemanagement?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as propriedades de navegação **teacherRootCertificates**, **teacherIdentityCertificate**, **studentRootCertificates** e **studentIdentityCertificate** da entidade [iosEducationDeviceConfiguration](/graph/api/resources/intune-deviceconfig-ioseducationdeviceconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foi alterado o tipo das seguintes propriedades na entidade [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta):<br/>**deviceStatuses** da coleção [managedDeviceMobileAppProvisioningConfigurationDeviceStatus](/graph/api/resources/manageddevicemobileappprovisioningconfigurationdevicestatus?view=graph-rest-beta) para a coleção [managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta)<br/>**groupAssignments** da coleção [appProvisioningConfigGroupAssignment](/graph/api/resources/appprovisioningconfiggroupassignment?view=graph-rest-beta) para a coleção [mobileAppProvisioningConfigGroupAssignment](/graph/api/resources/intune-apps-mobileappprovisioningconfiggroupassignment?view=graph-rest-beta)<br/> |
| Alteração      | Beta    | A propriedade de navegação **managedDeviceCertificateStates** foi adicionada à entidade [iosScepCertificateProfile](/graph/api/resources/intune-deviceconfig-iosscepcertificateprofile?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **managedDeviceCertificateStates** foi adicionada à entidade [macOSScepCertificateProfile](/graph/api/resources/intune-deviceconfig-macosscepcertificateprofile?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **deviceConfigurationStates** e **deviceCompliancePolicyStates** à entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **deviceStatusSummary** e **userStatusSummary** à entidade [managedDeviceMobileAppConfiguration](/graph/api/resources/intune-apps-manageddevicemobileappconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **installSummary** foi adicionada à entidade [mobileApp](/graph/api/resources/intune-apps-mobileapp?view=graph-rest-beta) |
| Alteração      | Beta    | Foi removida a propriedade de navegação **sideLoadingKeys** da entidade [organization](/graph/api/resources/intune-onboarding-organization?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **managedDeviceCertificateStates** foi adicionada à entidade [windows81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windows81scepcertificateprofile?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **managedDeviceCertificateStates** foi adicionada à entidade [windowsPhone81SCEPCertificateProfile](/graph/api/resources/intune-deviceconfig-windowsphone81scepcertificateprofile?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as propriedades **applicationId**, **appName**, **platformId**, **userFailures** e **deviceFailures** do tipo complexo [appInstallationFailure](/graph/api/resources/intune-apps-appinstallationfailure?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **displayName** foi adicionada ao tipo complexo [iosHomeScreenFolderPage](/graph/api/resources/intune-deviceconfig-ioshomescreenfolderpage?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **displayName** foi adicionada ao tipo complexo [iosHomeScreenPage](/graph/api/resources/intune-deviceconfig-ioshomescreenpage?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **subjectName**, **description**, **expirationDateTime** e **certificate** ao tipo complexo [windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-mam-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as propriedades **dataRecoveryCertificate** e **certificateFileName** do tipo complexo [windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-mam-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **displayName** foi adicionada ao tipo complexo [windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta) |
| Alteração      | Beta    | Foi alterado o tipo das seguintes propriedades no tipo complexo [windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta):<br/>**applicableArchitecture** de [windowsArchitecture](/graph/api/resources/windowsarchitecture?view=graph-rest-beta) para cadeia de caracteres<br/> |
| Alteração      | Beta    | Foram alteradas as seguintes propriedades no tipo complexo [windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta):<br/>**applicableArchitecture** de opcional para obrigatório<br/> |

### <a name="add-contracts-to-microsoft-graph"></a>Adicionar contratos ao Microsoft Graph

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Novo recurso:</br>[contract](/graph/api/resources/contract?view=graph-rest-beta) |

### <a name="add-domain-operations-to-microsoft-graph"></a>Adicionar operações de domínio ao Microsoft Graph

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Adicionou funções nos [domínios](/graph/api/resources/domain?view=graph-rest-beta).<br/>Novas entidades:</br>[domain](/graph/api/resources/domain?view=graph-rest-beta)<br/>[domainDnsRecord](/graph/api/resources/domaindnsrecord?view=graph-rest-beta)<br/>[domainDnsCnameRecord](/graph/api/resources/domaindnscnamerecord?view=graph-rest-beta)<br/>[domainDnsMxRecord](/graph/api/resources/domaindnsmxrecord?view=graph-rest-beta)<br/>[domainDnsSrvRecord](/graph/api/resources/domaindnssrvrecord?view=graph-rest-beta)<br/>[domainDnsTxtRecord](/graph/api/resources/domaindnstxtrecord?view=graph-rest-beta)<br/>[domainDnsUnavailableRecord](/graph/api/resources/domaindnsunavailablerecord?view=graph-rest-beta)<br/>Novas ações:</br>[forceDelete](/graph/api/domain-forcedelete?view=graph-rest-beta)</br>[verify](/graph/api/domain-verify?view=graph-rest-beta) |

### <a name="add-custom-data-to-microsoft-graph-using-schema-extensions"></a>Adicionar dados personalizados ao Microsoft Graph usando extensões de esquema

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Estenda o Microsoft Graph com dados de aplicativos usando [extensões de esquema](extensibility-overview.md#schema-extensions).  Isso é suportado nos seguintes recursos:<br/>administrative unit<br/>calendar event<br/>device<br/>group<br/>message<br/>organization<br/>personal contact<br/>post<br/>user<br/>Veja o seguinte exemplo:<br/>[Adicionar dados personalizados a grupos usando Extensões do Esquema (visualização)](extensibility-schema-groups.md) |
| Adição        | Beta        | Foi fornecido uma maneira alternativa de criar uma definição de extensão do esquema sem a necessidade de um domínio personalizado .com verificado. Confira [extensões de esquema](extensibility-overview.md#schema-extensions) para obter detalhes. |

### <a name="add-custom-data-to-microsoft-graph-using-open-extensions"></a>Adicionar dados personalizados ao Microsoft Graph usando extensões abertas

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Alteração          | v1.0 e beta | As "extensões de dados do Office 365" anteriores foram renomeadas como "abrir extensões". |
| Adição        | Beta          | Foram adicionados recursos que oferecem suporte a [extensões abertas](extensibility-overview.md#open-extensions): <br/>administrative unit<br/>device<br/>grupo<br/>organization<br/>user<br/>Veja o seguinte exemplo:<br/>[Adicionar dados personalizados aos usuários usando extensões abertas (visualização)](extensibility-open-users.md) |

### <a name="directory-apis"></a>APIs de diretório

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foi adicionado o suporte para a [restauração e a exclusão permanente de grupos](/graph/api/resources/directory?view=graph-rest-beta).<br/>Nova entidade: diretório com a propriedade de navegação deleteditems. |
| Adição        | Beta        | Nova entidade:</br>[Ponto de extremidade](/graph/api/resources/endpoint?view=graph-rest-beta) |
| Alteração          | Beta        | Nova propriedade de navegação nos [pontos de extremidade](/graph/api/group-list-endpoints?view=graph-rest-beta) em [grupos](/graph/api/resources/group?view=graph-rest-beta) |
| Adição        | Beta        | Nova entidade:</br>[licenseDetails](/graph/api/resources/licensedetails?view=graph-rest-beta) |
| Alteração          | Beta        | Nova propriedade de navegação [licensedetails](/graph/api/user-list-licensedetails?view=graph-rest-beta) em [users](/graph/api/resources/user?view=graph-rest-beta) |

### <a name="reports-apis"></a>APIs de relatórios

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foi introduzida a nova API de visualização para relatórios do Office 365. Você pode usá-la para obter relatórios de uso sobre como as pessoas em sua empresa estão usando serviços do Office 365. Por exemplo, você pode identificar quem está usando muito um serviço e atingindo cotas, ou quem pode não precisar de uma licença do Office 365. Para obter mais detalhes, confira o [relatório](/graph/api/resources/report?view=graph-rest-beta). |

### <a name="directory-apis"></a>APIs de diretório

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Nova entidade:</br>[contract](/graph/api/resources/contract?view=graph-rest-beta) |

## <a name="february-2017"></a>Fevereiro de 2017

### <a name="intune-apis"></a>APIs do Intune

| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Adição    | Beta    | Foram adicionadas novas entidades:<br/>[androidForWorkCertificateProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkcertificateprofilebase?view=graph-rest-beta)<br/>[androidForWorkEasEmailProfileBase](/graph/api/resources/intune-deviceconfig-androidforworkeasemailprofilebase?view=graph-rest-beta)<br/>[androidForWorkEnterpriseWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkenterprisewificonfiguration?view=graph-rest-beta)<br/>[androidForWorkGmailEasConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkgmaileasconfiguration?view=graph-rest-beta)<br/>[androidForWorkNineWorkEasConfiguration](/graph/api/resources/intune-deviceconfig-androidforworknineworkeasconfiguration?view=graph-rest-beta)<br/>[androidForWorkPkcsCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkpkcscertificateprofile?view=graph-rest-beta)<br/>[androidForWorkScepCertificateProfile](/graph/api/resources/intune-deviceconfig-androidforworkscepcertificateprofile?view=graph-rest-beta)<br/>[androidForWorkTrustedRootCertificate](/graph/api/resources/intune-deviceconfig-androidforworktrustedrootcertificate?view=graph-rest-beta)<br/>[androidForWorkWiFiConfiguration](/graph/api/resources/intune-deviceconfig-androidforworkwificonfiguration?view=graph-rest-beta)<br/>[appleDeviceFeaturesConfigurationBase](/graph/api/resources/intune-deviceconfig-appledevicefeaturesconfigurationbase?view=graph-rest-beta)<br/>[appProvisioningConfigGroupAssignment](/graph/api/resources/intune-apps-appprovisioningconfiggroupassignment?view=graph-rest-beta)<br/>[deviceComplianceUserOverview](/graph/api/resources/intune-deviceconfig-devicecomplianceuseroverview?view=graph-rest-beta)<br/>[deviceConfigurationUserOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationuseroverview?view=graph-rest-beta)<br/>[enterpriseCertificate](/graph/api/resources/intune-apps-enterprisecertificate?view=graph-rest-beta)<br/>[iosEducationDeviceConfiguration](/graph/api/resources/intune-deviceconfig-ioseducationdeviceconfiguration?view=graph-rest-beta)<br/>[macOSDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-macosdevicefeaturesconfiguration?view=graph-rest-beta)<br/>[managedAndroidLobApp](/graph/api/resources/intune-apps-managedandroidlobapp?view=graph-rest-beta)<br/>[managedDeviceMobileAppProvisioningConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappprovisioningconfigurationdevicestatus?view=graph-rest-beta)<br/>[managedIOSLobApp](/graph/api/resources/intune-apps-managedioslobapp?view=graph-rest-beta)<br/>[managedMobileLobApp](/graph/api/resources/intune-apps-managedmobilelobapp?view=graph-rest-beta)<br/>[symantecCertificate](/graph/api/resources/intune-apps-symanteccertificate?view=graph-rest-beta)<br/>[windowsAppX](/graph/api/resources/intune-apps-windowsappx?view=graph-rest-beta)<br/>[windowsCertificateProfileBase](/graph/api/resources/intune-deviceconfig-windowscertificateprofilebase?view=graph-rest-beta)<br/>[windowsPhone81AppX](/graph/api/resources/intune-apps-windowsphone81appx?view=graph-rest-beta)<br/>[windowsPhone81AppXBundle](/graph/api/resources/intune-apps-windowsphone81appxbundle?view=graph-rest-beta)<br/>[windowsPhoneXAP](/graph/api/resources/intune-apps-windowsphonexap?view=graph-rest-beta)<br/>[windowsUniversalAppX](/graph/api/resources/intune-apps-windowsuniversalappx?view=graph-rest-beta)<br/> |
| Adição    | Beta    | Foram adicionados novos tipos complexos:<br/>[airPrintDestination](/graph/api/resources/intune-deviceconfig-airprintdestination?view=graph-rest-beta)<br/>[windowsArchitecture](/graph/api/resources/intune-apps-windowsarchitecture?view=graph-rest-beta)<br/>[windowsDeviceType](/graph/api/resources/intune-apps-windowsdevicetype?view=graph-rest-beta)<br/>[windowsMinimumOperatingSystem](/graph/api/resources/intune-apps-windowsminimumoperatingsystem?view=graph-rest-beta)<br/>[windowsPackageInformation](/graph/api/resources/intune-apps-windowspackageinformation?view=graph-rest-beta)<br/> |
| Adição    | Beta    | A ação [atribuir](/graph/api/intune-apps-ioslobappprovisioningconfiguration-assign?view=graph-rest-beta) foi adicionada à entidade [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) |
| Adição    | Beta    | A ação [scheduleActionsForRules](/graph/api/intune-deviceconfig-devicecompliancepolicy-scheduleactionsforrules?view=graph-rest-beta) foi adicionada à entidade [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) |
| Adição    | Beta    | A ação [updateTargetedSecurityGroups](/graph/api/intune-mam-targetedmanagedappconfiguration-updatetargetedsecuritygroups?view=graph-rest-beta) foi adicionada à entidade [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) |
| Adição    | Beta    | A função [getScopesForUser](/graph/api/intune-rbac-resourceoperation-getscopesforintune-devices-user?view=graph-rest-beta) foi adicionada à entidade [resourceOperation](/graph/api/resources/intune-rbac-resourceoperation?view=graph-rest-beta) |
| Alteração      | Beta    | Removido a propriedade **manifesto** a partir da entidade [androidLobApp](/graph/api/resources/intune-apps-androidlobapp?view=graph-rest-beta)  |
| Alteração      | Beta    | Foram adicionadas as propriedades **assetTagTemplate**, **lockScreenFootnote**, **homeScreenDockIcons** e **homeScreenPages** à entidade [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta)  |
| Alteração      | Beta    | Foram removidas as propriedades **deviceSharingAssetTagInformation** **deviceSharingLockScreenFootnote**, **homeScreenLayoutDockIcons** e **homeScreenLayoutPages** da entidade [iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta)  |
| Alteração      | Beta    | A propriedade **appsSingleAppModeBundleIds** foi adicionada à entidade [iosGeneralDeviceConfiguration](/graph/api/resources/intune-deviceconfig-iosgeneraldeviceconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foi removida a propriedade **manifesto** da entidade [iosLobApp](/graph/api/resources/intune-apps-ioslobapp?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **createdDateTime**, **descrição**, **lastModifiedDateTime**, **displayName** e **versão** à entidade [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **createdDateTime** e **lastModifiedDateTime** à entidade [managedAppPolicy](/graph/api/resources/intune-mam-managedapppolicy?view=graph-rest-beta)  |
| Alteração      | Beta    | Foi removida a propriedade **deviceRegistrationState** da entidade [managedDevice](/graph/api/resources/intune-devices-manageddevice?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **manifesto** foi adicionada à entidade [mobileAppContentFile](/graph/api/resources/intune-apps-mobileappcontentfile?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **osDescription** e **userName** à entidade [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) |
| Alteração      | Beta    | Foi removida a propriedade **deviceType** da entidade [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta) |
| Alteração      | Beta    | Foi alterado o tipo das seguintes propriedades na entidade [mobileAppInstallStatus](/graph/api/resources/intune-apps-mobileappinstallstatus?view=graph-rest-beta):<br/>**mobileAppInstallStatusValue** de Int32 para String |
| Alteração      | Beta    | Foram adicionadas as propriedades **targetedSecurityGroupIds** e **targetedSecurityGroupsCount** à entidade [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) entidade |
| Alteração      | Beta    | Foi removida a propriedade **numberOfTargetedSecurityGroups** da entidade [targetedManagedAppConfiguration](/graph/api/resources/intune-mam-targetedmanagedappconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade **id** foi adicionada à entidade [user](/graph/api/resources/intune-devices-user?view=graph-rest-beta)  |
| Alteração      | Beta    | Foram removidas as propriedades **renewalThresholdPercentage**, **keyStorageProvider**, **subjectNameFormat**, **subjectAlternativeNameType**, **certificateValidityPeriodValue** e **certificateValidityPeriodScale** da entidade [windows10CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows10certificateprofilebase?view=graph-rest-beta)  |
| Alteração      | Beta    | Foram removidas as propriedades **renewalThresholdPercentage**, **keyStorageProvider**, **subjectNameFormat**, **subjectAlternativeNameType**, **certificateValidityPeriodValue** e **certificateValidityPeriodScale** da entidade [windows81CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows81certificateprofilebase?view=graph-rest-beta) |
| Alteração      | Beta    | Foi removida a propriedade **applyToWindows10Mobile** da entidade [windowsPhone81GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windowsphone81generalconfiguration?view=graph-rest-beta)  |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **enterpriseCerts**, **iosLobAppProvisioningConfigurations** e **symantecCert** à entidade [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **userStatusOverview** foi adicionada à entidade [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta) |
| Alteração      | Beta    | A propriedade de navegação **userStatusOverview** foi adicionada à entidade [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **groupAssignments**, **deviceStatuses** e **userStatuses** à entidade [iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta) |
| Alteração      | Beta    | Foi alterado o tipo das seguintes propriedades na entidade [windows10VpnConfiguration](/graph/api/resources/intune-deviceconfig-windows10vpnconfiguration?view=graph-rest-beta):<br/>**identityCertificate** de [windows10CertificateProfileBase](/graph/api/resources/intune-deviceconfig-windows10certificateprofilebase?view=graph-rest-beta) para [windowsCertificateProfileBase](/graph/api/resources/intune-deviceconfig-windowscertificateprofilebase?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **deviceComplianceCheckinThresholdDays** e **isScheduledActionEnabled**ao tipo complexo [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) |
| Alteração      | Beta    | Foram removidas as propriedades **windowsCommercialId** e **windowsCommercialIdLastModifiedTime** do tipo complexo [deviceManagementSettings](/graph/api/resources/intune-deviceconfig-devicemanagementsettings?view=graph-rest-beta) |
| Alteração      | Beta    | Foram adicionadas as propriedades **bundleID**, **appName**, **publisher**, **habilitado** e **showOnLockScreen** ao tipo complexo [iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-beta)  |
| Alteração      | Beta    | Foram removidas as propriedades **bundleIdentifier**, **notificationsEnabled** e **showInLockScreen** do tipo complexo [iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-beta) |



## <a name="january-2017"></a>Janeiro de 2017

### <a name="outlook-calendar"></a>Calendário do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Nova ação [findMeetingTimes](/graph/api/user-findmeetingtimes?view=graph-rest-1.0) para o recurso [user](/graph/api/resources/user?view=graph-rest-1.0). |
| Adição        | v1.0        | Novo tipo complexo [attendeeBase](/graph/api/resources/attendeebase?view=graph-rest-1.0), que consiste em uma propriedade de tipo para o tipo attendee. |
| Adição        | v1.0        | Novos tipos complexos:<br/>[attendeeAvailability](/graph/api/resources/attendeeavailability?view=graph-rest-1.0)<br/>[locationConstraint](/graph/api/resources/locationconstraint?view=graph-rest-1.0) <br/>[locationConstraintItem](/graph/api/resources/locationconstraintitem?view=graph-rest-1.0)<br/>[meetingTimeSuggestion](/graph/api/resources/meetingtimesuggestion?view=graph-rest-1.0)<br/>[meetingTimeSuggestionsResult](/graph/api/resources/meetingtimesuggestionsresult?view=graph-rest-1.0)<br/>[timeConstraint](/graph/api/resources/timeconstraint?view=graph-rest-1.0)<br/>[timeSlot](/graph/api/resources/timeslot?view=graph-rest-1.0) |
| Alteração          | v1.0        | O tipo complexo [attendee](/graph/api/resources/attendee?view=graph-rest-1.0) agora deriva de attendeeBase,que, por sua vez, é derivado do [recipient](/graph/api/resources/recipient?view=graph-rest-1.0). Incluindo as propriedades herdadas, ele consiste nas mesmas propriedades de antes: **status**, **type** e **emailAddress**. |
| Adição        | Beta        | hexColor adicionado ao recurso [calendar](/graph/api/resources/calendar?view=graph-rest-beta). |

### <a name="intune-apis"></a>APIs do Intune

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foram adicionadas novas entidades: <br/>[appReportingOverviewStatus](/graph/api/resources/intune-apps-appreportingoverviewstatus?view=graph-rest-beta)<br/>[deviceComplianceDeviceOverview](/graph/api/resources/intune-deviceconfig-devicecompliancedeviceoverview?view=graph-rest-beta)<br/>[deviceConfigurationDeviceOverview](/graph/api/resources/intune-deviceconfig-deviceconfigurationdeviceoverview?view=graph-rest-beta)<br/>[deviceManagementExchangeOnpremisesPolicy](/graph/api/resources/intune-onboarding-devicemanagementexchangeonpremisespolicy?view=graph-rest-beta)<br/>[iosDeviceFeaturesConfiguration](/graph/api/resources/intune-deviceconfig-iosdevicefeaturesconfiguration?view=graph-rest-beta)<br/>[iosEducationDeviceConfiguration](/graph/api/resources/intune-deviceconfig-ioseducationdeviceconfiguration?view=graph-rest-beta)<br/>[iosLobAppProvisioningConfiguration](/graph/api/resources/intune-apps-ioslobappprovisioningconfiguration?view=graph-rest-beta)<br/>[onpremisesConditionalAccessSettings](/graph/api/resources/intune-onboarding-onpremisesconditionalaccesssettings?view=graph-rest-beta)<br/>[sharedPCConfiguration](/graph/api/resources/intune-deviceconfig-sharedpcconfiguration?view=graph-rest-beta)<br/>[windows10EnterpriseModernAppManagementConfiguration](/graph/api/resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration?view=graph-rest-beta)<br/>[windows10SecureAssessmentConfiguration](/graph/api/resources/intune-deviceconfig-windows10secureassessmentconfiguration?view=graph-rest-beta)<br/>[windows10WindowsInformationProtectionConfiguration](/graph/api/resources/intune-deviceconfig-windows10windowsinformationprotectionconfiguration?view=graph-rest-beta) |
|Adição|Beta|Foram adicionados novos tipos complexos: <br/> [appInstallationFailure](/graph/api/resources/intune-apps-appinstallationfailure?view=graph-rest-beta)<br/>[enterpriseCloudResource](/graph/api/resources/intune-deviceconfig-enterprisecloudresource?view=graph-rest-beta)<br/>[iosHomeScreenApp](/graph/api/resources/intune-deviceconfig-ioshomescreenapp?view=graph-rest-beta)<br/>[iosHomeScreenFolder](/graph/api/resources/intune-deviceconfig-ioshomescreenfolder?view=graph-rest-beta)<br/>[iosHomeScreenFolderPage](/graph/api/resources/intune-deviceconfig-ioshomescreenfolderpage?view=graph-rest-beta)<br/>[iosHomeScreenItem](/graph/api/resources/intune-deviceconfig-ioshomescreenitem?view=graph-rest-beta)<br/>[iosHomeScreenPage](/graph/api/resources/intune-deviceconfig-ioshomescreenpage?view=graph-rest-beta)<br/>[iosNotificationSettings](/graph/api/resources/intune-deviceconfig-iosnotificationsettings?view=graph-rest-beta)<br/>[iPv6Range](/graph/api/resources/intune-deviceconfig-ipv6range?view=graph-rest-beta)<br/>[sharedPCAccountManagerPolicy](/graph/api/resources/intune-deviceconfig-sharedpcaccountmanagerpolicy?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRule](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionapprule?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionappruleapplockerpolicyfiletemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleDesktopTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionappruledesktoptemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleStoreAppTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionapprulestoreapptemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionAppRuleTemplate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionappruletemplate?view=graph-rest-beta)<br/>[windowsInformationProtectionCorporateNetworkLocation](/graph/api/resources/intune-deviceconfig-windowsinformationprotectioncorporatenetworklocation?view=graph-rest-beta)<br/>[windowsInformationProtectionDataRecoveryCertificate](/graph/api/resources/intune-deviceconfig-windowsinformationprotectiondatarecoverycertificate?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocation](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocation?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseCloudResources](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterprisecloudresources?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseinternalproxyservers?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseipv4ranges?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseipv6ranges?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterprisenetworkdomainnames?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationEnterpriseProxyServers](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationenterpriseproxyservers?view=graph-rest-beta)<br/>[windowsInformationProtectionProtectedLocationNeutralResources](/graph/api/resources/intune-deviceconfig-windowsinformationprotectionprotectedlocationneutralresources?view=graph-rest-beta)
|Exclusão|Beta|Removido os seguintes tipos complexos e substituídos por microsoft.graph.Json:<br/>managedAppDeploymentSummary <br/>managedAppSummary<br /> |
|Alteração|Beta|Foi substituído o tipo de propriedade appConfigComplianceStatus por complianceStatus nas seguintes entidades: <br/>[managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta)<br/>[managedDeviceMobileAppConfigurationUserStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationuserstatus?view=graph-rest-beta)|
|Alteração|Beta|Para o recurso [managedAppStatusRaw](/graph/api/resources/intune-mam-managedappstatusraw?view=graph-rest-beta), foi alterado o tipo de conteúdo de propriedade de managedAppSummary para Json.|
|Alteração|Beta|Foi removida a função getUsersWithFlaggedAppRegistration da coleção [managedAppRegistration](/graph/api/resources/intune-mam-managedappregistration?view=graph-rest-beta).|
|Alteração|Beta|Foi alterada a propriedade de navegação **vppToken** da entidade [iosVppApp](/graph/api/resources/intune-apps-iosvppapp?view=graph-rest-beta) para que ela deixasse de ser uma coleção contida.|
|Alteração|Beta|A propriedade **deviceStatusOverview** foi adicionada às entidades [deviceConfiguration](/graph/api/resources/intune-deviceconfig-deviceconfiguration?view=graph-rest-beta) e [deviceCompliancePolicy](/graph/api/resources/intune-deviceconfig-devicecompliancepolicy?view=graph-rest-beta).|
|Alteração|Beta|A propriedade **appReportingOverview** foi adicionada ao singleton [deviceAppManagement](/graph/api/resources/intune-apps-deviceappmanagement?view=graph-rest-beta).|
|Alteração|Beta|Foram adicionadas as propriedades **deviceDisplayName** e **userPrincipalName** às entidades [deviceConfigurationDeviceStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationdevicestatus?view=graph-rest-beta), [deviceComplianceDeviceStatus](/graph/api/resources/intune-deviceconfig-devicecompliancedevicestatus?view=graph-rest-beta) e [managedDeviceMobileAppConfigurationDeviceStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationdevicestatus?view=graph-rest-beta).|
|Alteração|Beta|A propriedade **ruleName** foi adicionada à entidade [deviceComplianceScheduledActionForRule](/graph/api/resources/intune-deviceconfig-devicecompliancescheduledactionforrule?view=graph-rest-beta).|
|Alteração|Beta|Foram adicionadas as propriedades **devicesCount**, **userDisplayName** e **userPrincipalName** às entidades [deviceConfigurationUserStatus](/graph/api/resources/intune-deviceconfig-deviceconfigurationuserstatus?view=graph-rest-beta), [deviceComplianceUserStatus](/graph/api/resources/intune-deviceconfig-devicecomplianceuserstatus?view=graph-rest-beta) e [managedDeviceMobileAppConfigurationUserStatus](/graph/api/resources/intune-apps-manageddevicemobileappconfigurationuserstatus?view=graph-rest-beta).|
|Alteração|Beta|A coleção [notificationMessageTemplates](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-beta) foi adicionada ao singleton [deviceManagement](/graph/api/resources/intune-deviceconfig-devicemanagement?view=graph-rest-beta).|
|Alteração|Beta|Foram adicionadas as propriedades **isDefault**, **lastModifiedDateTime**, **locale**, **messageTemplate** e **subject** à entidade [localizedNotificationMessage](/graph/api/resources/intune-deviceconfig-localizednotificationmessage?view=graph-rest-beta).|
|Alteração|Beta|Foram adicionadas as propriedades **azureActiveDirectoryDeviceId**, **deviceCategory**, **deviceRegistrationState** e **managementAgent** à entidade [managedDevice](/graph/api/resources/intune-onboarding-manageddevice?view=graph-rest-beta).|
|Alteração|Beta|A propriedade **lastModifiedDateTime** foi adicionada à entidade [mobileAppCategory](/graph/api/resources/intune-apps-mobileappcategory?view=graph-rest-beta).|
|Alteração|Beta|Foram adicionadas as propriedades **brandingOptions**, **defaultLocale**, **displayName**, **fromEmailAddress**, **lastModifiedDateTime**, **localizedNotificationMessages** à entidade [notificationMessageTemplate](/graph/api/resources/intune-notification-notificationmessagetemplate?view=graph-rest-beta).|
|Alteração|Beta|Foram adicionadas as propriedades **appsAllowTrustedAppsSideloading**, **appsBlockWindowsStoreOriginatedApps**, **developerUnlockSetting**, **edgeBlockAccessToAboutFlags**, **edgeBlockDeveloperTools**, **edgeBlockExtensions**, **edgeBlockInPrivateBrowsing**, **edgeFirstRunUrl**, **edgeHomepageUrls**, **gameDvrBlocked**, **settingsBlockAddProvisioningPackage**, **settingsBlockChangeLanguage**, **settingsBlockChangePowerSleep**, ** settingsBlockChangeRegion**, **settingsBlockChangeSystemTime**, **settingsBlockEditDeviceName**, **settingsBlockRemoveProvisioningPackage**, **sharedUserAppDataAllowed**, **smartScreenBlockPromptOverride**, **smartScreenBlockPromptOverrideForFiles**, **storageRestrictAppDataToSystemVolume**, **storageRestrictAppInstallToSystemVolume**, **webRtcBlockLocalhostIpAddress**, **windowsStoreBlockAutoUpdate** e **windowsStoreEnablePrivateStoreOnly** à entidade [windows10GeneralConfiguration](/graph/api/resources/intune-deviceconfig-windows10generalconfiguration?view=graph-rest-beta).|

## <a name="december-2016"></a>Dezembro de 2016

### <a name="delta-query"></a>Consulta delta

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Adicionar uma nova função delta para as seguintes entidades realizem [consulta delta](delta-query-overview.md):<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>Confira os seguintes exemplos:<br/>[Obter as alterações incrementais para grupos (visualização)](delta-query-groups.md)<br/>[Obter as alterações incrementais para as mensagens em uma pasta (visualização)](delta-query-messages.md)<br/>[Obter as alterações incrementais para usuários (visualização)](delta-query-users.md) |

### <a name="excel-apis"></a>APIs do Excel

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Foi adicionado o recurso workbookPivotTable, as ações refresh e refreshAll a Tabelas Dinâmicas, o recurso workbookRangeView, a ação visibleView ao intervalo filtrado para retornar workbookRangeView para o usuário, extrair coleção de linhas e recurso de intervalo de visibleView, columnsAfter, columnsBefore, resizedRange, rowsAbove, e funções rowsBelow do recurso de intervalo, e novas propriedades de tabela. |

### <a name="intune-apis"></a>APIs do Intune

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Recursos adicionados e APIs de método para o Microsoft Intune. Este é um conjunto de recursos e métodos para dar suporte à visualização pública de Intune no Portal do Azure. Para saber mais sobre o serviço do Intune, veja a [documentação do Intune ](https://go.microsoft.com/fwlink/?linkid=836405). Para saber mais sobre os recursos do Intune e APIs, veja [Trabalho com o Intune no Microsoft Graph](/graph/api/resources/intune-graph-overview?view=graph-rest-beta). |

## <a name="october-2016"></a>Outubro de 2016

### <a name="authorization-provider"></a>Provedor de autorização

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0 e beta | O ponto de extremidade de autenticação v2.0 agora dá suporte à concessão do OAuth client_credentials, que pode ser usada para [daemon e processos com execução longa em cenários de negócios](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow). |
| Adição        | v1.0 e beta | O ponto de extremidade de autenticação v2.0 agora dá suporte a [escopos de permissão que exigem consentimento do administrador](permissions-reference.md), por meio do [ponto de extremidade de consentimento de administração](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#admin-restricted-permissions). |
| Adição        | v1.0 e beta | O ponto de extremidade de autenticação v2.0 agora dá suporte ao consentimento administrativo para todos os usuários de um locatário, por meio do [ponto de extremidade de consentimento de administração](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent#admin-restricted-permissions). |

### <a name="invitation-apis"></a>APIs de convite

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | A propriedade invitedUserType foi adicionada ao tipo de entidade de convite, que define o tipo de usuário (**Convidado** ou **Membro**) que é convidado. |
| Exclusão        | Beta        | Removeremos a propriedade invitedToGroups do tipo de entidade de convite em 11/11/2016. Isso significa que você não poderá mais adicionar um usuário convidado a um grupo usando essa API. Em vez disso, use a [API adicionar membro](/graph/api/group-post-members?view=graph-rest-1.0) para adicionar um usuário a um grupo. |

## <a name="september-2016"></a>Setembro de 2016

### <a name="azure-ad-application-proxy"></a>Proxy de aplicativo do Azure AD

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | O as APIs de Proxy de Aplicativo do Azure AD agora estão disponíveis nos pontos de extremidade beta do Microsoft Graph. Essas APIs permitem publicações seguras de aplicativos locais para usuários fora da rede corporativa que estejam usando o Azure AD como o plano de controle comum para acesso. Você pode usar as APIs publicadas para gravar os aplicativos que podem recuperar e atualizar diversos aspectos do proxy de aplicativo, como as configurações _conectores_, _connectorGroups_ e _onPremisesPublishing_ de um aplicativo. |

### <a name="drive"></a>Unidade

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | A coleção _shared_ foi adicionada para permitir o acesso aos driveItems compartilhados pela URL shareId ou sharing. |
| Adição        | Beta        | A função _search_ foi adicionada a uma unidade, o que permite pesquisar mais itens do que apenas aqueles que constam na pasta raiz da unidade. |


### <a name="driveitem"></a>DriveItem

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Suporte adicional para _createUploadSession_, o que permite carregar arquivos com mais de 4 MB no OneDrive, no OneDrive for Business e em bibliotecas de documentos do SharePoint. |
| Adição        | Beta        | A propriedade _sharepointIds_ foi adicionada ao driveItem que retorna identificadores de API do SharePoint tradicionais para driveItems armazenados no SharePoint. |
| Adição        | Beta        | Outras propriedades foram adicionadas ao _remoteItem_. |
| Adição        | Beta        | Foi adicionado o valor _quickXorHash_ aos arquivos no OneDrive for Business. |
| Adição        | Beta        | O escopo para _createSharingLink_ foi adicionado para permitir a criação de links compartilháveis da empresa ou links de compartilhamento anônimos. |

### <a name="extended-properties"></a>Propriedades estendidas

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | As [propriedades estendidas](/graph/api/resources/extended-properties-overview?view=graph-rest-1.0) agora são compatíveis com os seguintes recursos:message, mailFolder, event, calendar, contact, contactFolder, group event, group calendar, group post. |

### <a name="groups"></a>Grupos

Suporte adicionado para a associação de grupo dinâmico através de visualização pública API, incluindo as adições listados na tabela a seguir.

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | A propriedade **membershipRule** adicionada que contém regras de controle das associações a esse grupo, se o grupo for um grupo dinâmico |
| Adição        | Beta        | A propriedade **membershipRuleProcessingState** foi adicionada para controlar se o processamento de associação dinâmica está ativado ou pausado para esse grupo. |
| Adição        | Beta        | Defina a propriedade **groupTypes** para conter **"DynamicMembership"** a fim de ativar o recurso de grupos dinâmicos para esse grupo. |
| Adição        | Beta        | A propriedade **preferredLanguage** foi adicionada para indicar o idioma de preferência para um grupo do Office 365. |
| Adição        | Beta        | A propriedade **theme** foi adicionada para especificar o tema da cor de um grupo do Office 365. |

### <a name="hybrid-deployment-support"></a>Suporte à implantação híbrida

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Os aplicativos podem usar a versão 1.0 das APIs de Email, Calendário e Contatos do Outlook para acessar caixas de correio locais em uma implantação híbrida com a Atualização Cumulativa 3 (CU3) do Exchange 2016. Veja mais detalhes sobre o suporte à API REST em [implantações híbridas](hybrid-rest-support.md) específicas. **Observação:** se você estiver usando os conjuntos da API na versão 1.0, agora é possível que seus aplicativos, incluindo aplicativos de produção, funcionem com caixas de correio locais que atendam a requisitos de implantação híbrida específicos. Esse recurso só está disponível na visualização. |

### <a name="identityriskevents"></a>IdentityRiskEvents

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | Como parte da alteração de esquema em que o tipo de duas propriedades de local está sendo substituído por um novo tipo complexo no ponto de extremidade identityRiskEvents, as seguintes propriedades são alteradas/adicionadas no ponto de extremidade identityRiskEvents:</br>**location**  alterado de Edm.String para ComplexType signInLocation.<br/>**previousLocation** alterado de Edm.String para ComplexType signInLocation.<br/>**signInLocation** novo ComplexType que contém as propriedades city, state, countryOrRegion e geoCoordinates.<br/>**geoCoordinates** novo ComplexType que contém as propriedades latitude e longitude. |

### <a name="invitation-manager"></a>Gerenciador de convites

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | As APIs do gerenciador de convites agora estão disponíveis nos pontos de extremidade do Microsoft Graph na versão Beta. Você pode usar as APIs do gerenciador de convites para que o gerenciador de convites crie um convite para adicionar um usuário externo à organização. Como parte do convite, você também pode optar por adicionar o usuário convidado a um grupo do Office 365. Para obter mais detalhes, veja [gerenciador de convite](/graph/api/resources/invitation?view=graph-rest-beta). |

### <a name="onedrive"></a>OneDrive

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Foi adicionado o método **CreateUploadSession** ao **driveItem**, que permite arquivos grandes e carregamentos retomáveis. |
| Adição        | v1.0        | Foram adicionadas as propriedades para rastrear as IDs do SharePoint em itens do SharePoint (**sharepointIds**) e uma propriedade para identificar pastas-raiz (**root**). |
| Adição        | v1.0        | Foi adicionado o conjunto-raiz **Shares**, que pode ser usado com shareIds ou links de compartilhamento para acessar itens compartilhados no OneDrive e no SharePoint. Retorna um novo tipo, sharedDriveItem. |
| Adição        | v1.0        | Foi adicionado o método**Invite** ao driveItem, que permite adicionar permissões a itens. |
| Adição        | v1.0        | Foi adicionado o método **Search** à unidade, que permite pesquisar itens na unidade e itens compartilhados. |
| Adição        | v1.0        | A propriedade **processingMetadata** foi adicionada à propriedade quickXorHash do tipo complexo no tipo complexo hashes. |
| Adição        | v1.0        | A propriedade **quickXorHash** foi adicionada ao tipo complexo hashes. |

### <a name="outlook-calendar"></a>Calendário do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | A propriedade **onlineMeetingUrl** foi adicionada ao recurso [event](/graph/api/resources/event?view=graph-rest-1.0). |
| Adição        | Beta        | A ação [forward](/graph/api/event-forward?view=graph-rest-beta) foi adicionada ao recurso event. |
| Adição        | Beta        | Foram adicionadas as propriedades ao recurso [calendar](/graph/api/resources/calendar?view=graph-rest-beta) para dar suporte ao compartilhamento de calendários: **canEdit**, **canShare**, **canViewPrivateItems**, **isShared**, **isShareWithMe** e **owner**. |

### <a name="outlook-mail"></a>Email do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Foi adicionado o tipo complexo [mailboxSettings](/graph/api/resources/mailboxsettings?view=graph-rest-1.0), que inclui as propriedades **automaticRepliesSetting**, **timeZone** e **language**. |
| Adição        | v1.0        | A propriedade **mailboxSettings** foi adicionada ao recurso [user](/graph/api/resources/user?view=graph-rest-1.0). |
| Adição        | Beta        | Foi adicionado o suporte para criar, listar, obter e excluir uma ou mais instâncias de [mencionar](/graph/api/resources/mention?view=graph-rest-beta) em uma mensagem. As menções dão suporte a chamadas para chamar a atenção dos outros usuários em uma mensagem. |
| Adição        | Beta        | Foi adicionado suporte para a ação [getMailTips](/graph/api/user-getmailtips?view=graph-rest-beta) para obter Dicas de Email para destinatários específicos. Foram adicionados os seguintes recursos: [automaticRepliesMailTips](/graph/api/resources/automaticrepliesmailtips?view=graph-rest-beta), [mailTips](/graph/api/resources/mailtips?view=graph-rest-beta), [mailTipsError](/graph/api/resources/mailtipserror?view=graph-rest-beta). |

### <a name="query-parameters"></a>Parâmetros de consulta

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | Os prefixos de parâmetros de consulta sem $ são suportados a partir de 26/09/16. O prefixo $ nos parâmetros de consulta é opcional. Para obter mais detalhes, confira [Suporte a parâmetros da consulta sem prefixos $ no post do blog do Microsoft Graph](https://dev.office.com/queryparametersinMicrosoftGraph). |

### <a name="sharepoint"></a>SharePoint

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Acesso a sites do SharePoint e [listas por ID](/graph/api/list-get?view=graph-rest-beta) ou [caminho/URL](/graph/api/baseitem-getbyurl?view=graph-rest-beta) |
| Adição        | Beta        | Suporte para [listar, criar, obter e excluir instâncias de listItem](/graph/api/resources/listitem?view=graph-rest-beta). |

### <a name="users"></a>Usuários

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | A propriedade somente leitura **refreshTokensValidFromDateTime** foi adicionada para indicar quando os tokens de sessão e de atualização são válidos. Qualquer token emitido antes desse momento será inválido, e qualquer tentativa de usá-lo forçará uma nova entrada do usuário. |
| Adição        | Beta        | A propriedade **showInAddressList** foi adicionada para você controlar se a lista de endereços global do Outlook deve conter este usuário. |
| Adição        | Beta        | Foi adicionada a ação de serviço **invalidateAllRefreshTokens** que invalida todos os tokens de sessão e de atualização do usuário emitidos para aplicativos, redefinindo a propriedade do usuário **refreshTokensValidFromDateTime** para a data e a hora atuais. |


### <a name="webhooks"></a>Webhooks

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Os itens de raiz de unidade adicionados aos Webhooks como um recurso que está disponível para se inscrever. |

## <a name="august-2016"></a>Agosto de 2016

### <a name="contacts"></a>Contatos

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Como parte da mudança do esquema onde algumas propriedades estão sendo removidas e conjuntos de correspondentes estão sendo adicionados ao ponto de extremidade de contatos, as seguintes propriedades foram adicionadas ao ponto de extremidade de contatos: _Websites Collection(ComplexType: Website)_,_Phones Collection (ComplexType: Phone)_, _PostalAddress Collection(ComplexType: PhysicalAddress)_. Para obter detalhes, veja a postagem de blog [Upcoming changes to Contacts and People APIs](https://developer.microsoft.com/office/blogs/upcoming-changes-to-contacts-and-people-apis/) (Futuras alterações nas APIs de Contatos e Pessoas). |
| Exclusão        | Beta        | Como parte da mudança do esquema onde algumas propriedades estão sendo removidas e conjuntos de correspondentes estão sendo adicionados ao ponto de extremidade de contatos, as seguintes propriedades foram removidas do ponto de extremidade de contatos: _BusinessHomePage_,_HomePhones_, _MobilePhone1_, _BusinessPhones_, _HomeAddress_, _BusinessAddress_, _OtherAddress_. Para obter detalhes, veja a postagem de blog [Upcoming changes to Contacts and People APIs](https://developer.microsoft.com/office/blogs/upcoming-changes-to-contacts-and-people-apis/) (Futuras alterações nas APIs de Contatos e Pessoas). |

### <a name="excel-apis"></a>APIs do Excel

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Em geral, a API REST do Excel no Microsoft Graph está disponível. Agora, você pode criar integrações avançadas e profundas com pastas de trabalho do Excel no Office 365. Confira o [Turbine seus aplicativos com a nova API REST do Excel no Microsoft Graph](https://developer.microsoft.com/office/blogs/power-your-apps-with-the-new-excel-rest-api/) na postagem do blog para obter mais detalhes. |

### <a name="people"></a>Pessoas

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | A propriedade _WebSite_ será renomeada como _WebSite_. Para obter detalhes, veja [Futuras Alterações nas APIs de Contatos e Pessoas](https://developer.microsoft.com/office/blogs/upcoming-changes-to-contacts-and-people-apis/). |

### <a name="privileged-identity-management"></a>Privileged Identity Management

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | As APIs REST de Privileged Identity Management (PIM) agora estão disponíveis no ponto de extremidade beta do Microsoft Graph. O [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure) fornece ativação "just in time" para funções organizacionais privilegiadas do Azure AD, como Administrador Global, Administrador de Cobrança, etc. As APIs publicadas permitem que os desenvolvedores criem aplicativos que recuperem e atualizem as atribuições de funções privilegiadas e ativem usuários em funções. Para obter detalhes, veja [Microsoft Graph: APIs de Pré-Visualização do Azure AD Privileged Identity Management disponíveis na versão Beta](https://developer.microsoft.com/office/blogs/microsoft-graph-azure-ad-privileged-identity-management-apis-beta/) e o [Azure AD Privileged Identity Management](/graph/api/resources/privilegedidentitymanagement-root?view=graph-rest-beta). |

## <a name="july-2016"></a>Julho de 2016

### <a name="administrative-units"></a>Unidades administrativas

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Introduziu a nova API de pré-visualização das Unidades Administrativas. As unidades administrativas permitem às organizações subdividir seu Azure Active Directory e delegar tarefas administrativas a essas subdivisões. As subdivisões podem representar regiões, departamentos, centros de custo etc. Agora, isso pode ser gerenciado por meio da API do Microsoft Graph. |

## <a name="june-2016"></a>Junho de 2016

### <a name="identityriskevents"></a>IdentityRiskEvents

|**Tipo de alteração**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Adição|Beta|Introduziu a nova API de visualização de IdentityRiskEvents. Essa API funciona em conjunto com o Azure Active Directory Identity Protection. É possível utilizá-la para consultar eventos de risco gerados pelo Identity Protection. Para obter mais detalhes, veja a [Introdução de uma nova API de visualização do Microsoft Graph: Postagem do blog ](https://developer.microsoft.com/office/blogs/identityriskevents-api-preview/)IdentityRiskEvents

### <a name="subscriptions"></a>Assinaturas

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Os escopos somente aplicativo agora têm suporte para assinaturas de _email_ e _contatos_. |

## <a name="may-2016"></a>Maio de 2016

### <a name="calendar"></a>Calendário

|**Tipo de alteração**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Alteração significativa|Beta|Alterações na API findMeetingTimes. Para saber mais, veja a postagem de blog [Microsoft Graph findMeetingTimes API update](https://dev.office.com/microsoft-graph-findmeetingtimes-api-update) (Atualização da API findMeetingTimes do Microsoft Graph). Essa alteração entrou em vigor em 19 de maio de 2016.

### <a name="contact"></a>Contato

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Foram adicionadas _extensions_, que correspondem a um tipo abstrato que dá suporte à extensão openTypeExtension de tipo aberto do OData v4. |

### <a name="directory"></a>Diretório

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração significativa | Beta        | _settingTemplateId_ foi renomeado como _templateId_. Essa alteração entrou em vigor a partir de 19 de maio de 2016. |

### <a name="event"></a>Evento

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Foram adicionadas _extensions_, que correspondem a um tipo abstrato que dá suporte à extensão openTypeExtension de tipo aberto do OData v4. |

### <a name="eventmessages"></a>EventMessages

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | _inferenceClassification_ e _extensions_ foram adicionados a _eventMessages_. |
| Adição        | Beta        | _responseRequested_ foi adicionado a _eventMessageRequest_. |

### <a name="messages"></a>Mensagens

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | _inferenceClassification_ e _extensions_ foram adicionados a _messages_. |
| Adição        | Beta        | _wellknownname_ foi adicionado a _contactFolder_. |

### <a name="post"></a>Postagem

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Foram adicionadas _extensions_, que correspondem a um tipo abstrato que dá suporte à extensão openTypeExtension de tipo aberto do OData v4. |

### <a name="user"></a>Usuário

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | O tipo de recurso _inferenceClassification_ foi adicionado. |
| Adição        | Beta        | _timeZone_ foi adicionado a _mailboxsettings_.   |
| Adição        | Beta        | A API _findMeetingTimes_ foi adicionada a _user_.   |

## <a name="april-2016"></a>Abril de 2016

### <a name="general"></a>Geral

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0 e Beta | Obter suporte adicional para honrar a _Codificação de aceitação: gzip_. |
| Adição        | v1.0          | Foi adicionado suporte para o segmento de conversão no caminho de expansão. Por exemplo, 'https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event'. |
| Adição        | Beta          | Suporte adicional para solicitação de PATCH em relação a propriedades estruturais. Por exemplo: 'PATCH /me/mailboxSettings'. |
| Adição        | Beta          | O Azure Active Directory agora é usado como fallback para solicitações /beta/users/id/photo quando o Outlook não consegue atender à solicitação para casos como quando o usuário não tem nenhuma licença de caixa de correio ou o locatário não tem uma assinatura do Exchange Online. OBSERVAÇÃO: esse fallback está disponível para GET e PATCH. |
| Adição        | Beta          | Foi adicionado suporte para o segmento de conversão no caminho de expansão. Por exemplo, https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event’. |

### <a name="onedrive"></a>OneDrive

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Correção             | v1.0        | Corrigido o problema de solicitações createLink do OneDrive com falhas 500 e "Tipo de propriedade de extensão sem suporte". |

## <a name="march-2016"></a>Março de 2016

### <a name="calendar"></a>Calendário

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | As propriedades _singleValueExtendedProperties_ e _multiValueExtendedProperties_ foram adicionadas. |
| Adição        | Beta        | A propriedade _suggestionHint_ foi adicionada a _meetingTimeCandidate_. |
| Adição        | Beta        | A propriedade _locationUri_ foi adicionada a _location_. |
| Adição        | Beta        | _type_ e _postOfficeBox_ foram adicionadas a _physicalAddress_. |
| Alteração          | Beta        | _findMeetingTimes_ agora tem um novo parâmetro _ReturnSuggestionHint_. |
| Alteração          | Beta        | _findMeetingTimes_ agora retorna uma coleção de _meetingTimeCandidate_. |

### <a name="drive"></a>Unidade

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0 e beta | Foi adicionada a função _recent_ para listar um conjunto de itens usados recentemente pelo usuário conectado. Esta lista inclui itens que estão na unidade do usuário, assim como itens aos quais ele tem acesso por meio de outras unidades. Exemplo: GET /me/drive/recent. |
| Adição        | v1.0 e beta | Foi adicionada a função _sharedWithMe_ para listar um conjunto de itens que são compartilhados com o usuário atual. Exemplo: GET /me/drive/sharedWithMe |

### <a name="driveitem"></a>DriveItem

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0 e beta | Foi adicionado o tipo _remoteItem_ para fornecer um link a um item em outra unidade. |
| Adição        | v1.0 e beta | Foi adicionado o tipo _sharingInvitation_ para fornecer detalhes de qualquer convite de compartilhamento associado para essa permissão. |
| Adição        | v1.0 e beta | Foi adicionada a função _delta_ para rastrear as alterações aos itens de uma unidade. Exemplo: GET /e/drive/items/{id-do-item}/delta |
| Adição        | v1.0 e beta | Foi adicionada _copy_ para criar uma cópia de um _driveItem_ (incluindo todos os filhos) em um novo pai ou mãe com um novo nome. Exemplo: POST /me/drive/items/{item-id}/copy. |
| Adição        | v1.0 e beta | Os atributos da instância _conflictBehavior_ agora se aplicam ao _driveItem_. |
|Adição|Beta|Foi adicionada a função _invite_ para enviar um convite de compartilhamento a um item existente. Um convite de compartilhamento cria um link de compartilhamento exclusivo e envia um email ao destinatário do convite que inclui o link de compartilhamento. Exemplo: POST /drive/items/{id-do-item}/invite

### <a name="event"></a>Evento

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foram adicionados a nova propriedade _onlineMeetingUrl_ e o novo método _cancel_. |

### <a name="event-messages"></a>Mensagens de evento

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foram adicionadas as propriedades _startDateTime_, _endDateTime_, _location_, _type_, _recurrence_, _isOutOfDate_, _conversationIndex_, _unsubscribe_, _unsubscribeData_, _unsubscribeEnabled_ e _flag_ ao objeto _eventmessage_. |
| Adição        | Beta        | As propriedades _singleValueExtendedProperties_ e _multiValueExtendedProperties_ foram adicionadas. |
| Adição        | Beta        | O novo método _unsubscribe_ foi adicionado.          |

### <a name="excel"></a>Excel

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Estamos adicionando novas APIs REST do Excel que permitem a leitura e a modificação de dados em uma pasta de trabalho do Excel. Agora é possível criar aplicativos inteligentes que permitem que os usuários obtenham valor do conteúdo armazenado em uma pasta de trabalho do Excel, fornecendo informações aos dados. Aproveite o potencial analítico do Excel, crie tabelas e gráficos e extraia imagens do gráfico visualmente atraentes – tudo isso a partir do seu aplicativo. Para obter mais detalhes, veja [Trabalhando com o Excel no Microsoft Graph](/graph/api/resources/excel?view=graph-rest-beta). |

### <a name="general"></a>Geral

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0 e beta | Melhorar mensagens de erro ao resolver tokens JWT (AAD) rejeitados e alias do locatário. |
| Adição        | v1.0 e beta | A localização do ponto de extremidade do serviço de autorização agora é retornada no cabeçalho _www-authenticate_ quando uma solicitação é recebida com um token de portador vazio. |
| Adição        | v1.0 e beta | A capacidade de filtrar na propriedade de ID da entidade já está corrigida. Exemplo: GET https://graph.microsoft.com/v1.0/users?$filter=id+eq+'x'<br/>Antes, qualquer solicitação POST para ações de serviço e funções exigia a prefixação do nome da função ou ação com o prefixo microsoft.graph. Por exemplo: POST https://graph.microsoft.com/v1.0/me/Microsoft.Graph.getMemberGroups<br/>Agora, o prefixo não é mais necessário (embora ele ainda possa ser especificado). Portanto, o seguinte também funcionará agora: POST https://graph.microsoft.com/v1.0/me/getMemberGroups |
| Alteração          | Beta          | Foram limpos os nomes de propriedades de assinatura.  |
| Adição        | Beta          | Adicionamos a capacidade de descobrir (por meio de _directorySettingTemplates_) e substituir o comportamento padrão (criando uma _configuração_ do modelo) para entidades e suas funcionalidades associadas. Inicialmente, esse único modelo fornecido serve para controlar comportamentos de grupos do Office. |

### <a name="mail-folder"></a>Pasta de email

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | As propriedades _wellKnownName_ e _userConfigurations_ foram adicionadas. |
| Adição        | Beta        |  As propriedades _singleValueExtendedProperties_ e _multiValueExtendedProperties_ foram adicionadas |

### <a name="messages"></a>Mensagens

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0          | A propriedade _mobilePhone_ foi adicionada.            |
| Adição        | v1.0 e beta | A propriedade _internetMessageId_ foi adicionada. A ID da mensagem no formato especificado por [RFC2822](https://www.ietf.org/rfc/rfc2822.txt). |
| Alteração          | Beta          | A propriedade _mobilePhone1_ foi renomeada para _mobilePhone_. |
| Alteração          | Beta          | _createReply_ e _createReplyAll_ adotaram um novo parâmetro _Message_ e _comment_. |
| Alteração          | Beta          | _createForward_ adotou um novo parâmetro _Message_, _ToRecipients_ e _comment_. |
| Alteração          | Beta          | _reply_, _replyAll_ e _forward_ adotaram um novo parâmetro _Message_. |

### <a name="permission"></a>Permissão

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0 e beta | Foi adicionada a propriedade _sharingInvitation_ para fornecer detalhes sobre qualquer convite de compartilhamento associado para essa permissão. |

### <a name="person"></a>Pessoa

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foram adicionadas as novas propriedades _birthday_, _personNotes_, _isFavorite_, _phones_, _permission_, _postalAddresses_,_websites_,_yomiCompany_, _department_, _profession_, _mailboxType_ e _personType_. |
| Adição        | Beta        | Foram adicionados os novos tipos de enumeração _physicalAddressType_, _webSite_, _phone_ e _webSiteType_. |

### <a name="reference-attachment"></a>Anexo de referência

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foram adicionadas as novas propriedades _sourceUrl_, _providerType_, _thumbnailUrl_, _previewUrl_, _permission_ e _isFolder_. |
| Adição        | Beta        | As propriedades _singleValueExtendedProperties_ e _multiValueExtendedProperties_ foram adicionadas. |
| Adição        | Beta        | Foram adicionados os novos tipos enumeração _referenceAttachmentProvider_ e _referenceAttachmentPermission_. |

### <a name="subscriptions"></a>Assinaturas

| **Tipo de alteração** | **Ponto de extremidade** | **Descrição**                          |
| :-------------- | :----------- | :--------------------------------------- |
| Adição        | v1.0         | Os webhooks agora são GA no ponto de extremidade da versão 1.0 por meio do recurso _/Subscriptions_. Crie, Leia, Renove e Exclua assinaturas para receber notificações sobre dados do Outlook e de conversas de grupo do Office 365. |

### <a name="user"></a>Usuário

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foi adicionada a propriedade _mailboxSettings_ e os tipos correspondentes. |

## <a name="february-2016"></a>fevereiro de 2016

### <a name="driveitem"></a>DriveItem

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0 e beta | Nova propriedade _remoteItem_ em driveItem para contas da Microsoft. |

### <a name="general"></a>Geral

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Alteração          | v1.0 e beta | -_/me/drive_ agora funciona tanto para contas da Microsoft como para contas corporativas e de estudante. |
| Alteração          | v1.0 e beta | As solicitações de unidade para contas cujo armazenamento do OneDrive foi provisionado sob trabalho de demanda funcionam de forma mais confiável e em mais cenários onde os sites padrão do SharePoint do locatário usam nomes não padrão. |
| Exclusão        | Beta          | Diversos tipos não implementados do esquema beta foram removidos para obter uma melhor correspondência com o esquema 1.0. |

### <a name="subscriptions"></a>Assinaturas

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | validação de notificationUrl na criação da assinatura. Para obter detalhes, veja [Microsoft Graph WebHooks Update – janeiro de 2016](https://developer.microsoft.com/office/blogs/Microsoft-Graph-WebHooks-Update-January-2016/). |
| Adição        | Beta        | Agora, as entidades de assinatura podem ser excluídas: DELETE https://graph.microsoft.com/beta/subscriptions/ |

### <a name="users"></a>Usuários

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Alteração          | v1.0 e beta | _displayName_ agora é retornado para contas da Microsoft. |

## <a name="january-2016"></a>janeiro de 2016

### <a name="contacts"></a>Contatos

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Foi adicionada a propriedade mobilePhone ao conjunto de entidades personal contact. |

### <a name="directoryobjects"></a>directoryObjects

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Correção             | v1.0 e beta | As ações de chamada vinculadas a directoryObjects foram corrigidas, pois apresentavam os seguintes erros:  O tipo de retorno da operação não é compatível com o conjunto de entidades fornecido. Isso se aplica às seguintes ações: _microsoft.graph.checkMemberObjects_, _microsoft.graph.getMemberObjects_, _microsoft.graph.checkMemberGroups_, _microsoft.graph.assignLicense_, _microsoft.graph.changePassword_. |

## <a name="december-2015"></a>dezembro de 2015

### <a name="contacts"></a>Contatos

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foi adicionada a propriedade mobilePhone ao conjunto de entidades personal contact. |

### <a name="general"></a>Geral

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Correção             | v1.0 e beta | Foram corrigidas solicitações usando as expressões $filter que especificavam a mesma propriedade mais de uma vez, que estavam falhando com o seguinte erro 500: um item com a mesma chave já foi adicionado. |
| Correção             | v1.0 e beta | Foi corrigida a falta de sensibilidade a maiúsculas e minúsculas para valores e nomes de parâmetros de ação. |
| Correção             | v1.0 e beta | Foi corrigido o processamento de solicitações para cargas que contêm valores nulos para algumas propriedades complexas inseridos, que estavam falhando com uma exceção de referência nula. |
| Adição        | v1.0 e beta | Suporte adicional para a classificação e filtragem de propriedades de tipo complexas. |
| Adição        | v1.0 e beta | A propriedade authorization_uri foi adicionada ao cabeçalho www-authenticate em uma resposta 401. Esse uri pode ser usado para iniciar o fluxo de aquisição do token. |
| Adição        | v1.0 e beta | Mensagens de erro aprimoradas em usuários e grupos. |

### <a name="groups"></a>Grupos

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Correção             | v1.0 e beta | Corrigiu-se a chamada às seguintes ações de grupo: _microsoft.graph.addFavorite_, _microsoft.graph.removeFavorite_ e _microsoft.graph.resetUnseenCount_. |

### <a name="messages"></a>Mensagens

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foi adicionado o subtipo eventMessageRequest das propriedades eventMessage e startDateTime, endDateTime, location, type, recurrence e isOutOfDate ao tipo eventMessage. |

### <a name="users"></a>Usuários

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Correção             | v1.0 e beta | Corrigiu a possibilidade de selecionar determinadas propriedades de usuário em outros usuários ao referenciar o usuário pelo nome UPN. Por exemplo: https://graph.microsoft.com/v1.0/users/anotherUser@contoso.com?$select=aboutMe |
| Correção             | v1.0 e beta | Foi corrigida a chamada à função de limite do usuário _microsoft.graph.reminderView_, pois estava falhando com o seguinte erro: Não foi possível localizar uma propriedade chamada businessPhones no tipo 'Microsoft.OutlookServices.Reminder. |
| Correção             | v1.0 e beta | Foram corrigidas a criação e a atualização de usuário (POST/PATCH /v1.0/users), que estava falhando com um erro 400. |
