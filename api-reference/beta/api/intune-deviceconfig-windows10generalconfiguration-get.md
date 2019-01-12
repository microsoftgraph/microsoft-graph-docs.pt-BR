---
title: Get windows10GeneralConfiguration
description: Ler propriedades e relações do objeto windows10GeneralConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a4b7690250862080e53fe5458e178a094672f2b6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947845"
---
# <a name="get-windows10generalconfiguration"></a><span data-ttu-id="36355-103">Get windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="36355-103">Get windows10GeneralConfiguration</span></span>

> <span data-ttu-id="36355-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="36355-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36355-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="36355-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="36355-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="36355-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="36355-107">Ler propriedades e relações do objeto [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36355-107">Read properties and relationships of the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="36355-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="36355-108">Prerequisites</span></span>
<span data-ttu-id="36355-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36355-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36355-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36355-111">Permission type</span></span>|<span data-ttu-id="36355-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="36355-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36355-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36355-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36355-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="36355-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="36355-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36355-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36355-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36355-116">Not supported.</span></span>|
|<span data-ttu-id="36355-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36355-117">Application</span></span>|<span data-ttu-id="36355-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36355-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="36355-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36355-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36355-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="36355-120">Optional query parameters</span></span>
<span data-ttu-id="36355-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="36355-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="36355-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36355-122">Request headers</span></span>
|<span data-ttu-id="36355-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="36355-123">Header</span></span>|<span data-ttu-id="36355-124">Valor</span><span class="sxs-lookup"><span data-stu-id="36355-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36355-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="36355-125">Authorization</span></span>|<span data-ttu-id="36355-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36355-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36355-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="36355-127">Accept</span></span>|<span data-ttu-id="36355-128">application/json</span><span class="sxs-lookup"><span data-stu-id="36355-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36355-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36355-129">Request body</span></span>
<span data-ttu-id="36355-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36355-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36355-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="36355-131">Response</span></span>
<span data-ttu-id="36355-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36355-132">If successful, this method returns a `200 OK` response code and [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36355-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36355-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="36355-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36355-134">Request</span></span>
<span data-ttu-id="36355-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36355-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="36355-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="36355-136">Response</span></span>
<span data-ttu-id="36355-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36355-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 12903

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
    "windows10AppsForceUpdateSchedule": {
      "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "recurrence": "daily",
      "runImmediatelyIfAfterStartDateTime": true
    },
    "enableAutomaticRedeployment": true,
    "assignedAccessSingleModeUserName": "Assigned Access Single Mode User Name value",
    "assignedAccessSingleModeAppUserModelId": "Assigned Access Single Mode App User Model Id value",
    "microsoftAccountSignInAssistantSettings": "disabled",
    "authenticationAllowSecondaryDevice": true,
    "authenticationAllowFIDODevice": true,
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
    "defenderScheduleScanDay": "monday",
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
    "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
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
    "dataProtectionBlockDirectMemoryAccess": true
  }
}
```





