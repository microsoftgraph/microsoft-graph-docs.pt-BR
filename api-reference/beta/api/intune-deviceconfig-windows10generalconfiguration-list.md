---
title: Listar windows10GeneralConfigurations
description: Listar propriedades e relações dos objetos windows10GeneralConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c1c4892ef30004e682993209109b83ba37e08cbc
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127785"
---
# <a name="list-windows10generalconfigurations"></a><span data-ttu-id="a664e-103">Listar windows10GeneralConfigurations</span><span class="sxs-lookup"><span data-stu-id="a664e-103">List windows10GeneralConfigurations</span></span>

<span data-ttu-id="a664e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a664e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a664e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a664e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a664e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a664e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a664e-107">Listar propriedades e relações dos objetos [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a664e-107">List properties and relationships of the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a664e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a664e-108">Prerequisites</span></span>
<span data-ttu-id="a664e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a664e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a664e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a664e-111">Permission type</span></span>|<span data-ttu-id="a664e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a664e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a664e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a664e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a664e-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a664e-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a664e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a664e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a664e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a664e-116">Not supported.</span></span>|
|<span data-ttu-id="a664e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a664e-117">Application</span></span>|<span data-ttu-id="a664e-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a664e-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a664e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a664e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a664e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a664e-120">Request headers</span></span>
|<span data-ttu-id="a664e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a664e-121">Header</span></span>|<span data-ttu-id="a664e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a664e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a664e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a664e-123">Authorization</span></span>|<span data-ttu-id="a664e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a664e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a664e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a664e-125">Accept</span></span>|<span data-ttu-id="a664e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a664e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a664e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a664e-127">Request body</span></span>
<span data-ttu-id="a664e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a664e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a664e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a664e-129">Response</span></span>
<span data-ttu-id="a664e-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a664e-130">If successful, this method returns a `200 OK` response code and a collection of [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a664e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a664e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a664e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a664e-132">Request</span></span>
<span data-ttu-id="a664e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a664e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="a664e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a664e-134">Response</span></span>
<span data-ttu-id="a664e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a664e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 16638

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
      "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
        "osEditionTypes": [
          "windows10EnterpriseN"
        ],
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
        "minOSVersion": "Min OSVersion value",
        "maxOSVersion": "Max OSVersion value",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
        "deviceMode": "sModeConfiguration",
        "name": "Name value",
        "ruleType": "exclude"
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "taskManagerBlockEndTask": true,
      "energySaverOnBatteryThresholdPercentage": 7,
      "energySaverPluggedInThresholdPercentage": 7,
      "powerLidCloseActionOnBattery": "noAction",
      "powerLidCloseActionPluggedIn": "noAction",
      "powerButtonActionOnBattery": "noAction",
      "powerButtonActionPluggedIn": "noAction",
      "powerSleepButtonActionOnBattery": "noAction",
      "powerSleepButtonActionPluggedIn": "noAction",
      "powerHybridSleepOnBattery": "enabled",
      "powerHybridSleepPluggedIn": "enabled",
      "windows10AppsForceUpdateSchedule": {
        "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
        "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
        "recurrence": "daily",
        "runImmediatelyIfAfterStartDateTime": true
      },
      "enableAutomaticRedeployment": true,
      "microsoftAccountSignInAssistantSettings": "disabled",
      "authenticationAllowSecondaryDevice": true,
      "authenticationWebSignIn": "enabled",
      "authenticationPreferredAzureADTenantDomainName": "Authentication Preferred Azure ADTenant Domain Name value",
      "cryptographyAllowFipsAlgorithmPolicy": true,
      "displayAppListWithGdiDPIScalingTurnedOn": [
        "Display App List With Gdi DPIScaling Turned On value"
      ],
      "displayAppListWithGdiDPIScalingTurnedOff": [
        "Display App List With Gdi DPIScaling Turned Off value"
      ],
      "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
      "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
      "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
      "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
      "enterpriseCloudPrintDiscoveryMaxLimit": 5,
      "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
      "experienceDoNotSyncBrowserSettings": "blockedWithUserOverride",
      "messagingBlockSync": true,
      "messagingBlockMMS": true,
      "messagingBlockRichCommunicationServices": true,
      "printerNames": [
        "Printer Names value"
      ],
      "printerDefaultName": "Printer Default Name value",
      "printerBlockAddition": true,
      "searchBlockDiacritics": true,
      "searchDisableAutoLanguageDetection": true,
      "searchDisableIndexingEncryptedItems": true,
      "searchEnableRemoteQueries": true,
      "searchDisableUseLocation": true,
      "searchDisableLocation": true,
      "searchDisableIndexerBackoff": true,
      "searchDisableIndexingRemovableDrive": true,
      "searchEnableAutomaticIndexSizeManangement": true,
      "searchBlockWebResults": true,
      "findMyFiles": "enabled",
      "securityBlockAzureADJoinedDevicesAutoEncryption": true,
      "diagnosticsDataSubmissionMode": "none",
      "oneDriveDisableFileSync": true,
      "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
      "edgeTelemetryForMicrosoft365Analytics": "intranet",
      "inkWorkspaceAccess": "enabled",
      "inkWorkspaceAccessState": "blocked",
      "inkWorkspaceBlockSuggestedApps": true,
      "smartScreenEnableAppInstallControl": true,
      "smartScreenAppInstallControl": "anywhere",
      "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
      "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
      "bluetoothAllowedServices": [
        "Bluetooth Allowed Services value"
      ],
      "bluetoothBlockAdvertising": true,
      "bluetoothBlockPromptedProximalConnections": true,
      "bluetoothBlockDiscoverableMode": true,
      "bluetoothBlockPrePairing": true,
      "edgeBlockAutofill": true,
      "edgeBlocked": true,
      "edgeCookiePolicy": "allow",
      "edgeBlockDeveloperTools": true,
      "edgeBlockSendingDoNotTrackHeader": true,
      "edgeBlockExtensions": true,
      "edgeBlockInPrivateBrowsing": true,
      "edgeBlockJavaScript": true,
      "edgeBlockPasswordManager": true,
      "edgeBlockAddressBarDropdown": true,
      "edgeBlockCompatibilityList": true,
      "edgeClearBrowsingDataOnExit": true,
      "edgeAllowStartPagesModification": true,
      "edgeDisableFirstRunPage": true,
      "edgeBlockLiveTileDataCollection": true,
      "edgeSyncFavoritesWithInternetExplorer": true,
      "edgeFavoritesListLocation": "Edge Favorites List Location value",
      "edgeBlockEditFavorites": true,
      "edgeNewTabPageURL": "Edge New Tab Page URL value",
      "edgeHomeButtonConfiguration": {
        "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
      },
      "edgeHomeButtonConfigurationEnabled": true,
      "edgeOpensWith": "startPage",
      "edgeBlockSideloadingExtensions": true,
      "edgeRequiredExtensionPackageFamilyNames": [
        "Edge Required Extension Package Family Names value"
      ],
      "edgeBlockPrinting": true,
      "edgeFavoritesBarVisibility": "hide",
      "edgeBlockSavingHistory": true,
      "edgeBlockFullScreenMode": true,
      "edgeBlockWebContentOnNewTabPage": true,
      "edgeBlockTabPreloading": true,
      "edgeBlockPrelaunch": true,
      "edgeShowMessageWhenOpeningInternetExplorerSites": "disabled",
      "edgePreventCertificateErrorOverride": true,
      "edgeKioskModeRestriction": "digitalSignage",
      "edgeKioskResetAfterIdleTimeInMinutes": 4,
      "cellularBlockDataWhenRoaming": true,
      "cellularBlockVpn": true,
      "cellularBlockVpnWhenRoaming": true,
      "cellularData": "required",
      "defenderRequireRealTimeMonitoring": true,
      "defenderRequireBehaviorMonitoring": true,
      "defenderRequireNetworkInspectionSystem": true,
      "defenderScanDownloads": true,
      "defenderScheduleScanEnableLowCpuPriority": true,
      "defenderDisableCatchupQuickScan": true,
      "defenderDisableCatchupFullScan": true,
      "defenderScanScriptsLoadedInInternetExplorer": true,
      "defenderBlockEndUserAccess": true,
      "defenderSignatureUpdateIntervalInHours": 6,
      "defenderMonitorFileActivity": "disable",
      "defenderDaysBeforeDeletingQuarantinedMalware": 12,
      "defenderScanMaxCpu": 2,
      "defenderScanArchiveFiles": true,
      "defenderScanIncomingMail": true,
      "defenderScanRemovableDrivesDuringFullScan": true,
      "defenderScanMappedNetworkDrivesDuringFullScan": true,
      "defenderScanNetworkFiles": true,
      "defenderRequireCloudProtection": true,
      "defenderCloudBlockLevel": "high",
      "defenderCloudExtendedTimeout": 12,
      "defenderCloudExtendedTimeoutInSeconds": 5,
      "defenderPromptForSampleSubmission": "alwaysPrompt",
      "defenderScheduledQuickScanTime": "11:58:49.3840000",
      "defenderScanType": "disabled",
      "defenderSystemScanSchedule": "everyday",
      "defenderScheduledScanTime": "11:59:10.9990000",
      "defenderPotentiallyUnwantedAppAction": "block",
      "defenderPotentiallyUnwantedAppActionSetting": "enable",
      "defenderSubmitSamplesConsentType": "alwaysPrompt",
      "defenderBlockOnAccessProtection": true,
      "defenderDetectedMalwareActions": {
        "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
        "lowSeverity": "clean",
        "moderateSeverity": "clean",
        "highSeverity": "clean",
        "severeSeverity": "clean"
      },
      "defenderFileExtensionsToExclude": [
        "Defender File Extensions To Exclude value"
      ],
      "defenderFilesAndFoldersToExclude": [
        "Defender Files And Folders To Exclude value"
      ],
      "defenderProcessesToExclude": [
        "Defender Processes To Exclude value"
      ],
      "lockScreenAllowTimeoutConfiguration": true,
      "lockScreenBlockActionCenterNotifications": true,
      "lockScreenBlockCortana": true,
      "lockScreenBlockToastNotifications": true,
      "lockScreenTimeoutInSeconds": 10,
      "lockScreenActivateAppsWithVoice": "enabled",
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordMinimumCharacterSetCount": 0,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordRequired": true,
      "passwordRequireWhenResumeFromIdleState": true,
      "passwordRequiredType": "alphanumeric",
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordMinimumAgeInDays": 8,
      "privacyAdvertisingId": "blocked",
      "privacyAutoAcceptPairingAndConsentPrompts": true,
      "privacyDisableLaunchExperience": true,
      "privacyBlockInputPersonalization": true,
      "privacyBlockPublishUserActivities": true,
      "privacyBlockActivityFeed": true,
      "activateAppsWithVoice": "enabled",
      "startBlockUnpinningAppsFromTaskbar": true,
      "startMenuAppListVisibility": "collapse",
      "startMenuHideChangeAccountSettings": true,
      "startMenuHideFrequentlyUsedApps": true,
      "startMenuHideHibernate": true,
      "startMenuHideLock": true,
      "startMenuHidePowerButton": true,
      "startMenuHideRecentJumpLists": true,
      "startMenuHideRecentlyAddedApps": true,
      "startMenuHideRestartOptions": true,
      "startMenuHideShutDown": true,
      "startMenuHideSignOut": true,
      "startMenuHideSleep": true,
      "startMenuHideSwitchAccount": true,
      "startMenuHideUserTile": true,
      "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
      "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
      "startMenuMode": "fullScreen",
      "startMenuPinnedFolderDocuments": "hide",
      "startMenuPinnedFolderDownloads": "hide",
      "startMenuPinnedFolderFileExplorer": "hide",
      "startMenuPinnedFolderHomeGroup": "hide",
      "startMenuPinnedFolderMusic": "hide",
      "startMenuPinnedFolderNetwork": "hide",
      "startMenuPinnedFolderPersonalFolder": "hide",
      "startMenuPinnedFolderPictures": "hide",
      "startMenuPinnedFolderSettings": "hide",
      "startMenuPinnedFolderVideos": "hide",
      "settingsBlockSettingsApp": true,
      "settingsBlockSystemPage": true,
      "settingsBlockDevicesPage": true,
      "settingsBlockNetworkInternetPage": true,
      "settingsBlockPersonalizationPage": true,
      "settingsBlockAccountsPage": true,
      "settingsBlockTimeLanguagePage": true,
      "settingsBlockEaseOfAccessPage": true,
      "settingsBlockPrivacyPage": true,
      "settingsBlockUpdateSecurityPage": true,
      "settingsBlockAppsPage": true,
      "settingsBlockGamingPage": true,
      "windowsSpotlightBlockConsumerSpecificFeatures": true,
      "windowsSpotlightBlocked": true,
      "windowsSpotlightBlockOnActionCenter": true,
      "windowsSpotlightBlockTailoredExperiences": true,
      "windowsSpotlightBlockThirdPartyNotifications": true,
      "windowsSpotlightBlockWelcomeExperience": true,
      "windowsSpotlightBlockWindowsTips": true,
      "windowsSpotlightConfigureOnLockScreen": "disabled",
      "networkProxyApplySettingsDeviceWide": true,
      "networkProxyDisableAutoDetect": true,
      "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
      "networkProxyServer": {
        "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
        "address": "Address value",
        "exceptions": [
          "Exceptions value"
        ],
        "useForLocalAddresses": true
      },
      "accountsBlockAddingNonMicrosoftAccountEmail": true,
      "antiTheftModeBlocked": true,
      "bluetoothBlocked": true,
      "cameraBlocked": true,
      "connectedDevicesServiceBlocked": true,
      "certificatesBlockManualRootCertificateInstallation": true,
      "copyPasteBlocked": true,
      "cortanaBlocked": true,
      "deviceManagementBlockFactoryResetOnMobile": true,
      "deviceManagementBlockManualUnenroll": true,
      "safeSearchFilter": "strict",
      "edgeBlockPopups": true,
      "edgeBlockSearchSuggestions": true,
      "edgeBlockSearchEngineCustomization": true,
      "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
      "edgeSendIntranetTrafficToInternetExplorer": true,
      "edgeRequireSmartScreen": true,
      "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
      "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
      "edgeSearchEngine": {
        "@odata.type": "microsoft.graph.edgeSearchEngineBase"
      },
      "edgeHomepageUrls": [
        "Edge Homepage Urls value"
      ],
      "edgeBlockAccessToAboutFlags": true,
      "smartScreenBlockPromptOverride": true,
      "smartScreenBlockPromptOverrideForFiles": true,
      "webRtcBlockLocalhostIpAddress": true,
      "internetSharingBlocked": true,
      "settingsBlockAddProvisioningPackage": true,
      "settingsBlockRemoveProvisioningPackage": true,
      "settingsBlockChangeSystemTime": true,
      "settingsBlockEditDeviceName": true,
      "settingsBlockChangeRegion": true,
      "settingsBlockChangeLanguage": true,
      "settingsBlockChangePowerSleep": true,
      "locationServicesBlocked": true,
      "microsoftAccountBlocked": true,
      "microsoftAccountBlockSettingsSync": true,
      "nfcBlocked": true,
      "resetProtectionModeBlocked": true,
      "screenCaptureBlocked": true,
      "storageBlockRemovableStorage": true,
      "storageRequireMobileDeviceEncryption": true,
      "usbBlocked": true,
      "voiceRecordingBlocked": true,
      "wiFiBlockAutomaticConnectHotspots": true,
      "wiFiBlocked": true,
      "wiFiBlockManualConfiguration": true,
      "wiFiScanInterval": 0,
      "wirelessDisplayBlockProjectionToThisDevice": true,
      "wirelessDisplayBlockUserInputFromReceiver": true,
      "wirelessDisplayRequirePinForPairing": true,
      "windowsStoreBlocked": true,
      "appsAllowTrustedAppsSideloading": "blocked",
      "windowsStoreBlockAutoUpdate": true,
      "developerUnlockSetting": "blocked",
      "sharedUserAppDataAllowed": true,
      "appsBlockWindowsStoreOriginatedApps": true,
      "windowsStoreEnablePrivateStoreOnly": true,
      "storageRestrictAppDataToSystemVolume": true,
      "storageRestrictAppInstallToSystemVolume": true,
      "gameDvrBlocked": true,
      "experienceBlockDeviceDiscovery": true,
      "experienceBlockErrorDialogWhenNoSIM": true,
      "experienceBlockTaskSwitcher": true,
      "logonBlockFastUserSwitching": true,
      "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
      "appManagementMSIAllowUserControlOverInstall": true,
      "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
      "dataProtectionBlockDirectMemoryAccess": true,
      "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
        "App Management Package Family Names To Launch After Log On value"
      ],
      "uninstallBuiltInApps": true,
      "configureTimeZone": "Configure Time Zone value"
    }
  ]
}
```




