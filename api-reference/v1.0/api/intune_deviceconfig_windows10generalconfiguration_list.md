# <a name="list-windows10generalconfigurations"></a><span data-ttu-id="e77d4-101">Listar windows10GeneralConfigurations</span><span class="sxs-lookup"><span data-stu-id="e77d4-101">List windows10GeneralConfigurations</span></span>

> <span data-ttu-id="e77d4-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e77d4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e77d4-103">Listar propriedades e relações dos objetos [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e77d4-103">List properties and relationships of the [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e77d4-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e77d4-104">Prerequisites</span></span>
<span data-ttu-id="e77d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="e77d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e77d4-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e77d4-107">Permission type</span></span>|<span data-ttu-id="e77d4-108">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e77d4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e77d4-109">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e77d4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e77d4-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="e77d4-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="e77d4-111">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e77d4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e77d4-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e77d4-112">Not supported.</span></span>|
|<span data-ttu-id="e77d4-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e77d4-113">Application</span></span>|<span data-ttu-id="e77d4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e77d4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e77d4-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e77d4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e77d4-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e77d4-116">Request headers</span></span>
|<span data-ttu-id="e77d4-117">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e77d4-117">Header</span></span>|<span data-ttu-id="e77d4-118">Valor</span><span class="sxs-lookup"><span data-stu-id="e77d4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e77d4-119">Autorização</span><span class="sxs-lookup"><span data-stu-id="e77d4-119">Authorization</span></span>|<span data-ttu-id="e77d4-120">Token&gt; de portador obrigatório.&lt;</span><span class="sxs-lookup"><span data-stu-id="e77d4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e77d4-121">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e77d4-121">Accept</span></span>|<span data-ttu-id="e77d4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e77d4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e77d4-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e77d4-123">Request body</span></span>
<span data-ttu-id="e77d4-124">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e77d4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e77d4-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="e77d4-125">Response</span></span>
<span data-ttu-id="e77d4-126">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e77d4-126">If successful, this method returns a `200 OK` response code and a collection of [windows10GeneralConfiguration](../resources/intune_deviceconfig_windows10generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e77d4-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e77d4-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="e77d4-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e77d4-128">Request</span></span>
<span data-ttu-id="e77d4-129">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e77d4-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="e77d4-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="e77d4-130">Response</span></span>
<span data-ttu-id="e77d4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e77d4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 10832

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
      "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
      "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
      "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
      "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
      "enterpriseCloudPrintDiscoveryMaxLimit": 5,
      "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
      "searchBlockDiacritics": true,
      "searchDisableAutoLanguageDetection": true,
      "searchDisableIndexingEncryptedItems": true,
      "searchEnableRemoteQueries": true,
      "searchDisableIndexerBackoff": true,
      "searchDisableIndexingRemovableDrive": true,
      "searchEnableAutomaticIndexSizeManangement": true,
      "diagnosticsDataSubmissionMode": "none",
      "oneDriveDisableFileSync": true,
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
      "cellularBlockDataWhenRoaming": true,
      "cellularBlockVpn": true,
      "cellularBlockVpnWhenRoaming": true,
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
      "privacyAdvertisingId": "blocked",
      "privacyAutoAcceptPairingAndConsentPrompts": true,
      "privacyBlockInputPersonalization": true,
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
      "logonBlockFastUserSwitching": true
    }
  ]
}
```








