# <a name="changelog-for-microsoft-graph"></a>Log de mudanças do Microsoft Graph

Esse log de mudanças cobre o que foi alterado no Microsoft Graph, incluindo a versão 1.0 e a beta ponto de extremidade e APIs do Microsoft Graph para pontos de extremidade beta.  

## <a name="april-2017"></a>Abril de 2017

### <a name="application-and-serviceprincipal-api-changes"></a>Alterações de API de aplicativo e ServicePrincipal

|**Alterar tipo**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Change|Beta| As APIs de [aplicativo](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/application) e [servicePrincipal](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/serviceprincipal) serão atualizadas na visualização (beta). O primeiro conjunto de alterações será aplicado em 8 de maio de 2017. As alterações incluem a renomeação e a reestruturação de propriedade. Algumas propriedades (como funções de aplicativos e suplementos) não estarão disponíveis até que as alterações sejam concluídas. As alterações serão lançadas na Visualização (beta) antes do lançamento da versão 1.0. |

### <a name="added-preview-support-for-cloud-solution-provider-developers"></a>Foi adicionado o suporte à visualização para desenvolvedores de Provedor de Soluções na Nuvem

|**Alterar tipo**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Addition|Beta|Foram adicionados novos recursos de visualização para permitir que os aplicativos previamente consentidos do Provedor de Soluções na Nuvem chamem o Microsoft Graph, descrito em um novo [tópico de autorização](https://graph.microsoft.io/en-us/docs/authorization/auth_cloudsolutionprovider). |

### <a name="added-onpremises-properties-to-user-entity"></a>Adicionadas propriedades onPremises à entidade do usuário

|**Alterar tipo**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Addition|Beta|Foram adicionadas novas propriedades onPremises, onPremisesDomainName, OnPremisesSamAccountName e onPremisesUserPrincipalName à entidade do [usuário](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/user). |

### <a name="new-planner-apis-and-an-update-to-the-group-visibility-property"></a>Novas APIs do Planner e uma atualização da propriedade de visibilidade do grupo

|**Alterar tipo**|**Versão**|**Descrição**| 
|:-------------|:-----------|:--------------|
|Change|Beta|Foi adicionado o **HiddenMembership** como um valor adicional para a propriedade de visibilidade para a entidade de [Grupo](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/group) |
|Addition|Beta|Foi adicionada uma nova [API do Planner](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/planner_overview).<br />Novos recursos:<br />[plannerPlan](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerPlan) <br />[plannerTask](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerTask) <br />[plannerPlanDetails](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerPlanDetails) <br />[plannerTaskDetails](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerTaskDetails) <br />[plannerBucket](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerBucket) <br />[plannerAssignedToTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerassignedtotaskboardtaskformat) <br />[plannerBucketTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerbuckettaskboardtaskformat) <br />[plannerProgressTaskBoardTaskFormat](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/plannerprogresstaskboardtaskformat) | 

### <a name="intune-apis"></a>APIs do Intune
|**Alterar tipo**|**Versão**|**Descrição**|
|:---|:---|:---|
|Addition|Beta|Foram adicionadas novas entidades:<br/>[androidForWorkCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkcompliancepolicy)<br/>[deviceComplianceSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate)<br/>[deviceInstallState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_deviceinstallstate)<br/>[deviceManagementScript](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript)<br/>[deviceManagementScriptGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptgroupassignment)<br/>[deviceManagementScriptState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptstate)<br/>[eBookGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_ebookgroupassignment)<br/>[iosVppEBook](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_iosvppebook)<br/>[managedEBook](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_managedebook)<br/>[userInstallStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_books_userinstallstatesummary)<br/>[windowsManagementApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp)<br/>[windowsManagementAppHealthState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapphealthstate)<br/>|
|Addition|Beta|Foram adicionados novos tipos complexos:<br/>[dailySchedule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_dailyschedule)<br/>[hourlySchedule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_hourlyschedule)<br/>[iosBookmark](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosbookmark)<br/>[iosWebContentFilterAutoFilter](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterautofilter)<br/>[iosWebContentFilterBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterbase)<br/>[iosWebContentFilterSpecificWebsitesAccess](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterspecificwebsitesaccess)<br/>[runSchedule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_runschedule)<br/>[sharedAppleDeviceUser](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_sharedappledeviceuser)<br/>[windows10NetworkProxyServer](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10networkproxyserver)<br/>|
|Addition|Beta|Foi adicionada a ação [requestRemoteAssistance](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_devicefe_manageddevice_requestremoteassistance.md) ao [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_manageddevice) |
|Addition|Beta|Foi adicionada a ação [cleanWindowsDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_devicefe_manageddevice_cleanwindowsdevice.md) ao [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_manageddevice) |
|Addition|Beta|Foi adicionada a ação [logoutSharedAppleDeviceActiveUser](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_devicefe_manageddevice_logoutsharedappledeviceactiveuser.md) ao [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_manageddevice) |
|Addition|Beta|Foi adicionada a ação [deleteUserFromSharedAppleDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_devicefe_manageddevice_deleteuserfromsharedappledevice.md) ao [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_manageddevice) |
|Addition|Beta|Foi adicionada a ação [assign](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_devicefe_devicemanagementscript_assign.md) ao [deviceManagementScript](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript) |
|Addition|Beta|Foi adicionada a ação [syncLicenses](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_onboarding_applevolumepurchaseprogramtoken_synclicenses.md) ao [appleVolumePurchaseProgramToken](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_applevolumepurchaseprogramtoken) |
|Addition|Beta|Foi adicionada a função **getMobileAppCount** à coleção [mobileApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) |
|Addition|Beta|Foi adicionada a função **getTopMobileApps** à coleção [mobileApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) |
|Addition|Beta|Foi adicionada a função [downloadApplePushNotificationCertificateSigningRequest](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_devicefe_applepushnotificationcertificate_downloadapplepushnotificationcertificatesigningrequest.md) a [applePushNotificationCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_applepushnotificationcertificate) |
|Addition|Beta|Foi adicionada a função [getDeviceComplianceSettingStates](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_devicemanagement_getdevicecompliancesettingstates.md) a [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) |
|Addition|Beta|Foi adicionada a função [deviceConfigurationUserActivity](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_reportroot_deviceconfigurationuseractivity.md) a [reportRoot](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_reportroot) |
|Addition|Beta|Foi adicionada a função [deviceConfigurationDeviceActivity](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_reportroot_deviceconfigurationdeviceactivity.md) a [reportRoot](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_reportroot) |
|Deletion|Beta|Foram removidos os seguintes tipos complexos:<br/>**enterpriseCloudResource**<br/>**windowsInformationProtectionAppRule**<br/>**windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate**<br/>**windowsInformationProtectionAppRuleDesktopTemplate**<br/>**windowsInformationProtectionAppRuleStoreAppTemplate**<br/>**windowsInformationProtectionAppRuleTemplate**<br/>**windowsInformationProtectionCorporateNetworkLocation**<br/>**windowsInformationProtectionProtectedLocation**<br/>**windowsInformationProtectionProtectedLocationEnterpriseCloudResources**<br/>**windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames**<br/>**windowsInformationProtectionProtectedLocationEnterpriseProxyServers**<br/>**windowsInformationProtectionProtectedLocationNeutralResources**<br/>|
|Change|Beta|Foi adicionada a propriedade **deviceSharingAllowed** à entidade [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration)|
|Change|Beta|Foi removida a propriedade **deviceSharingBlocked** à entidade [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration)|
|Change|Beta|Foi adicionada a propriedade **minimumRequiredSdkVersion** à entidade [defaultManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection)|
|Change|Beta|Foi adicionada a propriedade **windowsManagementAppEnabled** à entidade [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement)|
|Change|Beta|Adicionada a propriedade **notificationTemplateId** à entidade [deviceComplianceActionItem](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceactionitem)|
|Change|Beta|Foi adicionada a propriedade **excludeGroup** à entidade [deviceConfigurationGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationgroupassignment)|
|Change|Beta|Foram alteradas as seguintes propriedades na entidade [iosCustomConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioscustomconfiguration):<br/>**payloadFileName** de opcional para obrigatório<br/>|
|Change|Beta|Foi adicionada a propriedade **contentFilterSettings** à entidade [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration)|
|Change|Beta|Adicionadas as propriedades **cellularBlockPersonalHotspot** e **passcodeBlockFingerprintModification** à entidade [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration)|
|Change|Beta|Foi adicionada a propriedade **minimumRequiredSdkVersion** à entidade [iosManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection)|
|Change|Beta|Foram alteradas as seguintes propriedades na entidade [macOSCustomConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscustomconfiguration):<br/>**payloadFileName** de opcional para obrigatório<br/>|
|Change|Beta|Foram adicionadas as propriedades **disableAppPinIfDevicePinIsSet**, **minimumRequiredOsVersion**, **minimumWarningOsVersion**, **minimumRequiredAppVersion** e **minimumWarningAppVersion** à entidade [managedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedappprotection)|
|Change|Beta|Foram adicionadas as propriedades **remoteAssistanceSessionUrl**, **isEncrypted**, **modelo** e **fabricante** à entidade [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_manageddevice)|
|Change|Beta|Foi adicionada a propriedade **vpnConfigurationId** à entidade [mobileAppGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappgroupassignment)|
|Change|Beta|Foi removida a propriedade **fromEmailAddress** da entidade [notificationMessageTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_notificationmessagetemplate)|
|Change|Beta|Foi adicionada a propriedade **excludedApps** à entidade [officeSuiteApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp)|
|Change|Beta|Foi removida a propriedade **excludedOfficeApps** da entidade [officeSuiteApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp)|
|Change|Beta|Foi adicionada a propriedade **enabled** à entidade [sharedPCConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcconfiguration)|
|Change|Beta|Foram adicionadas as propriedades **networkProxyApplySettingsDeviceWide**, **networkProxyDisableAutoDetect**, **networkProxyAutomaticConfigurationUrl**, **networkProxyServer**, **bluetoothDeviceName**, **wiFiScanInterval**, **wirelessDisplayBlockProjectionToThisDevice**, **wirelessDisplayBlockUserInputFromReceiver**, **wirelessDisplayRequirePinForPairing**, **experienceBlockDeviceDiscovery**, **experienceBlockErrorDialogWhenNoSIM**, **experienceBlockTaskSwitcher**, ** startMenuPinnedFolderDocuments**, **startMenuPinnedFolderDownloads**, **startMenuPinnedFolderFileExplorer**, **startMenuPinnedFolderHomeGroup**, **startMenuPinnedFolderMusic**, **startMenuPinnedFolderNetwork**, **startMenuPinnedFolderPersonalFolder**, **startMenuPinnedFolderPictures**, **startMenuPinnedFolderSettings**, **startMenuPinnedFolderVideos**, **startMenuAppListVisibility**, **startMenuHideFrequentlyUsedApps**, ** startMenuHideRecentJumpLists**, **startMenuHideRecentlyAddedApps**, **startMenuHideRestartOptions**, **startMenuHideUserTile**, **startMenuHidePowerButton**, **startMenuLayoutEdgeAssetsXml**, **personalizationDesktopImageUrl** e **personalizationLockScreenImageUrl** à entidade [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration)|
|Change|Beta|Foi alterado o tipo das seguintes propriedades na entidade [windowsMobileMSI](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi):<br/>**productCode** do Guid para a cadeia de caracteres<br/>|
|Change|Beta|Foram alteradas as seguintes propriedades na entidade [windowsPhone81AppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx):<br/>**phoneProductIdentifier** de obrigatório para opcional<br/>**phonePublisherId** de obrigatório para opcional<br/>|
|Change|Beta|Foram alteradas as seguintes propriedades na entidade [windowsPhone81AppXBundle](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appxbundle):<br/>**appXPackageInformationList** de obrigatório para opcional<br/>|
|Change|Beta|Foram adicionadas as propriedades **productKey** e **licenseType** à entidade [windowsStoreForBusinessApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsstoreforbusinessapp)|
|Change|Beta|Foi adicionada a propriedade **previewBuildSetting** à entidade [windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration)|
|Change|Beta|Foram adicionadas as propriedades de navegação **windowsManagementApp** e **managedEBooks** à entidade [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement)|
|Change|Beta|Foram adicionadas as propriedades de navegação **deviceManagementScripts**, **managedDeviceOverview** e **cloudPkiSubscriptions** à entidade [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement)|
|Change|Beta|Foram adicionadas as propriedades **osMinimumVersion** e **osMaximumVersion** ao tipo complexo [deviceEnrollmentPlatformRestrictions](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_deviceenrollmentplatformrestrictions)|
|Change|Beta|Foram adicionadas as propriedades **isSharedDevice** e **sharedDeviceCachedUsers** ao tipo complexo [hardwareInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_hardwareinformation)|
|Change|Beta|Foram alteradas as seguintes propriedades no tipo complexo [omaSettingBase64](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_omasettingbase64):<br/>**fileName** de obrigatório para opcional<br/>|
|Change|Beta|Foram alteradas as seguintes propriedades no tipo complexo [omaSettingStringXml](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_omasettingstringxml):<br/>**fileName** de obrigatório para opcional<br/>|

## <a name="march-2017"></a>Março de 2017

### <a name="intune-apis"></a>APIs do Intune

|Alterar tipo|Versão|Descrição|
|:---|:---|:---|
|Addition|Beta|Foram adicionadas novas entidades:<br/>[androidForWorkApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_androidforworkapp)<br/>[androidForWorkAppConfigurationSchema](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationschema)<br/>[androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings)<br/>[androidForWorkVpnConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkvpnconfiguration)<br/>[applePushNotificationCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_applepushnotificationcertificate)<br/>[complianceSettingStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_compliancesettingstatesummary)<br/>[deviceCompliancePolicyDeviceStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary)<br/>[deviceCompliancePolicyState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicystate)<br/>[deviceConfigurationDeviceStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatesummary)<br/>[deviceConfigurationState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationstate)<br/>[enterpriseCodeSigningCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_enterprisecodesigningcertificate)<br/>[iosEduDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosedudeviceconfiguration)<br/>[managedDeviceCertificateState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_manageddevicecertificatestate)<br/>[managedDeviceMobileAppConfigurationDeviceSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicesummary)<br/>[managedDeviceMobileAppConfigurationUserSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationusersummary)<br/>[mdmWindowsInformationProtectionPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_mdmwindowsinformationprotectionpolicy)<br/>[mobileAppInstallSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallsummary)<br/>[mobileAppProvisioningConfigGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappprovisioningconfiggroupassignment)<br/>[mobileThreatDefenseConnector](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_mobilethreatdefenseconnector)<br/>[officeSuiteApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp)<br/>[settingStateDeviceSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_settingstatedevicesummary)<br/>[softwareUpdateStatusSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_softwareupdatestatussummary)<br/>[symantecCodeSigningCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_symanteccodesigningcertificate)<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration)<br/>[windowsInformationProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection)<br/>[windowsInformationProtectionAppLockerFile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionapplockerfile)<br/>[windowsInformationProtectionPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionpolicy)<br/>[windowsMobileMSI](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi)<br/>|
|Addition|Beta|Foram adicionados novos tipos complexos:<br/>[androidForWorkAppConfigurationExample](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationexample)<br/>[androidForWorkAppConfigurationExampleJson](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationexamplejson)<br/>[androidForWorkAppConfigurationSchemaItem](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationschemaitem)<br/>[deviceCompliancePolicySettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate)<br/>[deviceConfigurationSettingState](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate)<br/>[deviceExchangeAccessStateSummary](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_deviceexchangeaccessstatesummary)<br/>[edgeSearchEngine](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchengine)<br/>[edgeSearchEngineBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchenginebase)<br/>[edgeSearchEngineCustom](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchenginecustom)<br/>[excludedApps](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_excludedapps)<br/>[iosEduCertificateSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducertificatesettings)<br/>[ipRange](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iprange)<br/>[windowsInformationProtectionApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionapp)<br/>[windowsInformationProtectionCloudResource](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioncloudresource)<br/>[windowsInformationProtectionCloudResourceCollection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioncloudresourcecollection)<br/>[windowsInformationProtectionDesktopApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondesktopapp)<br/>[windowsInformationProtectionIPRangeCollection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioniprangecollection)<br/>[windowsInformationProtectionResourceCollection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionresourcecollection)<br/>[windowsInformationProtectionStoreApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionstoreapp)<br/>|
|Addition|Beta|Foi adicionada a ação [requestSignupUrl](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_requestsignupurl) ao [androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) |
|Addition|Beta|Foi adicionada a ação [completeSignup](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_completesignup) ao [androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) |
|Addition|Beta|Foi adicionada a ação [syncApps](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_syncapps) ao [androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) |
|Addition|Beta|Foi adicionada a ação [unbind](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_unbind) ao [androidForWorkSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) |
|Addition|Beta|Foi adicionada a ação [assign](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_apps_ioslobappprovisioningconfiguration_assign) a [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) |
|Addition|Beta|Foi adicionada a ação [recoverPasscode](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_devicefe_manageddevice_recoverpasscode) a [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_manageddevice) |
|Addition|Beta|Foi adicionada a ação [removeApplePushNotificationCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_onboarding_organization_removeapplepushnotificationcertificate) a [organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_organization) |
|Addition|Beta|Foi adicionada a ação [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_iosmanagedappprotection_updatemobileappidentifierdeployments) a [iosManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) |
|Addition|Beta|Foi adicionada a ação [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_androidmanagedappprotection_updatemobileappidentifierdeployments) a [androidManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) |
|Addition|Beta|Foi adicionada a ação [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_targetedmanagedappconfiguration_updatemobileappidentifierdeployments) a [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) |
|Addition|Beta|Foi adicionada a ação [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_iosmanagedappprotection_updatetargetedsecuritygroups) a [iosManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) |
|Addition|Beta|Foi adicionada a ação [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_androidmanagedappprotection_updatetargetedsecuritygroups) a [androidManagedAppProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) |
|Addition|Beta|Foi adicionada a ação [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_windowsinformationprotection_updatetargetedsecuritygroups) a [windowsInformationProtection](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection) |
|Addition|Beta|Foi adicionada a ação [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_windowsinformationprotection_updatetargetedsecuritygroups.mdPolicy) a [windowsInformationProtectionPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionpolicy) |
|Addition|Beta|Foi adicionada a ação [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_mdmwindowsinformationprotectionpolicy_updatetargetedsecuritygroups) a [mdmWindowsInformationProtectionPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_mdmwindowsinformationprotectionpolicy) |
|Addition|Beta|Foi adicionada a ação [wipeManagedAppRegistrationByDeviceTag](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_user_wipemanagedappregistrationbydevicetag) a [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_user) |
|Addition|Beta|Foi adicionada a função [getTopMobileApps](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_apps_mobileapp_gettopmobileapps) a [mobileApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) |
|Addition|Beta|Foi adicionada a função [verifyWindowsEnrollmentAutoDiscovery](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_corpenrollment_devicemanagement_verifywindowsenrollmentautodiscovery) a [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) |
|Deletion|Beta|Foram removidas as seguintes entidades:<br/>**appProvisioningConfigGroupAssignment**<br/>**defaultManagedAppConfiguration**<br/>**enterpriseCertificate**<br/>**managedDeviceMobileAppProvisioningConfigurationDeviceStatus**<br/>**symantecCertificate**<br/>**windows10WindowsInformationProtectionConfiguration**<br/>|
|Deletion|Beta|Foram removidos os seguintes tipos complexos:<br/>**mobileAppInstallSummary**<br/>**windowsArchitecture**<br/>**windowsDeviceType**<br/>|
|Change|Beta|Foi adicionada a propriedade **webBrowserBlockPopups** à entidade [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration)|
|Change|Beta|Foi removida a propriedade **webBrowserAllowPopups** da entidade [androidGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration)|
|Change|Beta|Foi adicionada a propriedade **appIdentifier** à entidade [androidStoreApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_androidstoreapp)|
|Change|Beta|Foram removidas as propriedades **applicationCount**, **failedApplicationCount** e **appInstallFailures** da entidade [appReportingOverviewStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/appReportingOverviewStatus)|
|Change|Beta|Foram adicionadas as propriedades **sharedIPadMaximumUserCount** e **enableSharedIPad** à entidade [depEnrollmentProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_corpenrollment_depenrollmentprofile)|
|Change|Beta|Foram adicionadas as propriedades **shareTokenWithSchoolDataSyncService** e **lastSyncErrorCode** à entidade [depOnboardingSetting](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_deponboardingsetting)|
|Change|Beta|Foram adicionadas as propriedades **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** e **configurationVersion** à entidade [deviceComplianceDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview)|
|Change|Beta|Foram removidas as propriedades **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** e **policyRevision** da entidade [deviceComplianceDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview)|
|Change|Beta|Foram adicionadas as propriedades **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** e **configurationVersion** à entidade [deviceComplianceUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview)|
|Change|Beta|Foram removidas as propriedades **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** e **policyRevision** da entidade [deviceComplianceUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview)|
|Change|Beta|Foram adicionadas as propriedades **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** e **configurationVersion** à entidade [deviceConfigurationDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview)|
|Change|Beta|Foram removidas as propriedades **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** e **policyRevision** da entidade [deviceConfigurationDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview)|
|Change|Beta|Foram adicionadas as propriedades **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** e **configurationVersion** à entidade [deviceConfigurationUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview)|
|Change|Beta|Foram removidas as propriedades **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** e **policyRevision** da entidade [deviceConfigurationUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview)|
|Change|Beta|Foi adicionada a propriedade **subscriptionState** à entidade [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement)|
|Change|Beta|Foi adicionada a propriedade **managedEmailProfileRequired** à entidade [iosCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioscompliancepolicy)|
|Change|Beta|Foi adicionada a propriedade **appsSingleAppModeList** à entidade [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration)|
|Change|Beta|Foi removida a propriedade **appsSingleAppModeBundleIds** da entidade [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration)|
|Change|Beta|Foi adicionada a propriedade **expirationDateTime** à entidade [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)|
|Change|Beta|Foi removida a propriedade **expiration** da entidade [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)|
|Change|Beta|Foram adicionadas as propriedades **passwordMinimumCharacterSetCount**, **osMinimumVersion**, **osMaximumVersion**, **deviceThreatProtectionEnabled**, **deviceThreatProtectionRequiredSecurityLevel** e **storageRequireEncryption** à entidade [macOSCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscompliancepolicy)|
|Change|Beta|Foi removida a propriedade **manifest** da entidade [managedAndroidLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedandroidlobapp)|
|Change|Beta|Foram adicionadas as propriedades **isSupervised**, **exchangeLastSuccessfulSyncDateTime**, **exchangeAccessState** e **exchangeAccessStateReason** à entidade [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_manageddevice)|
|Change|Beta|Foi adicionada a propriedade **deviceExchangeAccessStateSummary** à entidade [managedDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_manageddeviceoverview)|
|Change|Beta|Foi removida a propriedade **manifest** da entidade [managedIOSLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedioslobapp)|
|Change|Beta|Foi removida a propriedade **installSummary** da entidade [mobileApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileapp)|
|Change|Beta|Foi adicionada a propriedade **uploadState** à entidade [mobileAppContentFile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile)|
|Change|Beta|Foram alteradas as seguintes propriedades na entidade [mobileAppContentFile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile):<br/>**azureStorageUriExpirationDateTime** de obrigatório para opcional<br/>|
|Change|Beta|Foram adicionadas as propriedades **initiatedByUserPrincipalName**, **deviceOwnerUserPrincipalName**, **deviceIMEI** e **actionState** à entidade [remoteActionAudit](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_remoteactionaudit)|
|Change|Beta|Foram adicionadas as propriedades **oneDriveDisableFileSync**, **safeSearchFilter**, **edgeSearchEngine**, **settingsBlockSettingsApp**, **settingsBlockSystemPage**, **settingsBlockDevicesPage**, **settingsBlockNetworkInternetPage**, **settingsBlockPersonalizationPage**, **settingsBlockAccountsPage**, **settingsBlockTimeLanguagePage**, **settingsBlockEaseOfAccessPage**, **settingsBlockPrivacyPage**, **settingsBlockUpdateSecurityPage**, ** experienceBlockWindowsSpotlight**, **experienceBlockWindowsTips**, **experienceBlockConsumerSpecificFeatures**, **startMenuLayoutXml**, **startMenuMode**, **logonBlockFastUserSwitching** e **startBlockUnpinningAppsFromTaskbar** à entidade [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration)|
|Change|Beta|Foram adicionadas as propriedades **allowPrinting**, **allowScreenCapture** e **allowTextSuggestion** à entidade [windows10SecureAssessmentConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration)|
|Change|Beta|Foram removidas as propriedades **blockPrinting**, **blockScreenCapture** e **blockTextSuggestion** da entidade [windows10SecureAssessmentConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration)|
|Change|Beta|Foi adicionada a propriedade **identityName** à entidade [windowsAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsappx)|
|Change|Beta|Foi alterado o tipo das seguintes propriedades na entidade [windowsAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsappx):<br/>**applicableArchitectures** de [windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsArchitecture) para cadeia de caracteres<br/>|
|Change|Beta|Foi adicionada a propriedade **identityName** à entidade [windowsPhone81AppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx)|
|Change|Beta|Foi alterado o tipo das seguintes propriedades na entidade [windowsPhone81AppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx):<br/>**applicableArchitectures** de [windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsArchitecture) para cadeia de caracteres<br/>|
|Change|Beta|Foram adicionadas as propriedades **identityName**, **identityPublisherHash** e **identityResourceIdentifier** à entidade [windowsUniversalAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx)|
|Change|Beta|Foi alterado o tipo das seguintes propriedades na entidade [windowsUniversalAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx):<br/>**applicableArchitectures** de [windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsArchitecture) para cadeia de caracteres<br/>**applicableDeviceTypes** de [windowsDeviceType](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsDeviceType) para a cadeia de caracteres<br/>|
|Change|Beta|Foi adicionada a propriedade **restartMode** à entidade [windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration)|
|Change|Beta|Foi adicionada a propriedade de navegação **managedDeviceCertificateStates** à entidade [androidForWorkScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile)|
|Change|Beta|Foi adicionada a propriedade de navegação **managedDeviceCertificateStates** à entidade [androidScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidscepcertificateprofile)|
|Change|Beta|Foram adicionadas as propriedades de navegação **enterpriseCodeSigningCertificates**, **symantecCodeSigningCertificate**, **sideLoadingKeys**, **managedAppPolicies**, **iosManagedAppProtections**, **androidManagedAppProtections**, **defaultManagedAppProtections**, **targetedManagedAppConfigurations**, **mdmWindowsInformationProtectionPolicies**, **windowsInformationProtectionPolicies**, **managedAppRegistrations** e **managedAppStatuses** à entidade [deviceAppManagement ](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement)|
|Change|Beta|Foram removidas as propriedades de navegação **appReportingOverview**, **enterpriseCerts** e **symantecCert** da entidade [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement)|
|Change|Beta|Foi adicionada a propriedade de navegação **deviceSettingStateSummaries** à entidade [deviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy)|
|Change|Beta|Foi adicionada a propriedade de navegação **deviceSettingStateSummaries** à entidade [deviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration)|
|Change|Beta|Foram adicionadas as propriedades de navegação **termsAndConditions**, **androidForWorkSettings**, **androidForWorkAppConfigurationSchemas**, **applePushNotificationCertificate**, **softwareUpdateStatusSummary**, **deviceCompliancePolicyDeviceStateSummary**, **complianceSettingStateSummaries**, **deviceConfigurationDeviceStateSummaries** e **mobileThreatDefenseConnectors** à entidade [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement)|
|Change|Beta|Foram removidas as propriedades de navegação **teacherRootCertificates**, **teacherIdentityCertificate**, **studentRootCertificates** e **studentIdentityCertificate** da entidade [iosEducationDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration)|
|Change|Beta|Foi alterado o tipo das seguintes propriedades na entidade [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration):<br/>**deviceStatuses** da coleção [managedDeviceMobileAppProvisioningConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/managedDeviceMobileAppProvisioningConfigurationDeviceStatus) para a coleção [managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus)<br/>**groupAssignments** da coleção [appProvisioningConfigGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/appProvisioningConfigGroupAssignment) para a coleção [mobileAppProvisioningConfigGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappprovisioningconfiggroupassignment)<br/>|
|Change|Beta|Foi adicionada a propriedade de navegação **managedDeviceCertificateStates** à entidade [iosScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosscepcertificateprofile)|
|Change|Beta|Foi adicionada a propriedade de navegação **managedDeviceCertificateStates** à entidade [macOSScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosscepcertificateprofile)|
|Change|Beta|Foram adicionadas as propriedades de navegação **deviceConfigurationStates** e **deviceCompliancePolicyStates** à entidade [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devicefe_manageddevice)|
|Change|Beta|Foram adicionadas as propriedades de navegação **deviceStatusSummary** e **userStatusSummary** à entidade [managedDeviceMobileAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration)|
|Change|Beta|Foi adicionada a propriedade de navegação **installSummary** à entidade [mobileApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileapp)|
|Change|Beta|Foi removida a propriedade de navegação **sideLoadingKeys** da entidade [organization](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_organization)|
|Change|Beta|Foi adicionada a propriedade de navegação **managedDeviceCertificateStates** à entidade [windows81SCEPCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81scepcertificateprofile)|
|Change|Beta|Foi adicionada a propriedade de navegação **managedDeviceCertificateStates** à entidade [windowsPhone81SCEPCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81scepcertificateprofile)|
|Change|Beta|Foram removidas as propriedades **applicationId**, **appName**, **platformId**, **userFailures** e **deviceFailures** do tipo complexo [appInstallationFailure](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure)|
|Change|Beta|Foi adicionada a propriedade **displayName** ao tipo complexo [iosHomeScreenFolderPage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolderpage)|
|Change|Beta|Foi adicionada a propriedade **displayName** ao tipo complexo [iosHomeScreenPage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenpage)|
|Change|Beta|Foram adicionadas as propriedades **subjectName**, **description**, **expirationDateTime** e **certificate** ao tipo complexo [windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondatarecoverycertificate)|
|Change|Beta|Foram removidas as propriedades **dataRecoveryCertificate** e **certificateFileName** do tipo complexo [windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondatarecoverycertificate)|
|Change|Beta|Foi adicionada a propriedade **displayName** ao tipo complexo [windowsPackageInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation)|
|Change|Beta|Foi alterado o tipo das seguintes propriedades no tipo complexo [windowsPackageInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation):<br/>**applicableArchitecture** de [windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/windowsArchitecture) para cadeia de caracteres<br/>|
|Change|Beta|Foram alteradas as seguintes propriedades no tipo complexo [windowsPackageInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation):<br/>**applicableArchitecture** de opcional para obrigatório<br/>|

