---
title: Get windows10GeneralConfiguration
description: Ler propriedades e relações do objeto windows10GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6c6884a860f1227b5d17561cd630bdb9d4cf27a0
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30956601"
---
# <a name="get-windows10generalconfiguration"></a><span data-ttu-id="a1057-103">Get windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1057-103">Get windows10GeneralConfiguration</span></span>

> <span data-ttu-id="a1057-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1057-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1057-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1057-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1057-106">Ler propriedades e relações do objeto [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a1057-106">Read properties and relationships of the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1057-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a1057-107">Prerequisites</span></span>
<span data-ttu-id="a1057-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1057-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1057-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1057-110">Permission type</span></span>|<span data-ttu-id="a1057-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a1057-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1057-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1057-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1057-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1057-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="a1057-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1057-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1057-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1057-115">Not supported.</span></span>|
|<span data-ttu-id="a1057-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1057-116">Application</span></span>|<span data-ttu-id="a1057-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1057-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1057-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1057-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1057-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a1057-119">Optional query parameters</span></span>
<span data-ttu-id="a1057-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a1057-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1057-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1057-121">Request headers</span></span>
|<span data-ttu-id="a1057-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a1057-122">Header</span></span>|<span data-ttu-id="a1057-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a1057-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1057-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1057-124">Authorization</span></span>|<span data-ttu-id="a1057-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1057-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1057-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a1057-126">Accept</span></span>|<span data-ttu-id="a1057-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a1057-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1057-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1057-128">Request body</span></span>
<span data-ttu-id="a1057-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a1057-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1057-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1057-130">Response</span></span>
<span data-ttu-id="a1057-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1057-131">If successful, this method returns a `200 OK` response code and [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1057-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1057-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1057-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1057-133">Request</span></span>
<span data-ttu-id="a1057-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1057-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="a1057-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1057-135">Response</span></span>
<span data-ttu-id="a1057-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1057-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 14347

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
    "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "taskManagerBlockEndTask": true,
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
    "securityBlockAzureADJoinedDevicesAutoEncryption": true,
    "diagnosticsDataSubmissionMode": "none",
    "oneDriveDisableFileSync": true,
    "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
    "edgeTelemetryForMicrosoft365Analytics": "intranet",
    "inkWorkspaceAccess": "enabled",
    "inkWorkspaceAccessState": "blocked",
    "inkWorkspaceBlockSuggestedApps": true,
    "smartScreenEnableAppInstallControl": true,
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
    "defenderBlockEndUserAccess": true,
    "defenderDaysBeforeDeletingQuarantinedMalware": 12,
    "defenderDetectedMalwareActions": {
      "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
      "lowSeverity": "clean",
      "moderateSeverity": "clean",
      "highSeverity": "clean",
      "severeSeverity": "clean"
    },
    "defenderSystemScanSchedule": "everyday",
    "defenderFilesAndFoldersToExclude": [
      "Defender Files And Folders To Exclude value"
    ],
    "defenderFileExtensionsToExclude": [
      "Defender File Extensions To Exclude value"
    ],
    "defenderScanMaxCpu": 2,
    "defenderMonitorFileActivity": "disable",
    "defenderPotentiallyUnwantedAppAction": "block",
    "defenderPotentiallyUnwantedAppActionSetting": "enable",
    "defenderProcessesToExclude": [
      "Defender Processes To Exclude value"
    ],
    "defenderPromptForSampleSubmission": "alwaysPrompt",
    "defenderRequireBehaviorMonitoring": true,
    "defenderRequireCloudProtection": true,
    "defenderRequireNetworkInspectionSystem": true,
    "defenderRequireRealTimeMonitoring": true,
    "defenderScanArchiveFiles": true,
    "defenderScanDownloads": true,
    "defenderScheduleScanEnableLowCpuPriority": true,
    "defenderDisableCatchupQuickScan": true,
    "defenderDisableCatchupFullScan": true,
    "defenderScanNetworkFiles": true,
    "defenderScanIncomingMail": true,
    "defenderScanMappedNetworkDrivesDuringFullScan": true,
    "defenderScanRemovableDrivesDuringFullScan": true,
    "defenderScanScriptsLoadedInInternetExplorer": true,
    "defenderSignatureUpdateIntervalInHours": 6,
    "defenderScanType": "disabled",
    "defenderScheduledScanTime": "11:59:10.9990000",
    "defenderScheduledQuickScanTime": "11:58:49.3840000",
    "defenderCloudBlockLevel": "high",
    "defenderCloudExtendedTimeout": 12,
    "defenderCloudExtendedTimeoutInSeconds": 5,
    "defenderBlockOnAccessProtection": true,
    "defenderSubmitSamplesConsentType": "alwaysPrompt",
    "lockScreenAllowTimeoutConfiguration": true,
    "lockScreenBlockActionCenterNotifications": true,
    "lockScreenBlockCortana": true,
    "lockScreenBlockToastNotifications": true,
    "lockScreenTimeoutInSeconds": 10,
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
    ]
  }
}
```