### <a name="add-contracts-to-microsoft-graph"></a>Adicionar contratos ao Microsoft Graph

|**Alterar tipo**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Addition|Beta|Novo recurso:</br>[contract](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/contract) |

### <a name="add-domain-operations-to-microsoft-graph"></a>Adicionar operações de domínio ao Microsoft Graph

|**Alterar tipo**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Addition|Beta|Adicionou funções nos [domínios](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domain).<br/>Novas entidades:</br>[domain](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domain)<br/>[domainDnsRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domaindnsrecord)<br/>[domainDnsCnameRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsCnameRecord)<br/>[domainDnsMxRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsMxRecord)<br/>[domainDnsSrvRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsSrvRecord)<br/>[domainDnsTxtRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsTxtRecord)<br/>[domainDnsUnavailableRecord](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/domainDnsUnavailableRecord)<br/>Novas ações:</br>[forceDelete](https://graph.microsoft.io/en-us/docs/api-reference/beta/api/domain_forcedelete)</br>[verify](https://graph.microsoft.io/en-us/docs/api-reference/beta/api/domain_verify) |

### <a name="add-custom-data-to-microsoft-graph-using-schema-extensions"></a>Adicionar dados personalizados ao Microsoft Graph usando extensões de esquema

|**Alterar tipo**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Addition|Beta|Estenda o Microsoft Graph com dados de aplicativos usando [extensões de esquema](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_overview#schema-extensions-preview).  Isso é suportado nos seguintes recursos:<br/>administrative unit<br/>calendar event<br/>device<br/>group<br/>message<br/>organization<br/>personal contact<br/>post<br/>user<br/>Veja o seguinte exemplo:<br/>[Adicionar dados personalizados a grupos usando Extensões do Esquema (visualização)](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_schema_groups)|
|Addition|Beta|Foi fornecido uma maneira alternativa de criar uma definição de extensão do esquema sem a necessidade de um domínio personalizado .com verificado. Consulte [extensões de esquema](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_overview#schema-extensions-preview) para obter detalhes.|

### <a name="add-custom-data-to-microsoft-graph-using-open-extensions"></a>Adicionar dados personalizados ao Microsoft Graph usando extensões abertas

|**Alterar tipo**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Change| v1.0 e beta | As "extensões de dados do Office 365" anteriores foram renomeadas como "abrir extensões". |
|Addition|Beta|Foram adicionados recursos que oferecem suporte a [extensões abertas](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_overview#open-extensions): <br/>administrative unit<br/>device<br/>group<br/>organization<br/>user<br/>Veja o seguinte exemplo:<br/>[Adicionar dados personalizados aos usuários usando extensões abertas (visualização)](https://developer.microsoft.com/en-us/graph/docs/concepts/extensibility_open_users)|

### <a name="directory-apis"></a>APIs de diretório

|**Alterar tipo**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Addition|Beta|Foi adicionado o suporte para a [restauração e a exclusão permanente de grupos](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/directory).<br/>Nova entidade: diretório com a propriedade de navegação deleteditems. |
|Addition|Beta|Nova entity:</br>[Ponto de extremidade](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/endpoint) |
|Change  |Beta|Nova propriedade de navegação nos [pontos de extremidade](https://graph.microsoft.io/en-us/docs/api-reference/beta/api/group_list_endpoints) em [grupos](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/group) |
|Addition|Beta|Nova entity:</br>[licenseDetails](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/licensedetails) |
|Change  |Beta|Nova propriedade de navegação [licensedetails](https://graph.microsoft.io/en-us/docs/api-reference/beta/api/user_list_licensedetails) em [users](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/user) |

### <a name="reports-apis"></a>APIs de relatórios

|**Alterar tipo**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Addition|Beta|Foi introduzida a nova API de visualização para relatórios do Office 365. Você pode usá-la para obter relatórios de uso sobre como as pessoas em sua empresa estão usando serviços do Office 365. Por exemplo, você pode identificar quem está usando muito um serviço e atingindo cotas, ou quem pode não precisar de uma licença do Office 365. Para obter mais detalhes, consulte o [relatório](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/report).|

### <a name="directory-apis"></a>APIs de diretório

|**Alterar tipo**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Addition|Beta|Nova entity:</br>[contract](https://graph.microsoft.io/en-us/docs/api-reference/beta/resources/contract) |

## <a name="february-2017"></a>Fevereiro de 2017

### <a name="intune-apis"></a>APIs do Intune

|Alterar tipo|Versão|Descrição|
|:---|:---|:---|
|Addition|Beta|Foram adicionadas novas entidades:<br/>[androidForWorkCertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkcertificateprofilebase)<br/>[androidForWorkEasEmailProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkeasemailprofilebase)<br/>[androidForWorkEnterpriseWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkenterprisewificonfiguration)<br/>[androidForWorkGmailEasConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkgmaileasconfiguration)<br/>[androidForWorkNineWorkEasConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworknineworkeasconfiguration)<br/>[androidForWorkPkcsCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkpkcscertificateprofile)<br/>[androidForWorkScepCertificateProfile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile)<br/>[androidForWorkTrustedRootCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworktrustedrootcertificate)<br/>[androidForWorkWiFiConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkwificonfiguration)<br/>[appleDeviceFeaturesConfigurationBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_appledevicefeaturesconfigurationbase)<br/>[appProvisioningConfigGroupAssignment](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appprovisioningconfiggroupassignment)<br/>[deviceComplianceUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview)<br/>[deviceConfigurationUserOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview)<br/>[enterpriseCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_enterprisecertificate)<br/>[iosEducationDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration)<br/>[macOSDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosdevicefeaturesconfiguration)<br/>[managedAndroidLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedandroidlobapp)<br/>[managedDeviceMobileAppProvisioningConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappprovisioningconfigurationdevicestatus)<br/>[managedIOSLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedioslobapp)<br/>[managedMobileLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_managedmobilelobapp)<br/>[symantecCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_symanteccertificate)<br/>[windowsAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsappx)<br/>[windowsCertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowscertificateprofilebase)<br/>[windowsPhone81AppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx)<br/>[windowsPhone81AppXBundle](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appxbundle)<br/>[windowsPhoneXAP](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsphonexap)<br/>[windowsUniversalAppX](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx)<br/>|
|Addition|Beta|Foram adicionados novos tipos complexos:<br/>[airPrintDestination](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_airprintdestination)<br/>[windowsArchitecture](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsarchitecture)<br/>[windowsDeviceType](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsdevicetype)<br/>[windowsMinimumOperatingSystem](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowsminimumoperatingsystem)<br/>[windowsPackageInformation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation)<br/>|
|Addition|Beta|Foi adicionada a ação [atribuir](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_apps_ioslobappprovisioningconfiguration_assign) à entidade [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)|
|Addition|Beta|Foi adicionada a ação [scheduleActionsForRules](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_deviceconfig_devicecompliancepolicy_scheduleactionsforrules) à entidade [deviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy)|
|Addition|Beta|Foi adicionada a ação [updateTargetedSecurityGroups](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_mam_targetedmanagedappconfiguration_updatetargetedsecuritygroups) à entidade [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration)|
|Addition|Beta|Foi adicionada função [getScopesForUser](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/intune_rbac_resourceoperation_getscopesforintune_devices_user) à entidade [resourceOperation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_rbac_resourceoperation)|
|Change|Beta|Removido a propriedade **manifesto** a partir da entidade [androidLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_androidlobapp) |
|Change|Beta|Foram adicionadas as propriedades **assetTagTemplate**, **lockScreenFootnote**, **homeScreenDockIcons** e **homeScreenPages** à entidade [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration) |
|Change|Beta|Foram removidas as propriedades **deviceSharingAssetTagInformation** **deviceSharingLockScreenFootnote**, **homeScreenLayoutDockIcons** e **homeScreenLayoutPages** da entidade [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration) |
|Change|Beta|Foi adicionada a propriedade **appsSingleAppModeBundleIds** à entidade [iosGeneralDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration)|
|Change|Beta|Foi removida a propriedade **manifesto** da entidade [iosLobApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobapp)|
|Change|Beta|Foram adicionadas as propriedades **createdDateTime**, **descrição**, **lastModifiedDateTime**, **displayName** e **versão** à entidade [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)|
|Change|Beta|Foram adicionadas as propriedades **createdDateTime** e **lastModifiedDateTime** à entidade [managedAppPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy) |
|Change|Beta|Foi removida a propriedade **deviceRegistrationState** da entidade [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devices_manageddevice)|
|Change|Beta|Foi adicionada a propriedade **manifesto** à entidade [mobileAppContentFile](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile)|
|Change|Beta|Foram adicionadas as propriedades **osDescription** e **userName** à entidade [mobileAppInstallStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus)|
|Change|Beta|Foi removida a propriedade **deviceType** da entidade [mobileAppInstallStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus)|
|Change|Beta|Foi alterado o tipo das seguintes propriedades na entidade [mobileAppInstallStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus):<br/>**mobileAppInstallStatusValue** de Int32 para String|
|Change|Beta|Foram adicionadas as propriedades **targetedSecurityGroupIds** e **targetedSecurityGroupsCount** à entidade [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) entidade|
|Change|Beta|Foi removida a propriedade **numberOfTargetedSecurityGroups** da entidade [targetedManagedAppConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration)|
|Change|Beta|Foi adicionada a propriedade **id** à entidade [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_devices_user) |
|Change|Beta|Foram removidas as propriedades **renewalThresholdPercentage**, **keyStorageProvider**, **subjectNameFormat**, **subjectAlternativeNameType**, **certificateValidityPeriodValue** e **certificateValidityPeriodScale** da entidade [windows10CertificateProfileBas](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10certificateprofilebase) |
|Change|Beta|Foram removidas as propriedades **renewalThresholdPercentage**, **keyStorageProvider**, **subjectNameFormat**, **subjectAlternativeNameType**, **certificateValidityPeriodValue** e **certificateValidityPeriodScale** da entidade [windows81CertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81certificateprofilebase)|
|Change|Beta|Foi removida a propriedade **applyToWindows10Mobile** da entidade [windowsPhone81GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81generalconfiguration) |
|Change|Beta|Foram adicionadas as propriedades de navegação **enterpriseCerts**, **iosLobAppProvisioningConfigurations** e **symantecCert** à entidade [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement)|
|Change|Beta|Foi adicionada a propriedade de navegação **userStatusOverview** à entidade [deviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy)|
|Change|Beta|Foi adicionada a propriedade de navegação **userStatusOverview** à entidade [deviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration)|
|Change|Beta|Foram adicionadas as propriedades de navegação **groupAssignments**, **deviceStatuses** e **userStatuses** à entidade [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)|
|Change|Beta|Foi alterado o tipo das seguintes propriedades na entidade [windows10VpnConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10vpnconfiguration):<br/>**identityCertificate** de [windows10CertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10certificateprofilebase) para [windowsCertificateProfileBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowscertificateprofilebase)|
|Change|Beta|Foram adicionadas as propriedades **deviceComplianceCheckinThresholdDays** e **isScheduledActionEnabled**ao tipo complexo [deviceManagementSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings)|
|Change|Beta|Foram removidas as propriedades **windowsCommercialId** e **windowsCommercialIdLastModifiedTime** do tipo complexo [deviceManagementSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings)|
|Change|Beta|Foram adicionadas as propriedades **bundleID**, **appName**, **publisher**, **habilitado** e **showOnLockScreen** ao tipo complexo [iosNotificationSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings) |
|Change|Beta|Foram removidas as propriedades **bundleIdentifier**, **notificationsEnabled** e **showInLockScreen** do tipo complexo [iosNotificationSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings)|



## <a name="january-2017"></a>Janeiro de 2017

### <a name="outlook-calendar"></a>Calendário do Outlook

|**Alterar tipo**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Addition|v1.0|Nova ação [findMeetingTimes](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/user_findmeetingtimes) para o recurso [user](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user).|
|Addition|v1.0|Novo tipo complexo [attendeeBase](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/attendeebase), que consiste em uma propriedade de tipo para o tipo attendee.|
|Addition|v1.0|Novos tipos complexos:<br/>[attendeeAvailability](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/attendeeavailability)<br/>[locationConstraint](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/locationconstraint) <br/>[locationConstraintItem](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/locationconstraintitem)<br/>[meetingTimeSuggestion](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/meetingtimesuggestion)<br/>[meetingTimeSuggestionsResult](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/meetingtimesuggestionsresult)<br/>[timeConstraint](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/timeconstraint)<br/>[timeSlot](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/timeslot)|
|Change|v1.0|O tipo complexo [attendee](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/attendee) agora deriva de attendeeBase,que, por sua vez, é derivado do [recipient](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/recipient). Incluindo as propriedades herdadas, ele consiste nas mesmas propriedades de antes: **status**, **type** e **emailAddress**.|
|Addition|Beta|hexColor adicionado ao recurso [calendar](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/calendar).|

### <a name="intune-apis"></a>APIs do Intune

|**Alterar tipo**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Addition|Beta|Foram adicionadas novas entidades: <br/>[appReportingOverviewStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appreportingoverviewstatus)<br/>[deviceComplianceDeviceOverview](https://developer.microsoft.com/en-us/graph/docs//api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview)<br/>[deviceConfigurationDeviceOverview](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview)<br/>[deviceManagementExchangeOnpremisesPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_devicemanagementexchangeonpremisespolicy)<br/>[iosDeviceFeaturesConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration)<br/>[iosEducationDeviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration)<br/>[iosLobAppProvisioningConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)<br/>[onpremisesConditionalAccessSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_onpremisesconditionalaccesssettings)<br/>[sharedPCConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcconfiguration)<br/>[windows10EnterpriseModernAppManagementConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration)<br/>[windows10SecureAssessmentConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration)<br/>[windows10WindowsInformationProtectionConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10windowsinformationprotectionconfiguration)|
|Addition|Beta|Foram adicionados novos tipos complexos: <br/> [appInstallationFailure](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure)<br/>[enterpriseCloudResource](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_enterprisecloudresource)<br/>[iosHomeScreenApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenapp)<br/>[iosHomeScreenFolder](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolder)<br/>[iosHomeScreenFolderPage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolderpage)<br/>[iosHomeScreenItem](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenitem)<br/>[iosHomeScreenPage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenpage)<br/>[iosNotificationSettings](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings)<br/>[iPv6Range](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_ipv6range)<br/>[sharedPCAccountManagerPolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcaccountmanagerpolicy)<br/>[windowsInformationProtectionAppRule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionapprule)<br/>[windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruleapplockerpolicyfiletemplate)<br/>[windowsInformationProtectionAppRuleDesktopTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruledesktoptemplate)<br/>[windowsInformationProtectionAppRuleStoreAppTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionapprulestoreapptemplate)<br/>[windowsInformationProtectionAppRuleTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruletemplate)<br/>[windowsInformationProtectionCorporateNetworkLocation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectioncorporatenetworklocation)<br/>[windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectiondatarecoverycertificate)<br/>[windowsInformationProtectionProtectedLocation](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocation)<br/>[windowsInformationProtectionProtectedLocationEnterpriseCloudResources](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterprisecloudresources)<br/>[windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseinternalproxyservers)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseipv4ranges)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseipv6ranges)<br/>[windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterprisenetworkdomainnames)<br/>[windowsInformationProtectionProtectedLocationEnterpriseProxyServers](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseproxyservers)<br/>[windowsInformationProtectionProtectedLocationNeutralResources](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationneutralresources)
|Deletion|Beta|Removido os seguintes tipos complexos e substituídos por microsoft.graph.Json:<br/>managedAppDeploymentSummary <br/>managedAppSummary<br /> |
|Change|Beta|Foi substituído o tipo de propriedade appConfigComplianceStatus por complianceStatus nas seguintes entidades: <br/>[managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus)<br/>[managedDeviceMobileAppConfigurationUserStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationuserstatus)|
|Change|Beta|Para o recurso [managedAppStatusRaw](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedappstatusraw), foi alterado o tipo de conteúdo de propriedade de managedAppSummary para Json.|
|Change|Beta|Foi removida a função getUsersWithFlaggedAppRegistration da coleção [managedAppRegistration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_mam_managedappregistration).|
|Change|Beta|Foi alterada a propriedade de navegação **vppToken** da entidade [iosVppApp](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_iosvppapp) para que ela deixasse de ser uma coleção contida.|
|Change|Beta|Foi adicionada a propriedade **deviceStatusOverview** às entidades [deviceConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) e [deviceCompliancePolicy](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy).|
|Change|Beta|Foi adicionada a propriedade **appReportingOverview** ao singleton [deviceAppManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement).|
|Change|Beta|Foram adicionadas as propriedades **deviceDisplayName** e **userPrincipalName** às entidades [deviceConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatus), [deviceComplianceDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedevicestatus) e [managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus).|
|Change|Beta|Foi adicionada a propriedade **ruleName** à entidade [deviceComplianceScheduledActionForRule](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancescheduledactionforrule).|
|Change|Beta|Foram adicionadas as propriedades **devicesCount**, **userDisplayName** e **userPrincipalName** às entidades [deviceConfigurationUserStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuserstatus), [deviceComplianceUserStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuserstatus) e [managedDeviceMobileAppConfigurationUserStatus](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationuserstatus).|
|Change|Beta|Foi adicionada a coleção [notificationMessageTemplates](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_notification_notificationmessagetemplate) ao singleton [deviceManagement](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagement).|
|Change|Beta|Foram adicionadas as propriedades **isDefault**, **lastModifiedDateTime**, **locale**, **messageTemplate** e **subject** à entidade [localizedNotificationMessage](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_localizednotificationmessage.md ).|
|Change|Beta|Foram adicionadas as propriedades **azureActiveDirectoryDeviceId**, **deviceCategory**, **deviceRegistrationState** e **managementAgent** à entidade [managedDevice](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_onboarding_manageddevice).|
|Change|Beta|Foi adicionada a propriedade **lastModifiedDateTime** à entidade [mobileAppCategory](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_apps_mobileappcategory).|
|Change|Beta|Foram adicionadas as propriedades **brandingOptions**, **defaultLocale**, **displayName**, **fromEmailAddress**, **lastModifiedDateTime**, **localizedNotificationMessages** à entidade [notificationMessageTemplate](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_notification_notificationmessagetemplate).|
|Change|Beta|Foram adicionadas as propriedades **appsAllowTrustedAppsSideloading**, **appsBlockWindowsStoreOriginatedApps**, **developerUnlockSetting**, **edgeBlockAccessToAboutFlags**, **edgeBlockDeveloperTools**, **edgeBlockExtensions**, **edgeBlockInPrivateBrowsing**, **edgeFirstRunUrl**, **edgeHomepageUrls**, **gameDvrBlocked**, **settingsBlockAddProvisioningPackage**, **settingsBlockChangeLanguage**, **settingsBlockChangePowerSleep**, ** settingsBlockChangeRegion**, **settingsBlockChangeSystemTime**, **settingsBlockEditDeviceName**, **settingsBlockRemoveProvisioningPackage**, **sharedUserAppDataAllowed**, **smartScreenBlockPromptOverride**, **smartScreenBlockPromptOverrideForFiles**, **storageRestrictAppDataToSystemVolume**, **storageRestrictAppInstallToSystemVolume**, **webRtcBlockLocalhostIpAddress**, **windowsStoreBlockAutoUpdate** e **windowsStoreEnablePrivateStoreOnly** à entidade [windows10GeneralConfiguration](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration).|

## <a name="december-2016"></a>Dezembro de 2016

### <a name="delta-query"></a>Consulta delta

|**Alterar tipo**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Addition|Beta|Adicionar uma nova função delta para as seguintes entidades realizem [consulta delta](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_overview):<br/>contact<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>Confira os seguintes exemplos:<br/>[Obter as alterações incrementais para grupos (visualização)](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_groups)<br/>[Obter as alterações incrementais para as mensagens em uma pasta (visualização)](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_message)<br/>[Obter as alterações incrementais para usuários (visualização)](https://developer.microsoft.com/en-us/graph/docs/concepts/delta_query_users)|

### <a name="excel-apis"></a>APIs do Excel

|**Alterar tipo**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Addition|v1.0|Foi adicionado o recurso workbookPivotTable, as ações refresh e refreshAll a Tabelas Dinâmicas, o recurso workbookRangeView, a ação visibleView ao intervalo filtrado para retornar workbookRangeView para o usuário, extrair coleção de linhas e recurso de intervalo de visibleView, columnsAfter, columnsBefore, resizedRange, rowsAbove, e funções rowsBelow do recurso de intervalo, e novas propriedades de tabela.|

### <a name="intune-apis"></a>APIs do Intune

|**Alterar tipo**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Addition|Beta|Recursos adicionados e APIs de método para o Microsoft Intune. Este é um conjunto de recursos e métodos para dar suporte à visualização pública de Intune no Portal do Azure. Para saber mais sobre o serviço do Intune, veja a [documentação do Intune ](https://go.microsoft.com/fwlink/?linkid=836405). Para saber mais sobre os recursos do Intune e APIs, veja [Trabalho com o Intune no Microsoft Graph](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/intune_graph_overview).|

## <a name="october-2016"></a>Outubro de 2016

### <a name="authorization-provider"></a>Provedor de autorização

|**Alterar tipo**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Addition|v1.0 e beta|O ponto de extremidade de autenticação v2.0 agora dá suporte à concessão do OAuth client_credentials, que pode ser usada para [daemon e processos com execução longa em cenários de negócios](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-protocols-oauth-client-creds/).|
|Addition|v1.0 e beta|O ponto de extremidade de autenticação v2.0 agora dá suporte a [escopos de permissão que exigem consentimento do administrador](http://developer.microsoft.com/en-us/graph/docs/authorization/permission_scopes#permission-scope-details), por meio do [ponto de extremidade de consentimento de administração](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#admin-restricted-scopes).|
|Addition|v1.0 e beta|O ponto de extremidade de autenticação v2.0 agora dá suporte ao consentimento administrativo para todos os usuários de um locatário, por meio do [ponto de extremidade de consentimento de administração](https://azure.microsoft.com/en-us/documentation/articles/active-directory-v2-scopes/#admin-restricted-scopes).|

### <a name="invitation-apis"></a>APIs de convite

|**Alterar tipo**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Addition|Beta|Foi adicionada a propriedade invitedUserType ao tipo de entidade de convite, que define o tipo de usuário (**Convidado** ou **Membro**) que é convidado.|
|Deletion|Beta|Removeremos a propriedade invitedToGroups do tipo de entidade de convite em 11/11/2016. Isso significa que você não poderá mais adicionar um usuário convidado a um grupo usando essa API. Em vez disso, use a [API adicionar membro](https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/group_post_members) para adicionar um usuário a um grupo.|

## <a name="september-2016"></a>Setembro de 2016

### <a name="azure-ad-application-proxy"></a>Proxy de aplicativo do Azure AD

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|O as APIs de Proxy de Aplicativo do Azure AD agora estão disponíveis nos pontos de extremidade beta do Microsoft Graph.  Essas APIs permitem publicações seguras de aplicativos locais para usuários fora da rede corporativa que estejam usando o Azure AD como o plano de controle comum para acesso. Você pode usar as APIs publicadas para gravar os aplicativos que podem recuperar e atualizar diversos aspectos do proxy de aplicativo, como as configurações _conectores_, _connectorGroups_ e _onPremisesPublishing_ de um aplicativo.|

### <a name="drive"></a>Unidade

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|Foi adicionada a coleção _shared_ para permitir o acesso aos driveItems compartilhados pela URL shareId ou sharing.|
|Addition|Beta|Foi adicionada a função _search_ a uma unidade, o que permite pesquisar mais itens do que apenas aqueles que constam na pasta raiz da unidade.|


### <a name="driveitem"></a>DriveItem

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|Suporte adicional para _createUploadSession_, o que permite carregar arquivos com mais de 4 MB no OneDrive, no OneDrive for Business e em bibliotecas de documentos do SharePoint.|
|Addition|Beta|Foi adicionada a propriedade _sharepointIds_ ao driveItem que retorna identificadores de API do SharePoint tradicionais para driveItems armazenados no SharePoint.|
|Addition|Beta|Outras propriedades foram adicionadas ao _remoteItem_.|
|Addition|Beta|Foi adicionado o valor _quickXorHash_ aos arquivos no OneDrive for Business.|
|Addition|Beta|O escopo para _createSharingLink_ foi adicionado para permitir a criação de links compartilháveis da empresa ou links de compartilhamento anônimos.|

### <a name="extended-properties"></a>Propriedades estendidas

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0|As [propriedades estendidas](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/extended-properties-overview) agora são compatíveis com os seguintes recursos:message, mailFolder, event, calendar, contact, contactFolder, group event, group calendar, group post.|

### <a name="groups"></a>Grupos

Suporte adicionado para a associação de grupo dinâmico através de visualização pública API, incluindo as adições listados na tabela a seguir.

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|Foi adicionada a propriedade **membershipRule** que contém regras de controle das associações a esse grupo, se o grupo for um grupo dinâmico|
|Addition|Beta|Foi adicionada a propriedade **membershipRuleProcessingState** para controlar se o processamento de associação dinâmica está ativado ou pausado para esse grupo.|
|Addition|Beta|Defina a propriedade **groupTypes** para conter **"DynamicMembership"** a fim de ativar o recurso de grupos dinâmicos para esse grupo.|
|Addition|Beta|Foi adicionada a propriedade **preferredLanguage** para indicar o idioma de preferência para um grupo do Office 365.|
|Addition|Beta|Foi adicionada propriedade **theme** para especificar o tema da cor de um grupo do Office 365.|

### <a name="hybrid-deployment-support"></a>Suporte à implantação híbrida

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0|Os aplicativos podem usar a versão 1.0 das APIs de Email, Calendário e Contatos do Outlook para acessar caixas de correio locais em uma implantação híbrida com a Atualização Cumulativa 3 (CU3) do Exchange 2016. Veja mais detalhes sobre o suporte à API REST em [implantações híbridas](https://developer.microsoft.com/en-us/graph/docs/overview/hybrid_rest_support) específicas. **Observação:** Se você estiver usando os conjuntos da API na versão 1.0, agora é possível que seus aplicativos, incluindo aplicativos de produção, funcionem com caixas de correio locais que atendam a requisitos de implantação híbrida específicos. Esse recurso só está disponível na visualização.|

### <a name="identityriskevents"></a>IdentityRiskEvents

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Change|Beta|Como parte da alteração de esquema em que o tipo de duas propriedades de local está sendo substituído por um novo tipo complexo no ponto de extremidade identityRiskEvents, as seguintes propriedades são alteradas/adicionadas no ponto de extremidade identityRiskEvents:</br>**location**  alterado de Edm.String para ComplexType signInLocation.<br/>**previousLocation** alterado de Edm.String para ComplexType signInLocation.<br/>**signInLocation** novo ComplexType que contém as propriedades city, state, countryOrRegion e geoCoordinates.<br/>**geoCoordinates** novo ComplexType que contém as propriedades latitude e longitude.|

### <a name="invitation-manager"></a>Gerenciador de convites

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|As APIs do gerenciador de convites agora estão disponíveis nos pontos de extremidade do Microsoft Graph na versão Beta. Você pode usar as APIs do gerenciador de convites para que o gerenciador de convites crie um convite para adicionar um usuário externo à organização. Como parte do convite, você também pode optar por adicionar o usuário convidado a um grupo do Office 365. Para obter mais detalhes, veja [gerenciador de convite](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/invitation).|

### <a name="onedrive"></a>OneDrive

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0|Foi adicionado o método **CreateUploadSession** ao **driveItem**, que permite arquivos grandes e carregamentos retomáveis.|
|Addition|v1.0|Foram adicionadas as propriedades para rastrear as IDs do SharePoint em itens do SharePoint (**sharepointIds**) e uma propriedade para identificar pastas-raiz (**root**).|
|Addition|v1.0|Foi adicionado o conjunto-raiz **Shares**, que pode ser usado com shareIds ou links de compartilhamento para acessar itens compartilhados no OneDrive e no SharePoint. Retorna um novo tipo, sharedDriveItem.|
|Addition|v1.0|Foi adicionado o método**Invite** ao driveItem, que permite adicionar permissões a itens. |
|Addition|v1.0|Foi adicionado o método **Search** à unidade, que permite pesquisar itens na unidade e itens compartilhados. |
|Addition|v1.0|Foi adicionada a propriedade **processingMetadata** à propriedade quickXorHash do tipo complexo no tipo complexo hashes. |
|Addition|v1.0|Foi adicionada a propriedade **quickXorHash** ao tipo complexo hashes. |

### <a name="outlook-calendar"></a>Calendário do Outlook

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0|Foi adicionada a propriedade **onlineMeetingUrl** ao recurso [event](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/event).|
|Addition|Beta|Foi adicionada a ação [forward](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/event_forward) ao recurso event.|
|Addition|Beta|Foram adicionadas as propriedades ao recurso [calendar](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/calendar) para dar suporte ao compartilhamento de calendários: **canEdit**, **canShare**, **canViewPrivateItems**, **isShared**, **isShareWithMe** e **owner**.|

### <a name="outlook-mail"></a>Email do Outlook

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0|Foi adicionado o tipo complexo [mailboxSettings](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/mailboxsettings), que inclui as propriedades **automaticRepliesSetting**, **timeZone** e **language**.|
|Addition|v1.0|Foi adicionada a propriedade **mailboxSettings** ao recurso [user](http://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/user).|
|Addition|Beta|Foi adicionado o suporte para criar, listar, obter e excluir uma ou mais instâncias de [mencionar](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/mention) em uma mensagem. As menções dão suporte a chamadas para chamar a atenção dos outros usuários em uma mensagem.|
|Addition|Beta|Foi adicionado suporte para a ação [getMailTips](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/user_getmailtips) para obter Dicas de Email para destinatários específicos. Foram adicionados os seguintes recursos: automaticRepliesMailTips, mailTips, mailTipsError.|

### <a name="query-parameters"></a>Parâmetros de consulta

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Change|Beta|Os prefixos de parâmetros de consulta sem $ são suportados a partir de 26/09/16. O prefixo $ nos parâmetros de consulta é opcional. Para obter mais detalhes, confira [Suporte a parâmetros da consulta sem prefixos $ no post do blog do Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph).|

### <a name="sharepoint"></a>SharePoint

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|Acesso a sites do SharePoint e [listas por ID](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/list_get) ou [caminho/URL](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/baseitem_getbyurl)|
|Addition|Beta|Suporte para [listar, criar, obter e excluir instâncias de listItem](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/listitem).|

### <a name="users"></a>Usuários

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|Foi adicionada a propriedade somente leitura para **refreshTokensValidFromDateTime** para indicar quando os tokens de sessão e de atualização são válidos. Qualquer token emitido antes desse momento será inválido, e qualquer tentativa de usá-lo forçará uma nova entrada do usuário.|
|Addition|Beta|Foi adicionada a propriedade **showInAddressList** para você controlar se a lista de endereços global do Outlook deve conter este usuário.|
|Addition|Beta|Foi adicionada a ação de serviço **invalidateAllRefreshTokens** que invalida todos os tokens de sessão e de atualização do usuário emitidos para aplicativos, redefinindo a propriedade do usuário **refreshTokensValidFromDateTime** para a data e a hora atuais.|


### <a name="webhooks"></a>Webhooks

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|Os itens de raiz de unidade adicionados aos Webhooks como um recurso que está disponível para se inscrever.|

## <a name="august-2016"></a>Agosto de 2016

### <a name="contacts"></a>Contatos

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|Como parte da mudança do esquema onde algumas propriedades estão sendo removidas e conjuntos de correspondentes estão sendo adicionados ao ponto de extremidade de contatos, as seguintes propriedades foram adicionadas ao ponto de extremidade de contatos: _Websites Collection(ComplexType: Website)_,_Phones Collection (ComplexType: Phone)_, _PostalAddress Collection(ComplexType: PhysicalAddress)_. Para obter detalhes, veja a postagem de blog [Upcoming changes to Contacts and People APIs](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/) (Futuras alterações nas APIs de Contatos e Pessoas).|
|Deletion|Beta|Como parte da mudança do esquema onde algumas propriedades estão sendo removidas e conjuntos de correspondentes estão sendo adicionados ao ponto de extremidade de contatos, as seguintes propriedades foram removidas do ponto de extremidade de contatos: _BusinessHomePage_,_HomePhones_, _MobilePhone1_, _BusinessPhones_, _HomeAddress_, _BusinessAddress_, _OtherAddress_. Para obter detalhes, veja a postagem de blog [Upcoming changes to Contacts and People APIs](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/) (Futuras alterações nas APIs de Contatos e Pessoas).|

### <a name="excel-apis"></a>APIs do Excel

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0|Em geral, a API REST do Excel no Microsoft Graph está disponível. Agora, você pode criar integrações avançadas e profundas com pastas de trabalho do Excel no Office 365. Consulte o [Turbine seus aplicativos com a nova API REST do Excel no Microsoft Graph](http://dev.office.com/blogs/power-your-apps-with-the-new-excel-rest-api) na postagem do blog para obter mais detalhes.|

### <a name="people"></a>Pessoas

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Change|Beta|A propriedade _WebSite_ será renomeada como _WebSite_. Para obter detalhes, veja [Futuras Alterações nas APIs de Contatos e Pessoas](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/).|

### <a name="privileged-identity-management"></a>Privileged Identity Management

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|As APIs REST de Privileged Identity Management (PIM) agora estão disponíveis no ponto de extremidade beta do Microsoft Graph. O [Privileged Identity Management](https://azure.microsoft.com/en-us/documentation/articles/active-directory-privileged-identity-management-configure/) fornece ativação "just in time" para funções organizacionais privilegiadas do Azure AD, como Administrador Global, Administrador de Cobrança, etc. As APIs publicadas permitem que os desenvolvedores criem aplicativos que recuperem e atualizem as atribuições de funções privilegiadas e ativem usuários em funções. Para obter detalhes, veja [Microsoft Graph: APIs de Pré-Visualização do Azure AD Privileged Identity Management disponíveis na versão Beta](http://dev.office.com/blogs/microsoft-graph-azure-ad-privileged-identity-management-apis-beta) e o [Azure AD Privileged Identity Management](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/privilegedidentitymanagement_root).|

## <a name="july-2016"></a>Julho de 2016

### <a name="administrative-units"></a>Unidades administrativas

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|Introduziu a nova API de pré-visualização das Unidades Administrativas. As unidades administrativas permitem às organizações subdividir seu Azure Active Directory e delegar tarefas administrativas a essas subdivisões. As subdivisões podem representar regiões, departamentos, centros de custo etc. Agora, isso pode ser gerenciado por meio da API do Microsoft Graph.|

## <a name="june-2016"></a>Junho de 2016

### <a name="identityriskevents"></a>IdentityRiskEvents

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|Introduziu a nova API de visualização de IdentityRiskEvents. Essa API funciona em conjunto com o Azure Active Directory Identity Protection. É possível utilizá-la para consultar eventos de risco gerados pelo Identity Protection. Para obter mais detalhes, veja a [Introdução de uma nova API de visualização do Microsoft Graph: Postagem do blog ](http://dev.office.com/blogs/identityriskevents-api-preview)IdentityRiskEvents

### <a name="subscriptions"></a>Assinaturas

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|Os escopos somente aplicativo agora têm suporte para assinaturas de _email_ e _contatos_.|

## <a name="may-2016"></a>Maio de 2016

### <a name="calendar"></a>Calendário

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Breaking change|Beta|Alterações na API findMeetingTimes. Para saber mais, veja a postagem de blog para a [ atualização da API findMeetingTimes do Microsoft Graph](http://dev.office.com/microsoft-graph-findmeetingtimes-api-update). Essa alteração entrou em vigor em 19 de maio de 2016.

### <a name="contact"></a>Contato

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0|Foram adicionadas _extensions_, que correspondem a um tipo abstrato que dá suporte à extensão openTypeExtension de tipo aberto do OData v4.|

### <a name="directory"></a>Diretório

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Breaking change|Beta|_settingTemplateId_ foi renomeado como _templateId_. Essa alteração entrou em vigor a partir de 19 de maio de 2016.|

### <a name="event"></a>Event

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0|Foram adicionadas _extensions_, que correspondem a um tipo abstrato que dá suporte à extensão openTypeExtension de tipo aberto do OData v4.|

### <a name="eventmessages"></a>EventMessages

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0|_inferenceClassification_ e _extensions_ foram adicionados a _eventMessages_.|
|Addition|Beta|_responseRequested_ foi adicionado a _eventMessageRequest_.|

### <a name="messages"></a>Mensagens

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0|_inferenceClassification_ e _extensions_ foram adicionados a _messages_.|
|Addition|Beta|_wellknownname_ foi adicionado a _contactFolder_.|Alterações na API _findMeetingTimes_. Para saber mais, veja a postagem de blog [Microsoft Graph findMeetingTimes API update](http://dev.office.com/microsoft-graph-findmeetingtimes-api-update) (Atualização da API findMeetingTimes do Microsoft Graph). Essa alteração entrou em vigor a partir de 19 de maio de 2016.|

### <a name="post"></a>Postagem

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0|Foram adicionadas _extensions_, que correspondem a um tipo abstrato que dá suporte à extensão openTypeExtension de tipo aberto do OData v4.|

### <a name="user"></a>Usuário

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0|O tipo de recurso _inferenceClassification_ foi adicionado.|
|Addition|Beta|_timeZone_ foi adicionado a _mailboxsettings_.|
|Addition|Beta|A API _findMeetingTimes_ foi adicionada a _user_.|

## <a name="april-2016"></a>Abril de 2016

### <a name="general"></a>Geral

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0 e Beta|Obter suporte adicional para honrar a _Codificação de aceitação: gzip_.|
|Addition|v1.0|Foi adicionado suporte para o segmento de conversão no caminho de expansão. Por exemplo, 'https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event'.|
|Addition|Beta|Suporte adicional para solicitação de PATCH em relação a propriedades estruturais. Por exemplo: 'PATCH /me/mailboxSettings'.|
|Addition|Beta|O Azure Active Directory agora é usado como fallback para solicitações /beta/users/id/photo quando o Outlook não consegue atender à solicitação para casos como quando o usuário não tem nenhuma licença de caixa de correio ou o locatário não tem uma assinatura do Exchange Online. OBSERVAÇÃO: esse fallback está disponível para GET e PATCH.|
|Addition|Beta|Foi adicionado suporte para o segmento de conversão no caminho de expansão. Por exemplo, https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event’.|

### <a name="onedrive"></a>OneDrive

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Correção|v1.0|Corrigido o problema de solicitações createLink do OneDrive com falhas 500 e "Tipo de propriedade de extensão sem suporte".|

## <a name="march-2016"></a>Março de 2016

### <a name="calendar"></a>Calendário

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|As propriedades _singleValueExtendedProperties_ e _multiValueExtendedProperties_ foram adicionadas.|
|Addition|Beta|A propriedade _suggestionHint_ foi adicionada a _meetingTimeCandidate_.|
|Addition|Beta|A propriedade _locationUri_ foi adicionada a _location_.|
|Addition|Beta|_type_ e _postOfficeBox_ foram adicionadas a _physicalAddress_.|
|Change|Beta|_findMeetingTimes_ agora tem um novo parâmetro _ReturnSuggestionHint_.|
|Change|Beta|_findMeetingTimes_ agora retorna uma coleção de _meetingTimeCandidate_.|

### <a name="drive"></a>Unidade

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0 e beta|Foi adicionada a função _recent_ para listar um conjunto de itens usados recentemente pelo usuário conectado. Esta lista inclui itens que estão na unidade do usuário, assim como itens aos quais ele tem acesso por meio de outras unidades. Exemplo: GET /me/drive/recent.|
|Addition|v1.0 e beta|Foi adicionada a função _sharedWithMe_ para listar um conjunto de itens que são compartilhados com o usuário atual. Exemplo: GET /me/drive/sharedWithMe|

### <a name="driveitem"></a>DriveItem

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0 e beta|Foi adicionado o tipo _remoteItem_ para fornecer um link a um item em outra unidade.|
|Addition|v1.0 e beta|Foi adicionado o tipo _sharingInvitation_ para fornecer detalhes de qualquer convite de compartilhamento associado para essa permissão.|
|Addition|v1.0 e beta|Foi adicionada a função _delta_ para rastrear as alterações aos itens de uma unidade. Exemplo: GET /e/drive/items/{id-do-item}/delta|
|Addition|v1.0 e beta|Foi adicionada _copy_ para criar uma cópia de um _driveItem_ (incluindo todos os filhos) em um novo pai ou mãe com um novo nome. Exemplo: POST /me/drive/items/{item-id}/copy.|
|Addition|v1.0 e beta|Os atributos da instância _conflictBehavior_ agora se aplicam ao _driveItem_.|
|Addition|Beta|Foi adicionada a função _invite_ para enviar um convite de compartilhamento a um item existente. Um convite de compartilhamento cria um link de compartilhamento exclusivo e envia um email ao destinatário do convite que inclui o link de compartilhamento. Exemplo: POST /drive/items/{id-do-item}/invite

### <a name="event"></a>Event

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|Foram adicionados a nova propriedade _onlineMeetingUrl_ e o novo método _cancel_.|

### <a name="event-messages"></a>Mensagens de evento

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|Foram adicionadas as propriedades _startDateTime_, _endDateTime_, _location_, _type_, _recurrence_, _isOutOfDate_, _conversationIndex_, _unsubscribe_, _unsubscribeData_, _unsubscribeEnabled_ e _flag_ ao objeto _eventmessage_.|
|Addition|Beta|As propriedades _singleValueExtendedProperties_ e _multiValueExtendedProperties_ foram adicionadas.|
|Addition|Beta|O novo método _unsubscribe_ foi adicionado.|

### <a name="excel"></a>Excel

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|Estamos adicionando novas APIs REST do Excel que permitem a leitura e a modificação de dados em uma pasta de trabalho do Excel. Agora é possível criar aplicativos inteligentes que permitem que os usuários obtenham valor do conteúdo armazenado em uma pasta de trabalho do Excel, fornecendo informações aos dados. Aproveite o potencial analítico do Excel, crie tabelas e gráficos e extraia imagens do gráfico visualmente atraentes - tudo isso a partir do seu aplicativo. Para obter mais detalhes, veja [Trabalhando com o Excel no Microsoft Graph](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/resources/excel).|

### <a name="general"></a>Geral

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0 e beta|Melhorar mensagens de erro ao resolver tokens JWT (AAD) rejeitados e alias do locatário.|
|Addition|v1.0 e beta|A localização do ponto de extremidade do serviço de autorização agora é retornada no cabeçalho _www-authenticate_ quando uma solicitação é recebida com um token de portador vazio.|
|Addition|v1.0 e beta|A capacidade de filtrar na propriedade de id da entidade já está corrigida. Exemplo: GET https://graph.microsoft.com/v1.0/users?$filter=id+eq+'x'<br/>Antes, qualquer solicitação POST para ações de serviço e funções exigia a prefixação do nome da função ou ação com o prefixo microsoft.graph. Por exemplo: POST https://graph.microsoft.com/v1.0/me/Microsoft.Graph.getMemberGroups<br/>Agora, o prefixo não é mais necessário (embora ele ainda possa ser especificado). Portanto, o seguinte também funcionará agora: POST https://graph.microsoft.com/v1.0/me/getMemberGroups|
|Change|Beta|Foram limpos os nomes de propriedades de assinatura.|
|Addition|Beta|Adicionamos a capacidade de descobrir (por meio de _directorySettingTemplates_) e substituir o comportamento padrão (criando uma _configuração_ do modelo) para entidades e suas funcionalidades associadas. Inicialmente, esse único modelo fornecido serve para controlar comportamentos de grupos do Office.|

### <a name="mail-folder"></a>Pasta Email

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|As propriedades _wellKnownName_ e _userConfigurations_ foram adicionadas.|
|Addition|Beta| As propriedades _singleValueExtendedProperties_ e _multiValueExtendedProperties_ foram adicionadas|

### <a name="messages"></a>Mensagens

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0|A propriedade _mobilePhone_ foi adicionada.|
|Addition|v1.0 e beta|A propriedade _internetMessageId_ foi adicionada. A ID da mensagem no formato especificado por [RFC2822](http://www.ietf.org/rfc/rfc2822.txt).|
|Change|Beta|A propriedade _mobilePhone1_ foi renomeada para _mobilePhone_.|
|Change|Beta|_createReply_ e _createReplyAll_ adotaram um novo parâmetro _Message_ e _comment_.|
|Change|Beta|_createForward_ adotou um novo parâmetro _Message_, _ToRecipients_ e _comment_.|
|Change|Beta|_reply_, _replyAll_ e _forward_ adotaram um novo parâmetro _Message_.|

### <a name="permission"></a>Permissão

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0 e beta|Foi adicionada a propriedade _sharingInvitation_ para fornecer detalhes sobre qualquer convite de compartilhamento associado para essa permissão.|

### <a name="person"></a>Pessoa

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|Foram adicionadas as novas propriedades _birthday_, _personNotes_, _isFavorite_, _phones_, _permission_, _postalAddresses_,_websites_,_yomiCompany_, _department_, _profession_, _mailboxType_ e _personType_.|
|Addition|Beta|Foram adicionados os novos tipos de enumeração _physicalAddressType_, _webSite_, _phone_ e _webSiteType_.|

### <a name="reference-attachment"></a>Anexo de referência

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|Foram adicionadas as novas propriedades _sourceUrl_, _providerType_, _thumbnailUrl_, _previewUrl_, _permission_ e _isFolder_.|
|Addition|Beta|As propriedades _singleValueExtendedProperties_ e _multiValueExtendedProperties_ foram adicionadas.|
|Addition|Beta|Foram adicionados os novos tipos enumeração _referenceAttachmentProvider_ e _referenceAttachmentPermission_.|

### <a name="subscriptions"></a>Assinaturas

|**Alterar tipo**|**Ponto de extremidade**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0|Os webhooks agora são GA no ponto de extremidade da versão 1.0 por meio do recurso _/Subscriptions_. Crie, Leia, Renove e Exclua assinaturas para receber notificações sobre dados do Outlook e de conversas de grupo do Office 365.|

### <a name="user"></a>Usuário

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|Foi adicionada a propriedade _mailboxSettings_ e os tipos correspondentes.|

## <a name="february-2016"></a>fevereiro de 2016

### <a name="driveitem"></a>DriveItem

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0 e beta|Nova propriedade _remoteItem_ em driveItem para contas da Microsoft.|

### <a name="general"></a>Geral

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Change|v1.0 e beta|-_/me/drive_ agora funciona tanto para contas da Microsoft como para contas corporativas e de estudante.|
|Change|v1.0 e beta|As solicitações de unidade para contas cujo armazenamento do OneDrive foi provisionado sob trabalho de demanda funcionam de forma mais confiável e em mais cenários onde os sites padrão do SharePoint do locatário usam nomes não padrão.|
|Deletion|Beta|Diversos tipos não implementados do esquema beta foram removidos para obter uma melhor correspondência com o esquema 1.0.|

### <a name="subscriptions"></a>Assinaturas

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|validação de notificationUrl na criação da assinatura. Para obter detalhes, veja [Microsoft Graph WebHooks Update - janeiro de 2016](http://dev.office.com/blogs/Microsoft-Graph-WebHooks-Update-January-2016).|
|Addition|Beta|Agora, as entidades de assinatura podem ser excluídas: EXCLUIR https://graph.microsoft.com/beta/subscriptions/|

### <a name="users"></a>Usuários

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Change|v1.0 e beta|_displayName_ agora é retornado para contas da Microsoft.|

## <a name="january-2016"></a>janeiro de 2016

### <a name="contacts"></a>Contatos

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|v1.0|Foi adicionada a propriedade mobilePhone ao conjunto de entidades personal contact.|

### <a name="directoryobjects"></a>directoryObjects

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Correção|v1.0 e beta|As ações de chamada vinculadas a directoryObjects foram corrigidas, pois apresentavam os seguintes erros:  O tipo de retorno da operação não é compatível com o conjunto de entidades fornecido. Isso se aplica às seguintes ações: _microsoft.graph.checkMemberObjects_, _microsoft.graph.getMemberObjects_, _microsoft.graph.checkMemberGroups_, _microsoft.graph.assignLicense_, _microsoft.graph.changePassword_.|

## <a name="december-2015"></a>dezembro de 2015

### <a name="contacts"></a>Contatos

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|Foi adicionada a propriedade mobilePhone ao conjunto de entidades personal contact.|

### <a name="general"></a>Geral

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Correção|v1.0 e beta|Foram corrigidas solicitações usando as expressões $filter que especificavam a mesma propriedade mais de uma vez, que estavam falhando com o seguinte erro 500: um item com a mesma chave já foi adicionado.|
|Correção|v1.0 e beta|Foi corrigida a falta de sensibilidade a maiúsculas e minúsculas para valores e nomes de parâmetros de ação.|
|Correção|v1.0 e beta|Foi corrigido o processamento de solicitações para cargas que contêm valores nulos para algumas propriedades complexas inseridos, que estavam falhando com uma exceção de referência nula.|
|Addition|v1.0 e beta|Suporte adicional para a classificação e filtragem de propriedades de tipo complexas.|
|Addition|v1.0 e beta|A propriedade authorization_uri foi adicionada ao cabeçalho www-authenticate em uma resposta 401. Esse uri pode ser usado para iniciar o fluxo de aquisição do token.|
|Addition|v1.0 e beta|Mensagens de erro aprimoradas em usuários e grupos.|

### <a name="groups"></a>Grupos

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Correção|v1.0 e beta|Corrigiu-se a chamada às seguintes ações de grupo: _microsoft.graph.addFavorite_, _microsoft.graph.removeFavorite_ e _microsoft.graph.resetUnseenCount_.|

### <a name="messages"></a>Mensagens

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Addition|Beta|Foi adicionado o subtipo eventMessageRequest das propriedades eventMessage estartDateTime, endDateTime, location, type, recurrence e isOutOfDate ao tipo eventMessage.|

### <a name="users"></a>Usuários

|**Alterar tipo**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Correção|v1.0 e beta|Corrigiu a possibilidade de selecionar determinadas propriedades de usuário em outros usuários ao referenciar o usuário pelo nome UPN. Por exemplo: https://graph.microsoft.com/v1.0/users/anotherUser@contoso.com?$select=aboutMe|
|Correção|v1.0 e beta|Foi corrigida a chamada à função de limite do usuário _microsoft.graph.reminderView_, pois estava falhando com o seguinte erro: Não foi possível localizar uma propriedade chamada businessPhones no tipo 'Microsoft.OutlookServices.Reminder.|
|Correção|v1.0 e beta|Foram corrigidas a criação e a atualização de usuário (POST/PATCH /v1.0/users), que estava falhando com um erro 400.|
