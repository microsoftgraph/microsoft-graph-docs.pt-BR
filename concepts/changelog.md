# <a name="changelog-for-microsoft-graph"></a>Log de mudanças do Microsoft Graph

Esse log de mudanças cobre o que foi alterado no Microsoft Graph, incluindo as APIs do Microsoft Graph para pontos de extremidade v1.0 e beta.  

Confira os detalhes sobre problemas conhecidos com as APIs do Microsoft Graph em [problemas conhecidos](known_issues.md).

## <a name="november-2017"></a>Novembro de 2017

### <a name="webhooks"></a>Webhooks

| Tipo de alteração | Versão | Descrição                              |
|:------------|:--------|:-----------------------------------------|
| Alteração significativa | Beta e V1.0 | [Webhooks](../api-reference/v1.0/resources/webhooks.md) [reduzidos ao comprimento máximo do tempo de expiração da assinatura ](../api-reference/v1.0/resources/subscription.md#maximum-length-of-subscription-per-resource-type) para itens raiz da unidade. O novo valor é o tempo de expiração máximo suportado para itens raiz da unidade. | 

### <a name="reports-apis"></a>APIs de relatórios
| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Adição    | Beta    | Adicionado suporte JSON para as seguintes APIs:<br>[getEmailActivityUserDetail](../api-reference/beta/api/reportroot_getemailactivityuserdetail.md)<br>[getEmailActivityCounts](../api-reference/beta/api/reportroot_getemailactivitycounts.md)<br>[getEmailActivityUserCounts](../api-reference/beta/api/reportroot_getemailactivityusercounts.md)<br>[getEmailAppUsageUserDetail](../api-reference/beta/api/reportroot_getemailappusageuserdetail.md)<br>[getEmailAppUsageAppsUserCounts](../api-reference/beta/api/reportroot_getemailappusageappsusercounts.md)<br>[getEmailAppUsageUserCounts](../api-reference/beta/api/reportroot_getemailappusageusercounts.md)<br>[getEmailAppUsageVersionsUserCounts](../api-reference/beta/api/reportroot_getemailappusageversionsusercounts.md)<br>[getMailboxUsageDetail](../api-reference/beta/api/reportroot_getmailboxusagedetail.md)<br>[getMailboxUsageMailboxCounts](../api-reference/beta/api/reportroot_getmailboxusagemailboxcounts.md)<br>[getMailboxUsageQuotaStatusMailboxCounts](../api-reference/beta/api/reportroot_getmailboxusagequotastatusmailboxcounts.md)<br>[getMailboxUsageStorage](../api-reference/beta/api/reportroot_getmailboxusagestorage.md)<br>[getOffice365ActivationsUserDetail](../api-reference/beta/api/reportroot_getoffice365activationsuserdetail.md)<br>[getOffice365ActivationCounts](../api-reference/beta/api/reportroot_getoffice365activationcounts.md)<br>[getOffice365ActivationsUserCounts](../api-reference/beta/api/reportroot_getoffice365activationsusercounts.md)<br>[getOffice365ActiveUserDetail](../api-reference/beta/api/reportroot_getoffice365activeuserdetail.md)<br>[getOffice365ActiveUserCounts](../api-reference/beta/api/reportroot_getoffice365activeusercounts.md)<br>[getOffice365ServicesUserCounts](../api-reference/beta/api/reportroot_getoffice365servicesusercounts.md)<br>[getOffice365GroupsActivityDetail](../api-reference/beta/api/reportroot_getoffice365groupsactivitydetail.md)<br> [getOffice365GroupsActivityCounts](../api-reference/beta/api/reportroot_getoffice365groupsactivitycounts.md)<br>[getOffice365GroupsActivityGroupCounts](../api-reference/beta/api/reportroot_getoffice365groupsactivitygroupcounts.md)<br>[getOffice365GroupsActivityStorage](../api-reference/beta/api/reportroot_getoffice365groupsactivitystorage.md)<br>[getOffice365GroupsActivityFileCounts](../api-reference/beta/api/reportroot_getoffice365groupsactivityfilecounts.md)<br>[getOneDriveActivityUserDetail](../api-reference/beta/api/reportroot_getonedriveactivityuserdetail.md)<br>[getOneDriveActivityUserCounts](../api-reference/beta/api/reportroot_getonedriveactivityusercounts.md)<br>[getOneDriveActivityFileCounts](../api-reference/beta/api/reportroot_getonedriveactivityfilecounts.md)<br>[getOneDriveUsageAccountDetail](../api-reference/beta/api/reportroot_getonedriveusageaccountdetail.md)<br>[getOneDriveUsageAccountCounts](../api-reference/beta/api/reportroot_getonedriveusageaccountcounts.md)<br>[getOneDriveUsageFileCounts](../api-reference/beta/api/reportroot_getonedriveusagefilecounts.md)<br>[getOneDriveUsageStorage](../api-reference/beta/api/reportroot_getonedriveusagestorage.md)<br>[getSharePointActivityUserDetail](../api-reference/beta/api/reportroot_getsharepointactivityuserdetail.md)<br>[getSharePointActivityFileCounts](../api-reference/beta/api/reportroot_getsharepointactivityfilecounts.md)<br>[getSharePointActivityUserCounts](../api-reference/beta/api/reportroot_getsharepointactivityusercounts.md)<br>[getSharePointActivityPages](../api-reference/beta/api/reportroot_getsharepointactivitypages.md)<br>[getSharePointSiteUsageDetail](../api-reference/beta/api/reportroot_getsharepointsiteusagedetail.md)<br>[getSharePointSiteUsageFileCounts](../api-reference/beta/api/reportroot_getsharepointsiteusagefilecounts.md)<br>[getSharePointSiteUsageSiteCounts](../api-reference/beta/api/reportroot_getsharepointsiteusagesitecounts.md)<br>[getSharePointSiteUsageStorage](../api-reference/beta/api/reportroot_getsharepointsiteusagestorage.md)<br>[getSharePointSiteUsagePages](../api-reference/beta/api/reportroot_getsharepointsiteusagepages.md)<br>[getSkypeForBusinessActivityUserDetail](../api-reference/beta/api/reportroot_getskypeforbusinessactivityuserdetail.md)<br>[getSkypeForBusinessActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinessactivitycounts.md)<br>[getSkypeForBusinessActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessactivityusercounts.md)<br>[getSkypeForBusinessDeviceUsageUserDetail](../api-reference/beta/api/reportroot_getskypeforbusinessdeviceusageuserdetail.md)<br>[getSkypeForBusinessDeviceUsageDistributionUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessdeviceusagedistributionusercounts.md)<br>[getSkypeForBusinessDeviceUsageUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessdeviceusageusercounts.md)<br>[getSkypeForBusinessOrganizerActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinessorganizeractivitycounts.md)<br>[getSkypeForBusinessOrganizerActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessorganizeractivityusercounts.md)<br>[getSkypeForBusinessOrganizerActivityMinuteCounts](../api-reference/beta/api/reportroot_getskypeforbusinessorganizeractivityminutecounts.md)<br>[getSkypeForBusinessParticipantActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinessparticipantactivitycounts.md)<br>[getSkypeForBusinessParticipantActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessparticipantactivityusercounts.md)<br>[getSkypeForBusinessParticipantActivityMinuteCounts](../api-reference/beta/api/reportroot_getskypeforbusinessparticipantactivityminutecounts.md)<br>[getSkypeForBusinessPeerToPeerActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinesspeertopeeractivitycounts.md)<br>[getSkypeForBusinessPeerToPeerActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinesspeertopeeractivityusercounts.md)<br>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](../api-reference/beta/api/reportroot_getskypeforbusinesspeertopeeractivityminutecounts.md)<br>[getYammerActivityUserDetail](../api-reference/beta/api/reportroot_getyammeractivityuserdetail.md)<br>[getYammerActivityCounts](../api-reference/beta/api/reportroot_getyammeractivitycounts.md)<br>[getYammerActivityUserCounts](../api-reference/beta/api/reportroot_getyammeractivityusercounts.md)<br>[getYammerDeviceUsageUserDetail](../api-reference/beta/api/reportroot_getyammerdeviceusageuserdetail.md)<br>[getYammerDeviceUsageDistributionUserCounts](../api-reference/beta/api/reportroot_getyammerdeviceusagedistributionusercounts.md)<br>[getYammerDeviceUsageUserCounts](../api-reference/beta/api/reportroot_getyammerdeviceusageusercounts.md)<br>[getYammerGroupsActivityDetail](../api-reference/beta/api/reportroot_getyammergroupsactivitydetail.md)<br>[getYammerGroupsActivityGroupCounts](../api-reference/beta/api/reportroot_getyammergroupsactivitygroupcounts.md)<br>[getYammerGroupsActivityCounts](../api-reference/beta/api/reportroot_getyammergroupsactivitycounts.md). |

## <a name="october-2017"></a>Outubro de 2017

### <a name="azure-ad-apis"></a>APIs do Azure AD

| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
|Adição|Beta|Adição da entidade [identityProvider](../api-reference/beta/resources/identityprovider.md) e das operações [create](../api-reference/beta/api/identityprovider_post_identityproviders.md), [list](../api-reference/beta/api/identityprovider_list.md), [get](../api-reference/beta/api/identityprovider_get.md), [update](../api-reference/beta/api/identityprovider_update.md) e [delete](../api-reference/beta/api/identityprovider_delete.md).|


### <a name="microsoft-intune-apis"></a>APIs do Microsoft Intune
|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|Beta|Foram adicionadas novas entidades:<br/>[androidDeviceComplianceLocalActionLockDeviceWithPasscode](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androiddevicecompliancelocalactionlockdevicewithpasscode)<br/>[iosLobAppProvisioningConfigurationAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfigurationassignment)<br/>[iosVppEBookAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_books_iosvppebookassignment)<br/>[managedDeviceMobileAppConfigurationAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationassignment)<br/>[managedEBookAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_books_managedebookassignment)<br/>[managedMobileApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_managedmobileapp)<br/>[mobileAppAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileappassignment)<br/>[termsAndConditionsAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_companyterms_termsandconditionsassignment)<br/>[vppToken](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_onboarding_vpptoken)<br/>[windows10PFXImportCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10pfximportcertificateprofile)<br/>[windowsAssignedAccessProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsassignedaccessprofile)<br/>[windowsDomainJoinConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsdomainjoinconfiguration)<br/>|
|Adição|Beta|Foram adicionados novos tipos complexos:<br/>[iosLobAppAssignmentSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_ioslobappassignmentsettings)<br/>[iosSingleSignOnSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iossinglesignonsettings)<br/>[iosStoreAppAssignmentSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_iosstoreappassignmentsettings)<br/>[iosVppAppAssignmentSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_iosvppappassignmentsettings)<br/>[mobileAppAssignmentSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileappassignmentsettings)<br/>[proxiedDomain](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_proxieddomain)<br/>[windowsInformationProtectionProxiedDomainCollection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionproxieddomaincollection)<br/>[windowsStoreForBusinessAppAssignmentSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsstoreforbusinessappassignmentsettings)<br/>|
|Adição|Beta|A ação [assign](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_apps_mobileapp_assign.md) foi adicionada no [mobileApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) |
|Adição|Beta|Foi adicionada a ação [assign](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_apps_ioslobappprovisioningconfiguration_assign.md) a [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) |
|Adição|Beta|A ação [assign](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_apps_manageddevicemobileappconfiguration_assign.md) foi adicionada ao [managedDeviceMobileAppConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration) |
|Adição|Beta|A ação [assign](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_deviceconfig_devicecompliancepolicy_assign.md) foi adicionada ao [deviceCompliancePolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy) |
|Adição|Beta|A ação [assignedAccessMultiModeProfiles](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_deviceconfig_deviceconfiguration_assignedaccessmultimodeprofiles.md) foi adicionada ao [deviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) |
|Adição|Beta|A ação [syncLicenses](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_onboarding_vpptoken_synclicenses.md) foi adicionada ao [vppToken](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_onboarding_vpptoken) |
|Adição|Beta|A ação [targetApps](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_mam_managedapppolicy_targetapps.md) foi adicionada ao [managedAppPolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy) |
|Adição|Beta|A ação [targetApps](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_mam_managedappprotection_targetapps.md) foi adicionada ao [managedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_managedappprotection) |
|Adição|Beta|A ação a[targetApps](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_mam_targetedmanagedappconfiguration_targetapps.md) foi adicionada ao [targetedManagedAppConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) |
|Adição|Beta|A ação [assign](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_books_managedebook_assign.md) foi adicionada no [managedEBook](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_books_managedebook) |
|Exclusão|Beta|Foram removidas as seguintes entidades:<br/>**cloudPkiSubscription**<br/>|
|Exclusão|Beta|Foram removidos os seguintes tipos complexos:<br/>**cloudPkiAdministratorCredentials**<br/>**windowsNetworkIsolationCloudResource**<br/>**windowsNetworkIsolationCloudResourceCollection**<br/>**windowsNetworkIsolationIPRangeCollection**<br/>**windowsNetworkIsolationResourceCollection**<br/>|
|Alteração|Beta|A propriedade **gracePeriodInMinutes** foi adicionada à entidade [androidDeviceComplianceLocalActionBase](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androiddevicecompliancelocalactionbase)|
|Alteração|Beta|A propriedade **enableSplitTunneling** foi removida da entidade [androidForWorkVpnConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkvpnconfiguration)|
|Alteração|Beta|As propriedades **versionName** e **versionCode** foram adicionadas à entidade [androidLobApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_androidlobapp)|
|Alteração|Beta|As propriedades **minimumRequiredPatchVersion** e **minimumWarningPatchVersion** foram adicionadas à entidade [androidManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection)|
|Alteração|Beta|As propriedades **minimumRequiredPatchVersion** e **minimumWarningPatchVersion** foram adicionadas à entidade [defaultManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection)|
|Alteração|Beta|A propriedade **target** foi adicionada à entidade [deviceCompliancePolicyAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicyassignment)|
|Alteração|Beta|A propriedade **singleSignOnSettings** foi adicionada à entidade [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration)|
|Alteração|Beta|As propriedades **versionNumber** e **buildNumber** foram adicionadas à entidade [iosLobApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_ioslobapp)|
|Alteração|Beta|A propriedade **bundleId** foi adicionada à entidade [iosVppApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_iosvppapp) |
|Alteração|Beta|Foi adicionada a propriedade **preSharedKey** à entidade [iosWiFiConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswificonfiguration)|
|Alteração|Beta|As propriedades **versionName** e **versionCode** foram adicionadas à entidade [managedAndroidLobApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_managedandroidlobapp)|
|Alteração|Beta|A propriedade **periodBeforePinReset** foi adicionada à entidade [managedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_managedappprotection)|
|Alteração|Beta|As propriedades **subscriberCarrier**, **meid**, **totalStorageSpaceInBytes** e **freeStorageSpaceInBytes** foram adicionadas à entidade [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice)|
|Alteração|Beta|A propriedade **enrollmentType** foi removida da entidade [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice)|
|Alteração|Beta|As propriedades **versionNumber** e **buildNumber** foram adicionadas à entidade [managedIOSLobApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_managedioslobapp)|
|Alteração|Beta|A propriedade **displayVersion** foi adicionada à entidade [mobileAppInstallStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus)|
|Alteração|Beta|As propriedades **defaultDeviceEnrollmentRestrictions**, **defaultDeviceEnrollmentWindowsHelloForBusinessSettings** e **defaultDeviceEnrollmentLimit** foram removidas da entidade [organization](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_onboarding_organization)|
|Alteração|Beta|A propriedade **isAssigned** foi adicionada à entidade [targetedManagedAppConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration)|
|Alteração|Beta|A propriedade **isAssigned** foi adicionada à entidade [targetedManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappprotection)|
|Alteração|Beta|As propriedades **activeFirewallRequired**, **uacRequired**, **defenderEnabled**, **defenderVersion**, **signatureOutOfDate** e **rtpEnabled** foram adicionadas à entidade [windows10CompliancePolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10compliancepolicy)|
|Alteração|Beta|As propriedades **assignedAccessSingleModeUserName**, **assignedAccessSingleModeAppUserModelId**, **microsoftAccountSignInAssistantSettings**, **authenticationAllowSecondaryDevice**, **cryptographyAllowFipsAlgorithmPolicy**, **securityBlockAzureADJoinedDevicesAutoEncryption**, **systemTelemetryProxyServer**, **inkWorkspaceAccess**, **inkWorkspaceBlockSuggestedApps**, **defenderCloudBlockLevel** e **defenderCloudExtendedTimeout** foram adicionadas à entidade [windows10GeneralConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration)|
|Alteração|Beta|As propriedades **protectedApps**, **enterpriseProxiedDomains** e **isAssigned** foram adicionadas à entidade [windowsInformationProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection)|
|Alteração|Beta|A propriedade **productVersion** foi adicionada à entidade [windowsMobileMSI](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi)|
|Alteração|Beta|A propriedade de navegação **apps** foi adicionada à entidade [androidManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection)|
|Alteração|Beta|A propriedade de navegação **apps** foi adicionada à entidade [defaultManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection)|
|Alteração|Beta|A propriedade de navegação **vppTokens** foi adicionada à entidade [deviceAppManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement)|
|Alteração|Beta|A propriedade de navegação **assignments** foi adicionada à entidade [deviceCompliancePolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy)|
|Alteração|Beta|A propriedade de navegação **deviceCompliancePolicy** foi removida da entidade [deviceCompliancePolicyAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicyassignment)|
|Alteração|Beta|A propriedade de navegação **deviceCompliancePolicy** foi removida da entidade [deviceCompliancePolicyGroupAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicygroupassignment)|
|Alteração|Beta|A propriedade de navegação **identityCertificateForClientAuthentication** foi adicionada à entidade [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration)|
|Alteração|Beta|A propriedade de navegação **assignments** foi adicionada à entidade [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)|
|Alteração|Beta|A propriedade de navegação **apps** foi adicionada à entidade [iosManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection)|
|Alteração|Beta|A propriedade de navegação **assignments** foi adicionada à entidade [managedDeviceMobileAppConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration)|
|Alteração|Beta|A propriedade de navegação **assignments** foi adicionada à entidade [managedEBook](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_books_managedebook)|
|Alteração|Beta|A propriedade de navegação **assignments** foi adicionada à entidade [mobileApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileapp)|
|Alteração|Beta|A propriedade de navegação **apps** foi adicionada à entidade [targetedManagedAppConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration)|
|Alteração|Beta|A propriedade de navegação **assignments** foi adicionada à entidade [termsAndConditions](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_companyterms_termsandconditions)|
|Alteração|Beta|A propriedade de navegação **assignedAccessMultiModeProfiles** foi adicionada à entidade [windows10GeneralConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration)|
|Alteração|Beta|A propriedade de navegação **protectedAppLockerFiles** foi adicionada à entidade [windowsInformationProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection)|
|Alteração|Beta|As propriedades **port** e **forceTls** foram adicionadas ao tipo complexo [airPrintDestination](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_airprintdestination)|
|Alteração|Beta|O tipo das seguintes propriedades no tipo complexo [deviceCompliancePolicySettingState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate) foi alterado:<br/>**errorCode** de Int32 para Int64<br/>|
|Alteração|Beta|O tipo das seguintes propriedades no tipo complexo [deviceConfigurationSettingState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) foi alterado:<br/>**errorCode** de Int32 para Int64<br/>|
|Alteração|Beta|O tipo das seguintes propriedades no tipo complexo [windowsNetworkIsolationPolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsnetworkisolationpolicy) foi alterado:<br/>**enterpriseCloudResources** de [windowsNetworkIsolationCloudResourceCollection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsNetworkIsolationCloudResourceCollection.md) para a coleção [proxiedDomain](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_proxieddomain)<br/>**enterpriseInternalProxyServers** de [windowsNetworkIsolationResourceCollection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsNetworkIsolationResourceCollection.md) para a coleção String<br/>**enterpriseIPRanges** de [windowsNetworkIsolationIPRangeCollection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsNetworkIsolationIPRangeCollection.md) para a coleção [ipRange](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iprange)<br/>**enterpriseNetworkDomainNames** de [windowsNetworkIsolationResourceCollection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsNetworkIsolationResourceCollection.md) para a coleção String<br/>**enterpriseProxyServers** de [windowsNetworkIsolationResourceCollection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsNetworkIsolationResourceCollection.md) para a coleção String<br/>**neutralDomainResources** de [windowsNetworkIsolationResourceCollection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsNetworkIsolationResourceCollection.md) para a coleção String<br/>|

### <a name="microsoft-teams-apis"></a>APIs do Microsoft Teams

|Tipo de alteração|Versão|Descrição|
|:---|:---|:---|
|Adição|Beta|Uma nova entidade [team](../api-reference/beta/resources/team.md) foi adicionada.|
|Adição|Beta|As operações [create](../api-reference/beta/api/team_put_teams.md), [get](../api-reference/beta/api/team_get.md) e [update](../api-reference/beta/api/team_update.md) foram adicionadas à entidade [team](../api-reference/beta/resources/team.md).|

### <a name="outlook-messages"></a>Mensagens do Outlook

| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Alteração          | v1.0 e beta | Esse aprimoramento do comportamento recai sobre a obtenção de uma pasta de emails compartilhada ou do conteúdo das mensagens desta pasta quando um usuário compartilhar uma pasta de email com o usuário conectado ou delegar ou não sua caixa de correio ao usuário conectado. Nesses casos, um aplicativo poderá especificar a identificação desse usuário ou nome da entidade de segurança do usuário para [obter essa pasta de emails compartilhada](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/mailfolder_get) ou [obter as mensagens desse calendário compartilhado](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/user_list_messages), desde que o usuário conectado tenha fornecido permissões delegadas ao aplicativo. |


### <a name="outlook-user-choices"></a>Opções de usuário do Outlook

| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
|Adição | Beta | A propriedade **workingHours** foi adicionada a [mailboxSettings](../api-reference/beta/resources/mailboxsettings.md). Confira [tipo de recurso workingHours](../api-reference/beta/resources/workinghours.md) para saber mais sobre casos de uso com suporte.|
|Adição | Beta | Os seguintes tipos complexos foram adicionados: <br> [workingHours](../api-reference/beta/resources/workinghours.md) <br> [timeZoneBase](../api-reference/beta/resources/timezonebase.md) <br> [customTimeZone](../api-reference/beta/resources/customtimezone.md) <br> [standardTimeZoneOffset](../api-reference/beta/resources/standardtimezoneoffset.md) <br> [daylightTimeZoneOffset](../api-reference/beta/resources/daylighttimezoneoffset.md)|


### <a name="reports-apis"></a>APIs de relatórios
| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Alteração      | Beta    | Adição das APIs [getEmailActivityUserDetail](../api-reference/beta/api/reportroot_getemailactivityuserdetail.md), [getEmailActivityCounts](../api-reference/beta/api/reportroot_getemailactivitycounts.md) e [getEmailActivityUserCounts](../api-reference/beta/api/reportroot_getemailactivityusercounts.md). Essas substituíram a API EmailActivity. |
| Alteração      | Beta    | Adição das APIs [getEmailAppUsageUserDetail](../api-reference/beta/api/reportroot_getemailappusageuserdetail.md), [getEmailAppUsageAppsUserCounts](../api-reference/beta/api/reportroot_getemailappusageappsusercounts.md), [getEmailAppUsageUserCounts](../api-reference/beta/api/reportroot_getemailappusageusercounts.md) e [getEmailAppUsageVersionsUserCounts](../api-reference/beta/api/reportroot_getemailappusageversionsusercounts.md). Essas substituíram a API EmailAppUsage. |
| Alteração      | Beta    | As APIs [getMailboxUsageDetail](../api-reference/beta/api/reportroot_getmailboxusagedetail.md), [getMailboxUsageMailboxCounts](../api-reference/beta/api/reportroot_getmailboxusagemailboxcounts.md), [getMailboxUsageQuotaStatusMailboxCounts](../api-reference/beta/api/reportroot_getmailboxusagequotastatusmailboxcounts.md) e [getMailboxUsageStorage](../api-reference/beta/api/reportroot_getmailboxusagestorage.md) foram adicionadas. Elas substituíram a API MailboxUsage. |
| Alteração      | Beta    | Adição das APIs [getOffice365ActivationsUserDetail](../api-reference/beta/api/reportroot_getoffice365activationsuserdetail.md), [getOffice365ActivationCounts](../api-reference/beta/api/reportroot_getoffice365activationcounts.md) e [getOffice365ActivationsUserCounts](../api-reference/beta/api/reportroot_getoffice365activationsusercounts.md). Essas substituíram a API Office365Activations. |
| Alteração      | Beta    | Adição das APIs [getOffice365ActiveUserDetail](../api-reference/beta/api/reportroot_getoffice365activeuserdetail.md), [getOffice365ActiveUserCounts](../api-reference/beta/api/reportroot_getoffice365activeusercounts.md) e [getOffice365ServicesUserCounts](../api-reference/beta/api/reportroot_getoffice365servicesusercounts.md). Essas substituíram a API Office365ActiveUser. |
| Alteração      | Beta    | As APIs [getOffice365GroupsActivityDetail](../api-reference/beta/api/reportroot_getoffice365groupsactivitydetail.md), [getOffice365GroupsActivityCounts](../api-reference/beta/api/reportroot_getoffice365groupsactivitycounts.md),[getOffice365GroupsActivityGroupCounts](../api-reference/beta/api/reportroot_getoffice365groupsactivitygroupcounts.md), [getOffice365GroupsActivityStorage](../api-reference/beta/api/reportroot_getoffice365groupsactivitystorage.md) e [getOffice365GroupsActivityFileCounts](../api-reference/beta/api/reportroot_getoffice365groupsactivityfilecounts.md) foram adicionadas. Essas substituíram a API Office365GroupsActivity. |
| Alteração      | Beta    | Adição das APIs [getOneDriveActivityUserDetail](../api-reference/beta/api/reportroot_getonedriveactivityuserdetail.md), [getOneDriveActivityUserCounts](../api-reference/beta/api/reportroot_getonedriveactivityusercounts.md) e [getOneDriveActivityFileCounts](../api-reference/beta/api/reportroot_getonedriveactivityfilecounts.md). Essas substituíram a API OneDriveActivity. |
| Alteração      | Beta    | As APIs [getOneDriveUsageAccountDetail](../api-reference/beta/api/reportroot_getonedriveusageaccountdetail.md), [getOneDriveUsageAccountCounts](../api-reference/beta/api/reportroot_getonedriveusageaccountcounts.md), [getOneDriveUsageFileCounts](../api-reference/beta/api/reportroot_getonedriveusagefilecounts.md) e [getOneDriveUsageStorage](../api-reference/beta/api/reportroot_getonedriveusagestorage.md) foram adicionadas. Essas substituíram a API OneDriveUsage. |
| Alteração      | Beta    | Adição das APIs [getSharePointActivityUserDetail](../api-reference/beta/api/reportroot_getsharepointactivityuserdetail.md), [getSharePointActivityFileCounts](../api-reference/beta/api/reportroot_getsharepointactivityfilecounts.md), [getSharePointActivityUserCounts](../api-reference/beta/api/reportroot_getsharepointactivityusercounts.md) e [getSharePointActivityPages](../api-reference/beta/api/reportroot_getsharepointactivitypages.md). Essas substituíram a API SharePointActivity. |
| Alteração      | Beta    | As APIs [getSharePointSiteUsageDetail](../api-reference/beta/api/reportroot_getsharepointsiteusagedetail.md), [getSharePointSiteUsageFileCounts](../api-reference/beta/api/reportroot_getsharepointsiteusagefilecounts.md), [getSharePointSiteUsageSiteCounts](../api-reference/beta/api/reportroot_getsharepointsiteusagesitecounts.md), [getSharePointSiteUsageStorage](../api-reference/beta/api/reportroot_getsharepointsiteusagestorage.md) e [getSharePointSiteUsagePages](../api-reference/beta/api/reportroot_getsharepointsiteusagepages.md) foram adicionadas. Essas substituíram a API SharePointSiteUsage. |
| Alteração      | Beta    | Adição das APIs [getSkypeForBusinessActivityUserDetail](../api-reference/beta/api/reportroot_getskypeforbusinessactivityuserdetail.md), [getSkypeForBusinessActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinessactivitycounts.md) e [getSkypeForBusinessActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessactivityusercounts.md). Essas substituíram a API SfbActivity. |
| Alteração      | Beta    | Adição das APIs [getSkypeForBusinessDeviceUsageUserDetail](../api-reference/beta/api/reportroot_getskypeforbusinessdeviceusageuserdetail.md), [getSkypeForBusinessDeviceUsageDistributionUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessdeviceusagedistributionusercounts.md), e [getSkypeForBusinessDeviceUsageUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessdeviceusageusercounts.md). Essas substituíram a API SfbDeviceUsage. |
| Alteração      | Beta    | Adição das APIs [getSkypeForBusinessOrganizerActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinessorganizeractivitycounts.md), [getSkypeForBusinessOrganizerActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessorganizeractivityusercounts.md) e [getSkypeForBusinessOrganizerActivityMinuteCounts](../api-reference/beta/api/reportroot_getskypeforbusinessorganizeractivityminutecounts.md). Essas substituíram a API SfbOrganizerActivity. |
| Alteração      | Beta    | Adição das APIs [getSkypeForBusinessParticipantActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinessparticipantactivitycounts.md), [getSkypeForBusinessParticipantActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinessparticipantactivityusercounts.md) e [getSkypeForBusinessParticipantActivityMinuteCounts](../api-reference/beta/api/reportroot_getskypeforbusinessparticipantactivityminutecounts.md). Essas substituíram a API SfbParticipantActivity. |
| Alteração      | Beta    | Adição das APIs [getSkypeForBusinessPeerToPeerActivityCounts](../api-reference/beta/api/reportroot_getskypeforbusinesspeertopeeractivitycounts.md), [getSkypeForBusinessPeerToPeerActivityUserCounts](../api-reference/beta/api/reportroot_getskypeforbusinesspeertopeeractivityusercounts.md) e [getSkypeForBusinessPeerToPeerActivityMinuteCounts](../api-reference/beta/api/reportroot_getskypeforbusinesspeertopeeractivityminutecounts.md). Essas substituíram a API SfbP2PActivity. |
| Alteração      | Beta    | Adição das APIs [getYammerActivityUserDetail](../api-reference/beta/api/reportroot_getyammeractivityuserdetail.md), [getYammerActivityCounts](../api-reference/beta/api/reportroot_getyammeractivitycounts.md) e [getYammerActivityUserCounts](../api-reference/beta/api/reportroot_getyammeractivityusercounts.md). Essas substituíram a API YammerActivity. |
| Alteração      | Beta    | Adição das APIs [getYammerDeviceUsageUserDetail](../api-reference/beta/api/reportroot_getyammerdeviceusageuserdetail.md), [getYammerDeviceUsageDistributionUserCounts](../api-reference/beta/api/reportroot_getyammerdeviceusagedistributionusercounts.md) e [getYammerDeviceUsageUserCounts](../api-reference/beta/api/reportroot_getyammerdeviceusageusercounts.md). Essas substituíram a API YammerDeviceUsage. |
| Alteração      | Beta    | As APIs [getYammerGroupsActivityDetail](../api-reference/beta/api/reportroot_getyammergroupsactivitydetail.md), [getYammerGroupsActivityGroupCounts](../api-reference/beta/api/reportroot_getyammergroupsactivitygroupcounts.md) e [getYammerGroupsActivityCounts](../api-reference/beta/api/reportroot_getyammergroupsactivitycounts.md) foram adicionadas. Essas substituíram a API YammerGroupsActivity. |



## <a name="september-2017"></a>Setembro de 2017

### <a name="intune-apis"></a>APIs do Intune

| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Adição    | Beta    | Foram adicionadas novas entidades:<br/>[activeDirectoryWindowsAutopilotDeploymentProfile](../api-reference/beta/resources/intune_enrollment_activedirectorywindowsautopilotdeploymentprofile.md)<br/>[azureADWindowsAutopilotDeploymentProfile](../api-reference/beta/resources/intune_enrollment_azureadwindowsautopilotdeploymentprofile.md)<br/>[deviceEnrollmentConfiguration](../api-reference/beta/resources/intune_onboarding_deviceenrollmentconfiguration.md)<br/>[deviceEnrollmentLimitConfiguration](../api-reference/beta/resources/intune_onboarding_deviceenrollmentlimitconfiguration.md)<br/>[deviceEnrollmentPlatformRestrictionsConfiguration](../api-reference/beta/resources/intune_onboarding_deviceenrollmentplatformrestrictionsconfiguration.md)<br/>[deviceEnrollmentWindowsHelloForBusinessConfiguration](../api-reference/beta/resources/intune_onboarding_deviceenrollmentwindowshelloforbusinessconfiguration.md)<br/>[deviceManagementPartner](../api-reference/beta/resources/intune_onboarding_devicemanagementpartner.md)<br/>[enrollmentConfigurationAssignment](../api-reference/beta/resources/intune_onboarding_enrollmentconfigurationassignment.md)<br/>[windows10EnrollmentCompletionPageConfiguration](../api-reference/beta/resources/intune_onboarding_windows10enrollmentcompletionpageconfiguration.md)<br/>[windows10NetworkBoundaryConfiguration](../api-reference/beta/resources/intune_deviceconfig_windows10networkboundaryconfiguration.md)<br/>[windowsAutopilotDeploymentProfile](../api-reference/beta/resources/intune_enrollment_windowsautopilotdeploymentprofile.md)<br/>[windowsAutopilotDeviceIdentity](../api-reference/beta/resources/intune_enrollment_windowsautopilotdeviceidentity.md)<br/>[windowsAutopilotSettings](../api-reference/beta/resources/intune_enrollment_windowsautopilotsettings.md)<br/> |
| Adição    | Beta    | Foram adicionados novos tipos complexos:<br/>[adminConsent](../api-reference/beta/resources/intune_devices_adminconsent.md)<br/>[allDevicesAssignmentTarget](../api-reference/beta/resources/intune_onboarding_alldevicesassignmenttarget.md)<br/>[allLicensedUsersAssignmentTarget](../api-reference/beta/resources/intune_onboarding_alllicensedusersassignmenttarget.md)<br/>[deviceAndAppManagementAssignmentTarget](../api-reference/beta/resources/intune_onboarding_deviceandappmanagementassignmenttarget.md)<br/>[deviceEnrollmentPlatformRestriction](../api-reference/beta/resources/intune_onboarding_deviceenrollmentplatformrestriction.md)<br/>[deviceHealthAttestationState](../api-reference/beta/resources/intune_devices_devicehealthattestationstate.md)<br/>[exclusionGroupAssignmentTarget](../api-reference/beta/resources/intune_onboarding_exclusiongroupassignmenttarget.md)<br/>[groupAssignmentTarget](../api-reference/beta/resources/intune_onboarding_groupassignmenttarget.md)<br/>[outOfBoxExperienceSettings](../api-reference/beta/resources/intune_enrollment_outofboxexperiencesettings.md)<br/>[windowsFirewallNetworkProfile](../api-reference/beta/resources/intune_deviceconfig_windowsfirewallnetworkprofile.md)<br/>[windowsNetworkIsolationCloudResource](../api-reference/beta/resources/intune_deviceconfig_windowsnetworkisolationcloudresource.md)<br/>[windowsNetworkIsolationCloudResourceCollection](../api-reference/beta/resources/intune_deviceconfig_windowsnetworkisolationcloudresourcecollection.md)<br/>[windowsNetworkIsolationIPRangeCollection](../api-reference/beta/resources/intune_deviceconfig_windowsnetworkisolationiprangecollection.md)<br/>[windowsNetworkIsolationPolicy](../api-reference/beta/resources/intune_deviceconfig_windowsnetworkisolationpolicy.md)<br/>[windowsNetworkIsolationResourceCollection](../api-reference/beta/resources/intune_deviceconfig_windowsnetworkisolationresourcecollection.md)<br/> |
| Adição    | Beta    | Adição da ação [sync](../api-reference/beta/api/intune_enrollment_windowsautopilotsettings_sync.md) em [windowsAutopilotSettings](../api-reference/beta/resources/intune_enrollment_windowsautopilotsettings.md) |
| Adição    | Beta    | Adição da ação [assign](../api-reference/beta/api/intune_enrollment_windowsautopilotdeploymentprofile_assign.md) em [windowsAutopilotDeploymentProfile](../api-reference/beta/resources/intune_enrollment_windowsautopilotdeploymentprofile.md) |
| Adição    | Beta    | Adição da ação [localActions](../api-reference/beta/api/intune_deviceconfig_devicecompliancepolicy_localactions.md) em [deviceCompliancePolicy](../api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy.md) |
| Adição    | Beta    | Adição da ação [setPriority](../api-reference/beta/api/intune_onboarding_deviceenrollmentconfiguration_setpriority.md) em [deviceEnrollmentConfiguration](../api-reference/beta/resources/intune_onboarding_deviceenrollmentconfiguration.md) |
| Adição    | Beta    | Adição da ação [assign](../api-reference/beta/api/intune_onboarding_deviceenrollmentconfiguration_assign.md) em [deviceEnrollmentConfiguration](../api-reference/beta/resources/intune_onboarding_deviceenrollmentconfiguration.md) |
| Adição    | Beta    | Adição da ação uploadDepToken na coleção [depOnboardingSetting](../api-reference/beta/resources/intune_onboarding_deponboardingsetting.md) |
| Adição    | Beta    | Adição da ação syncWithAppleDeviceEnrollmentProgram action na coleção [depOnboardingSetting](../api-reference/beta/resources/intune_onboarding_deponboardingsetting.md) |
| Adição    | Beta    | Adição da ação updateMobileAppIdentifierDeployments em [managedAppProtection](../api-reference/beta/resources/intune_mam_managedappprotection.md) |
| Adição    | Beta    | Adição da ação assign em [targetedManagedAppProtection](../api-reference/beta/resources/intune_mam_targetedmanagedappprotection.md) |
| Adição    | Beta    | Adição da ação assign em [targetedManagedAppConfiguration](../api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration.md) |
| Adição    | Beta    | Adição da ação assign em [windowsInformationProtection](../api-reference/beta/resources/intune_mam_windowsinformationprotection.md) |
| Adição    | Beta    | Adição da função getEncryptionPublicKey na coleção [depOnboardingSetting](../api-reference/beta/resources/intune_onboarding_deponboardingsetting.md) |
| Alteração      | Beta    | Adição das propriedades **requireSafetyNetAttestationBasicIntegrity**, **requireSafetyNetAttestationCertifiedDevice**, **requireGooglePlayServices**, **requireUpToDateSecurityProviders**, **requireCompanyPortalAppIntegrity** e **conditionStatementId** à entidade [androidCompliancePolicy](../api-reference/beta/resources/intune_deviceconfig_androidcompliancepolicy.md) |
| Alteração      | Beta    | Adição das propriedades **requireAppVerify**, **requireSafetyNetAttestationBasicIntegrity**, **requireSafetyNetAttestationCertifiedDevice**, **requireGooglePlayServices**, **requireUpToDateSecurityProviders** e **requireCompanyPortalAppIntegrity** à entidade [androidForWorkCompliancePolicy](../api-reference/beta/resources/intune_deviceconfig_androidforworkcompliancepolicy.md) |
| Alteração      | Beta    | Adição das propriedades **blockCrossProfileCopyPaste** e **requireAppVerify** à entidade [androidForWorkGeneralDeviceConfiguration](../api-reference/beta/resources/intune_deviceconfig_androidforworkgeneraldeviceconfiguration.md) |
| Alteração      | Beta    | Adição das propriedades **kioskModeApps** e **requireAppVerify** à entidade [androidGeneralDeviceConfiguration](../api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) |
| Alteração      | Beta    | Remoção da propriedade **kioskModeManagedApps** da entidade [androidGeneralDeviceConfiguration](../api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration.md) |
| Alteração      | Beta    | Remoção das propriedades **cloudPkiProvider**, **createdDateTime**, **description**, **lastModifiedDateTime**, **displayName**, **syncStatus**, **lastSyncError**, **lastSyncDateTime**, **credentials**, **trustedRootCertificate** e **version** da entidade [cloudPkiSubscription](../api-reference/beta/resources/intune_deviceconfig_cloudpkisubscription.md) |
| Alteração      | Beta    | Remoção das propriedades **assignmentStatus**, **assignmentProgress** e **assignmentErrorMessage** da entidade [deviceConfiguration](../api-reference/beta/resources/intune_deviceconfig_deviceconfiguration.md) |
| Alteração      | Beta    | Adição da propriedade **adminConsent** à entidade [deviceManagement](../api-reference/beta/resources/intune_androidforwork_devicemanagement.md) |
| Alteração      | Beta    | Adição das propriedades **vppTokenOrganizationName**, **vppTokenAccountType** e **vppTokenAppleId** à entidade [iosVppApp](../api-reference/beta/resources/intune_apps_iosvppapp.md) |
| Alteração      | Beta    | Adição das propriedades **deviceEnrollmentType**, **wiFiMacAddress** e **deviceHealthAttestationState** à entidade [managedDevice](../api-reference/beta/resources/intune_deviceconfig_manageddevice.md) |
| Alteração      | Beta    | Adição da propriedade **legacyAppConfiguration** à entidade [managedDeviceMobileAppConfiguration](../api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration.md) |
| Alteração      | Beta    | Adição da propriedade **notApplicableCount** à entidade [managedDeviceMobileAppConfigurationDeviceSummary](../api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) |
| Alteração      | Beta    | Adição da propriedade **notApplicableCount** à entidade [managedDeviceMobileAppConfigurationUserSummary](../api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationusersummary.md) |
| Alteração      | Beta    | Adição das propriedades **firewallBlockStatefulFTP**, **firewallIdleTimeoutForSecurityAssociationInSeconds**, **firewallPreSharedKeyEncodingMethod**, **firewallIPSecExemptionsAllowNeighborDiscovery**, **firewallIPSecExemptionsAllowICMP**, **firewallIPSecExemptionsAllowRouterDiscovery**, **firewallIPSecExemptionsAllowDHCP**, **firewallCertificateRevocationListCheckMethod**, **firewallMergeKeyingModuleSettings**, **firewallPacketQueueingMethod**, **firewallProfileDomain**, **firewallProfilePublic**, **firewallProfilePrivate**, **defenderAttackSurfaceReductionExcludedPaths**, **defenderOfficeAppsOtherProcessInjectionType**, **defenderOfficeAppsExecutableContentCreationOrLaunchType**, **defenderOfficeAppsLaunchChildProcessType**, **defenderOfficeMacroCodeAllowWin32ImportsType**, **defenderScriptObfuscatedMacroCodeType**, **defenderScriptDownloadedPayloadExecutionType**, **defenderEmailContentExecutionType**, **defenderGuardMyFoldersType**, **defenderGuardedFoldersAllowedAppPaths**, **defenderAdditionalGuardedFolders**, **defenderNetworkProtectionType**, **defenderExploitProtectionXml**, **defenderExploitProtectionXmlFileName**, **defenderSecurityCenterBlockExploitProtectionOverride**, **appLockerApplicationControl**, **applicationGuardBlockClipboardSharing**, **applicationGuardAllowPrintToPDF**, **applicationGuardAllowPrintToXPS**, **applicationGuardAllowPrintToLocalPrinters**, **applicationGuardAllowPrintToNetworkPrinters** and **bitLockerDisableWarningForOtherDiskEncryption** à entidade [windows10EndpointProtectionConfiguration](../api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration.md) |
| Alteração      | Beta    | Adição das propriedades **displayAppListWithGdiDPIScalingTurnedOn**, **displayAppListWithGdiDPIScalingTurnedOff**, **messagingBlockSync**, **messagingBlockMMS** e **messagingBlockRichCommunicationServices** à entidade [windows10GeneralConfiguration](../api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration.md) |
| Alteração      | Beta    | Remoção da propriedade **bluetoothDeviceName** da entidade [windows10GeneralConfiguration](../api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration.md) |
| Alteração      | Beta    | Remoção das propriedades **deviceAccountBlockExchangeServices**, **deviceAccountEmailAddress**, **deviceAccountExchangeServerAddress**, **deviceAccountRequirePasswordRotation** and **deviceAccountSessionInitiationProtocolAddress** da entidade [windows10TeamGeneralConfiguration](../api-reference/beta/resources/intune_deviceconfig_windows10teamgeneralconfiguration.md) |
| Alteração      | Beta    | Adição da propriedade de navegação **localActions** à entidade [androidCompliancePolicy](../api-reference/beta/resources/intune_deviceconfig_androidcompliancepolicy.md) |
| Alteração      | Beta    | Adição das propriedades de navegação **windowsAutopilotSettings**, **windowsAutopilotDeviceIdentities**, **windowsAutopilotDeploymentProfiles**, **deviceEnrollmentConfigurations**, **deviceManagementPartners** e **depOnboardingSettings** à entidade [deviceManagement](../api-reference/beta/resources/intune_androidforwork_devicemanagement.md) |
| Alteração      | Beta    | Remoção da propriedade de navegação **cloudPkiSubscriptions** da entidade [deviceManagement](../api-reference/beta/resources/intune_androidforwork_devicemanagement.md) |
| Alteração      | Beta    | Adição da propriedade de navegação **assignments** à entidade [targetedManagedAppConfiguration](../api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration.md) |
| Alteração      | Beta    | Adição da propriedade de navegação **assignments** à entidade [targetedManagedAppProtection](../api-reference/beta/resources/intune_mam_targetedmanagedappprotection.md) |
| Alteração      | Beta    | Adição da propriedade de navegação **assignments** à entidade [windowsInformationProtection](../api-reference/beta/resources/intune_mam_windowsinformationprotection.md) |

### <a name="onedrive"></a>OneDrive

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Adição da propriedade **system** ao recurso [Drive][]. |
| Adição        | v1.0        | Adição da relação **list** ao recurso [Drive][]. |
| Adição        | v1.0        | Adição da relação **listItem** ao recurso [DriveItem][]. |
| Adição        | v1.0        | Adição das relações **list** e **listItem** ao recurso [SharedDriveItem][]. |
| Adição        | v1.0        | Foram adicionados novos tipos complexos: [FolderView][]  |
| Adição        | v1.0        | Adição da propriedade **view** ao tipo complexo [Folder][]. |
| Adição        | v1.0        | Adição da propriedade **driveType** ao tipo complexo [ItemReference][]. |
| Adição        | v1.0        | Adição das propriedades **audioBitsPerSample**, **audioChannels**, **audioFormat**, **audioSamplesPerSecond**, **fourCC** e **frameRate** ao tipo complexo [Video][]. |
| Adição        | beta        | Adição da propriedade **system** ao recurso [Drive][Drive-beta]. |
| Adição        | beta        | Adição da relação **activities** ao recurso [Drive][Drive-beta]. |
| Adição        | beta        | Adição da propriedade **publication** ao recurso [DriveItem][DriveItem-beta]. |
| Adição        | beta        | Adição das relações **activities** e **versions** ao recurso [DriveItem][DriveItem-beta]. |
| Adição        | beta        | Foram adicionadas novas entidades: [DriveItemVersion][DriveItemVersion-beta], [ItemActivity][ItemActivity-beta]. |
| Adição        | beta        | Foram adicionados novos tipos complexos: [CommentAction][CommentAction-beta], [CreateAction][CreateAction-beta], [DeleteAction][DeleteAction-beta], [EditAction][EditAction-beta], [ItemActionSet][ItemActionSet-beta], [ItemActivityTimeSet][ItemActivityTimeSet-beta], [MentionAction][MentionAction-beta], [MoveAction][MoveAction-beta], [PublicationFacet][PublicationFacet-beta], [RenameAction][RenameAction-beta], [RestoreAction][RestoreAction-beta], [ShareAction][ShareAction-beta] e [VersionAction][VersionAction-beta]. |
| Adição        | beta        | Adição da propriedade **driveType** ao tipo complexo [ItemReference][ItemReference-beta]. |
| Exclusão        | beta        | Remoção da propriedade **tenantId** do tipo complexo [SharepointIds][SharepointIds-beta]. |
| Adição        | v1.0        | Adição das propriedades **audioBitsPerSample**, **audioChannels**, **audioFormat**, **audioSamplesPerSecond**, **fourCC** e **frameRate** ao tipo complexo [Video][Video-beta]. |
| Adição        | beta        | Adição das ações [CheckIn][CheckIn-beta] e [CheckOut][CheckOut-beta] no recurso [DriveItem][DriveItem-beta]. |
| Adição        | beta        | Adição das propriedades **expirationDateTime**, **password**, **message** e **recipients** na ação [CreateLink][CreateLink-beta] em um recurso [DriveItem][DriveItem-beta]. |

[Drive]: ../api-reference/v1.0/resources/drive.md
[DriveItem]: ../api-reference/v1.0/resources/driveitem.md
[SharedDriveItem]: ../api-reference/v1.0/resources/shareddriveitem.md
[FolderView]: ../api-reference/v1.0/resources/folderview.md
[Folder]: ../api-reference/v1.0/resources/folder.md
[ItemReference]: ../api-reference/v1.0/resources/itemreference.md
[Video]: ../api-reference/v1.0/resources/video.md
[Drive-beta]: ../api-reference/beta/resources/drive.md
[DriveItem-beta]: ../api-reference/beta/resources/driveitem.md
[DriveItemVersion-beta]: ../api-reference/beta/resources/driveitemversion.md
[ItemActivity-beta]: ../api-reference/beta/resources/itemactivity.md
[CommentAction-beta]: ../api-reference/beta/resources/commentaction.md
[CreateAction-beta]: ../api-reference/beta/resources/createaction.md
[DeleteAction-beta]: ../api-reference/beta/resources/deleteaction.md
[EditAction-beta]: ../api-reference/beta/resources/editaction.md
[ItemActionSet-beta]: ../api-reference/beta/resources/itemactionset.md
[ItemActivityTimeSet-beta]: ../api-reference/beta/resources/itemactivitytimeset.md
[MentionAction-beta]: ../api-reference/beta/resources/mentionaction.md
[MoveAction-beta]: ../api-reference/beta/resources/moveaction.md
[PublicationFacet-beta]: ../api-reference/beta/resources/publicationfacet.md
[RenameAction-beta]: ../api-reference/beta/resources/renameaction.md
[RestoreAction-beta]: ../api-reference/beta/resources/restoreaction.md
[ShareAction-beta]: ../api-reference/beta/resources/shareaction.md
[VersionAction-beta]: ../api-reference/beta/resources/versionaction.md
[ItemReference-beta]: ../api-reference/beta/resources/itemreference.md
[SharepointIds-beta]: ../api-reference/beta/resources/sharepointids.md
[Video-beta]: ../api-reference/beta/resources/video.md
[CheckIn-beta]: ../api-reference/beta/api/driveitem_checkin.md
[CheckOut-beta]: ../api-reference/beta/api/driveitem_checkout.md
[CreateLink-beta]: ../api-reference/beta/api/driveitem_createlink.md


### <a name="outlook-calendar"></a>Calendário do Outlook

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | Beta          | Adição das funções [findRoomLists](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/user_findroomlists) e [findRooms](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/user_findrooms) à entidade [user](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/user). |
| Adição        | Beta          | Adição da propriedade **locations** à entidade [event](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/event) para dar suporte à organização de um evento em que os participantes podem participar de mais de um local. |
| Adição        | Beta          | Adicionada a propriedade **locationType** ao tipo complexo [location](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/location). |
| Adição        | Beta          | Adicionada as propriedades **uniqueId** e **uniqueIdType** ao tipo complexo [location](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/location). Atualmente, essas propriedades são apenas para uso interno. |
| Alteração          | v1.0 e beta | Esse aprimoramento do comportamento recai sobre a obtenção de um calendário compartilhado ou do conteúdo dos eventos deste calendário quando um usuário compartilhar um calendário com o usuário conectado ou delegar ou não sua caixa de correio ao usuário conectado. Nesses casos, um aplicativo poderá especificar a identificação desse usuário ou nome da entidade de segurança do usuário para [obter esse calendário compartilhado](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/calendar_get) ou [obter os eventos desse calendário compartilhado](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/user_list_events), desde que o usuário conectado tenha fornecido permissões delegadas ao aplicativo. |

### <a name="outlook-contacts"></a>Contatos do Outlook

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Alteração          | v1.0 e beta | Esse aprimoramento do comportamento recai sobre a obtenção de uma pasta de contatos compartilhada ou do conteúdo dos contatos desta pasta quando um usuário compartilhar uma pasta de contatos com o usuário conectado ou delegar ou não sua caixa de correio ao usuário conectado. Nesses casos, um aplicativo poderá especificar a identificação desse usuário ou nome da entidade de segurança do usuário para [obter essa pasta de contatos compartilhada](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/contactfolder_get) ou [obter os contatos dessa pasta compartilhada](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/user_list_contacts), desde que o usuário conectado tenha fornecido permissões delegadas ao aplicativo. |

### <a name="outlook-mail"></a>Email do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Adição da propriedade **internetMessageHeaders** à entidade [message](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/message). |
| Adição        | Beta        | Adição do tipo complexo [internetMessageHeader](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/internetmessageheader). |
| Adição        | Beta        | Adição da propriedade de navegação **messageRules** à entidade [mailFolder](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/mailfolder). **messageRules** é uma coleção das instâncias [messageRule](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/messagerule). |
| Adição        | Beta        | Adicionado a entidade [messageRule](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/messagerule) e os tipos complexos [messageRuleActions](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/messageruleactions), [messageRulePredicates](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/messagerulepredicates) e [sizeRange](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/sizerange). |
| Adição        | Beta        | Adicionadas as seguintes operações CRUD às regras de mensagem: [create](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/mailfolder_post_messagerules), [list](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/mailfolder_list_messagerules), [get](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/messagerule_get), [update](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/messagerule_update) e [delete](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/messagerule_delete). |


### <a name="outlook-user-choices"></a>Opções de usuário do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Adição da nova propriedade de navegação **masterCategories** à entidade [outlookUser](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/outlookuser). **masterCategories** é uma coleção de objetos [outlookCategory](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/outlookCategory). |
| Adição        | Beta        | Adição da entidade [outlookCategory](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/outlookCategory). |
| Adição        | Beta        | Adição das seguintes operações CRUD para [outlookCategory](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/outlookCategory): [create](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/outlookuser_post_mastercategories), [get](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/outlookcategory_get), [update](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/outlookcategory_update) e [delete](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/outlookcategory_delete). |
| Adição        | Beta        | Adicionada a nova função [supportedLanguages](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/outlookuser_supportedlanguages) à entidade [outlookUser](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/outlookuser). |
| Adição        | Beta        | Adição da nova função [supportedTimeZones](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/outlookuser_supportedtimezones) à entidade [outlookUser](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/outlookuser). |


### <a name="sharepoint-lists"></a>Listas do SharePoint

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Foram adicionadas novas entidades: [ColumnDefinition][], [ColumnLink][], [ContentType][], [List][], [ListItem][]. |
| Adição        | v1.0        | Adição das relações **columns**, **contentTypes**, **items** e **lists** ao recurso [Site][]. |
| Adição        | v1.0        | Foram adicionados novos tipos complexos: [BooleanColumn][], [CalculatedColumn][], [ChoiceColumn][], [ContentTypeInfo][], [ContentTypeOrder][], [CurrencyColumn][], [DateTimeColumn][], [DefaultColumnValue][], [ListInfo][], [LookupColumn][], [NumberColumn][], [PersonOrGroupColumn][], [SystemFacet][], [TextColumn][]. |
| Adição        | beta        | Foram adicionadas novas entidades: [BaseItemVersion][BaseItemVersion-beta], [ColumnLink][ColumnLink-beta], [ContentType][ContentType-beta], [ListItemVersion][ListItemVersion-beta], |
| Adição        | beta        | Adição das propriedades **columnGroup**, **currency**, **defaultValue** e **displayName** à [ColumnDefinition][ColumnDefinition-beta]. |
| Adição        | beta        | Adição das propriedades **displayName** e **system** ao recurso [List][List-beta]. |
| Adição        | beta        | Adição das relações **activities** e **contentTypes** ao recurso [List][List-beta]. |
| Adição        | beta        | Adição das propriedade **contentType** ao recurso [ListItem][ListItem-beta]. |
| Adição        | beta        | Adição das relações **activities** e **versions** ao recurso [ListItem][ListItem-beta]. |
| Adição        | beta        | Adição da relação **contentTypes** ao recurso [Site][Site-beta]. |
| Adição        | beta        | Adição da propriedade **outputType** ao tipo [BooleanColumn][BooleanColumn-beta]. |
| Adição        | beta        | Foram adicionados novos tipos complexos: [ContentTypeInfo][ContentTypeInfo-beta], [ContentTypeOrder][ContentTypeOrder-beta], [CurrencyColumn][CurrencyColumn-beta] e [SystemFacet][SystemFacet-beta]. |
| Adição        | beta        | Adição da propriedade **contentTypesEnabled** ao tipo complexo [ListInfo][ListInfo-beta]. |
| Adição        | beta        | Adição da propriedade **allowUnlimitedLength** no tipo complexo [LookupColumn][LookupColumn-beta]. |
| Alteração          | beta        | Renomeação da propriedade **allowMultipleValue** para **allowMultipleValues** no tipo complexo [LookupColumn][LookupColumn-beta]. |
| Alteração          | beta        | Renomeação da propriedade **chooseFrom** para **chooseFromType** no tipo complexo [PersonOrGroupColumn][PersonOrGroupColumn-beta]. |
| Exclusão        | beta        | Remoção da propriedade **locale** no tipo complexo [NumberColumn][NumberColumn-beta]. |
| Exclusão        | beta        | Remoção da propriedade **enforceUniqueValues** do tipo complexo [PersonOrGroupColumn][PersonOrGroupColumn-beta]. |

[BaseItemVersion-beta]: ../api-reference/beta/resources/baseitemversion.md
[BooleanColumn-beta]:  ../api-reference/beta/resources/booleanColumn.md
[BooleanColumn]: ../api-reference/v1.0/resources/booleancolumn.md
[CalculatedColumn]: ../api-reference/v1.0/resources/calculatedcolumn.md
[ChoiceColumn]: ../api-reference/v1.0/resources/choicecolumn.md
[ColumnDefinition-beta]: ../api-reference/beta/resources/columndefinition.md
[ColumnDefinition]: ../api-reference/v1.0/resources/columndefinition.md
[ColumnLink-beta]: ../api-reference/beta/resources/columnLink.md
[ColumnLink]: ../api-reference/v1.0/resources/columnLink.md
[ContentType-beta]: ../api-reference/beta/resources/contentType.md
[ContentType]: ../api-reference/v1.0/resources/contentType.md
[ContentTypeInfo-beta]: ../api-reference/beta/resources/contentTypeInfo.md
[ContentTypeInfo]: ../api-reference/v1.0/resources/contentTypeInfo.md
[ContentTypeOrder-beta]: ../api-reference/beta/resources/contentTypeOrder.md
[ContentTypeOrder]: ../api-reference/v1.0/resources/contentTypeOrder.md
[CurrencyColumn-beta]: ../api-reference/beta/resources/currencycolumn.md
[CurrencyColumn]: ../api-reference/v1.0/resources/currencycolumn.md
[DateTimeColumn]: ../api-reference/v1.0/resources/datetimecolumn.md
[DefaultColumnValue]: ../api-reference/v1.0/resources/defaultColumnValue.md
[List-beta]: ../api-reference/beta/resources/list.md
[List]: ../api-reference/v1.0/resources/list.md
[ListInfo-beta]: ../api-reference/beta/resources/listinfo.md
[ListInfo]: ../api-reference/v1.0/resources/listinfo.md
[ListItem-beta]: ../api-reference/beta/resources/listitem.md
[ListItem]: ../api-reference/v1.0/resources/listitem.md
[ListItemVersion-beta]: ../api-reference/beta/resources/listitemversion.md
[LookupColumn-beta]: ../api-reference/beta/resources/lookupColumn.md
[LookupColumn]: ../api-reference/v1.0/resources/lookupcolumn.md
[NumberColumn-beta]: ../api-reference/beta/resources/numberColumn.md
[NumberColumn]: ../api-reference/v1.0/resources/numbercolumn.md
[PersonOrGroupColumn-beta]: ../api-reference/beta/resources/personOrGroupColumn.md
[PersonOrGroupColumn]: ../api-reference/v1.0/resources/personorgroupcolumn.md
[Site-beta]: ../api-reference/beta/resources/site.md
[Site]: ../api-reference/v1.0/resources/site.md
[SystemFacet-beta]: ../api-reference/beta/resources/systemfacet.md
[SystemFacet]: ../api-reference/v1.0/resources/systemFacet.md
[TextColumn]: ../api-reference/v1.0/resources/textcolumn.md


### <a name="sharepoint-sites"></a>Sites do SharePoint

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | beta        | Adição das propriedades **dataLocationCode** e **root** ao tipo complexo [SiteCollection][SiteCollection-beta]. |

[SiteCollection-beta]: ../api-reference/beta/resources/sitecollection.md


## <a name="august-2017"></a>Agosto de 2017

### <a name="group-lifecycle-policy"></a>Política de ciclo de vida de grupo

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Adicionada a entidade [groupLifecyclePolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/grouplifecyclepolicy). |
| Adição        | Beta        | Adicionadas as seguintes APIs de política de ciclo de vida de grupo: [criar](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/grouplifecyclepolicy_post_grouplifecyclepolicies), [listar](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/grouplifecyclepolicy_list), [obter](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/grouplifecyclepolicy_get), [atualizar](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/grouplifecyclepolicy_update), [excluir](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/grouplifecyclepolicy_delete), [adicionar grupo](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/grouplifecyclepolicy_addgroup), [remover grupo](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/grouplifecyclepolicy_removegroup) e [renovar um grupo](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/grouplifecyclepolicy_renewgroup). |
| Adição        | Beta        | Adicionada a função [Listar groupLifecylePolicies](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/group_list_grouplifecyclepolicies.md) à entidade [grupo](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/group). |

### <a name="intune-apis"></a>APIs do Intune
| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Adição    | Beta    | Foi adicionada uma nova entidade:<br/>[windowsPrivacyDataAccessControlItem](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsprivacydataaccesscontrolitem)<br/> |
| Adição    | Beta    | Foram adicionados novos tipos complexos:<br/>[configurationManagerClientEnabledFeatures](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devices_configurationmanagerclientenabledfeatures)<br/>[windowsDefenderScanActionResult](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devices_windowsdefenderscanactionresult)<br/> |
| Adição    | Beta    | Foi adicionada a ação [windowsDefenderScan](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_devices_manageddevice_windowsdefenderscan.md) ao [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Adição    | Beta    | Foi adicionada a ação [windowsDefenderUpdateSignatures](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_devices_manageddevice_windowsdefenderupdatesignatures.md) ao [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Adição    | Beta    | Foi adicionada a ação [windowsPrivacyAccessControls](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_deviceconfig_deviceconfiguration_windowsprivacyaccesscontrols.md) ao [deviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) |
| Alteração      | Beta    | Foram adicionadas as propriedades **automaticallyUpdateApps** e **countryOrRegion** à entidade [appleVolumePurchaseProgramToken](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_applevolumepurchaseprogramtoken) |
| Alteração      | Beta    | Foi adicionada a propriedade **enableAuthenticationViaCompanyPortal** à entidade [depEnrollmentProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_corpenrollment_depenrollmentprofile) |
| Alteração      | Beta    | Adicionada a propriedade **notificationMessageCCList** à entidade [deviceComplianceActionItem](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceactionitem) |
| Alteração      | Beta    | Foi adicionada a propriedade **notApplicableCount** à entidade [deviceComplianceDeviceOverview](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview) |
| Alteração      | Beta    | Foi adicionada a propriedade **notApplicableCount** à entidade [deviceComplianceUserOverview](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview) |
| Alteração      | Beta    | Foi adicionada a propriedade **notApplicableCount** à entidade [deviceConfigurationDeviceOverview](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview) |
| Alteração      | Beta    | Foi adicionada a propriedade **notApplicableCount** à entidade [deviceConfigurationUserOverview](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview) |
| Alteração      | Beta    | Foi adicionada a propriedade **configurationManagerClientEnabledFeatures** à entidade [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Alteração      | Beta    | Foi removida a propriedade **intuneBrand** da entidade [organization](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_onboarding_organization) |
| Alteração      | Beta    | Foram adicionadas as propriedades **smartScreenEnableInShell**, **smartScreenBlockOverrideForFiles**, **applicationGuardEnabled**, **applicationGuardBlockFileTransfer**, **applicationGuardBlockNonEnterpriseContent**, **applicationGuardAllowPersistence** e **applicationGuardForceAuditing** à entidade [windows10EndpointProtectionConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration) |
| Alteração      | Beta    | Foram adicionadas as propriedades **searchBlockDiacritics**, **searchDisableAutoLanguageDetection**, **searchDisableIndexingEncryptedItems**, **searchEnableRemoteQueries**, **searchDisableUseLocation**, **searchDisableIndexerBackoff**, **searchDisableIndexingRemovableDrive**, **searchEnableAutomaticIndexSizeManangement**, **smartScreenEnableAppInstallControl** e **privacyAdvertisingId** à entidade [windows10GeneralConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) |
| Alteração      | Beta    | Foi removida a propriedade **settingsDeviceName** da entidade [windows10TeamGeneralConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10teamgeneralconfiguration) |
| Alteração      | Beta    | Foi removida a propriedade **restartMode** da entidade [windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **detectedApps** e **managedDevices** à entidade [deviceManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) |
| Alteração      | Beta    | Foi adicionada a propriedade de navegação **privacyAccessControls** à entidade [windows10GeneralConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) |
| Alteração      | Beta    | Foi adicionada a propriedade **secureByDefault** ao tipo complexo [deviceManagementSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings) |
| Alteração      | Beta    | Foi adicionada a propriedade **restartMode** ao tipo complexo [windowsUpdateScheduledInstall](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdatescheduledinstall) |

### <a name="onenote"></a>OneNote

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0 e Beta | Adicionou a propriedade de navegação [onenote](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/onenote) a **site**. |
| Adição        | Beta          | Adicionou os parâmetros de destino *siteCollectionId* e *siteId* para as operações de cópia. Por exemplo: [CopyNotebook](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/notebook_copynotebook). |

### <a name="people"></a>Pessoas 

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Adicionada a [API de Pessoas](../api-reference/v1.0/resources/person.md) à versão 1.0. Para detalhes sobre a API de Pessoas, confira [Obter informações relevantes sobre as pessoas](people_example.md). |

### <a name="user"></a>Usuário

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | beta        | Adicionada propriedade **employeeId** ao [usuário](../api-reference/beta/resources/user.md) |

## <a name="july-2017"></a>Julho de 2017

### <a name="group-settings"></a>Configurações de grupo

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Adicionado suporte para as configurações de grupo.<br/>Novos tipos de recurso: [groupSetting](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/groupsetting.md), [groupSettingTemplate](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/groupsettingtemplate.md), [settingValue](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/settingvalue.md) e [settingTemplateValue](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/settingtemplatevalue.md) |
| Alteração          | v1.0        | Adicionou a propriedade **classification** e a propriedade de navegação **settings** ao [group](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/group.md) |

### <a name="intune-apis"></a>APIs do Intune

| Change&nbsp;type | Versão | Descrição                              |
| :--------------- | :------ | :--------------------------------------- |
| Adição         | Beta    | Foi adicionada a ação [assign](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_apps_iosmobileappconfiguration_assign) a [iosMobileAppConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_iosmobileappconfiguration) |
| Adição         | Beta    | Foi adicionada a ação [syncDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_devices_manageddevice_syncdevice) ao [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Alteração           | Beta    | Foram adicionadas as propriedades **appsInstallAllowList**, **appsLaunchBlockList** e **appsHideList** à entidade [androidGeneralDeviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) |
| Alteração           | Beta    | Foi adicionada a propriedade **disableAppEncryptionIfDeviceEncryptionIsEnabled** à entidade [androidManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) |
| Alteração           | Beta    | Foi adicionada a propriedade **disableAppEncryptionIfDeviceEncryptionIsEnabled** à entidade [defaultManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) |
| Alteração           | Beta    | Foi adicionada a propriedade **complianceGracePeriodExpirationDateTime** à entidade [deviceComplianceDeviceStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedevicestatus) |
| Alteração           | Beta    | Foi adicionada a propriedade **complianceGracePeriodExpirationDateTime** à entidade [deviceComplianceSettingState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate) |
| Alteração           | Beta    | Foi adicionada a propriedade **complianceGracePeriodExpirationDateTime** à entidade [deviceConfigurationDeviceStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatus) |
| Alteração           | Beta    | Foi adicionada a propriedade **subscriptions** à entidade [deviceManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) |
| Alteração           | Beta    | Foi adicionada a propriedade **version** à entidade [deviceManagementExchangeConnector](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_onboarding_devicemanagementexchangeconnector) |
| Alteração           | Beta    | Foi adicionada a propriedade **utcTimeOffsetInMinutes** à entidade [iosUpdateConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdateconfiguration) |
| Alteração           | Beta    | Foi adicionada a propriedade **complianceGracePeriodExpirationDateTime** à entidade [iosUpdateDeviceStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdatedevicestatus) |
| Alteração           | Beta    | Foi adicionada a propriedade **preSharedKey** à entidade [macOSWiFiConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoswificonfiguration) |
| Alteração           | Beta    | Foram adicionadas as propriedades **phoneNumber**, **androidSecurityPatchLevel** e **userDisplayName** à entidade [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Alteração           | Beta    | Foram adicionadas as propriedades **userName**, **deviceModel**, **platform** e **complianceGracePeriodExpirationDateTime** à entidade [managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus) |
| Alteração           | Beta    | Foi adicionada a propriedade **userPrincipalName** à entidade [mobileAppInstallStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus) |
| Alteração           | Beta    | Foi adicionada a propriedade **overrideDefaultRule** à entidade [onPremisesConditionalAccessSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_onboarding_onpremisesconditionalaccesssettings) |
| Alteração           | Beta    | Foi adicionada a propriedade **userPrincipalName** à entidade [userAppInstallStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_userappinstallstatus) |
| Alteração           | Beta    | Foram adicionadas as propriedades **connectAppBlockAutoLaunch**, **deviceAccountBlockExchangeServices**, **deviceAccountEmailAddress**, **deviceAccountExchangeServerAddress**, **deviceAccountRequirePasswordRotation**, **deviceAccountSessionInitiationProtocolAddress**, **settingsBlockMyMeetingsAndFiles**, **settingsBlockSessionResume**, **settingsBlockSigninSuggestions**, **settingsDefaultVolume**, **settingsScreenTimeoutInMinutes**, **settingsSessionTimeoutInMinutes** e **settingsSleepTimeoutInMinutes** à entidade [windows10TeamGeneralConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10teamgeneralconfiguration) |
| Alteração           | Beta    | Foi adicionada a propriedade de navegação **deploymentSummary** à entidade [defaultManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) |
| Alteração           | Beta    | Foram adicionadas as propriedades **settingName**, **userId**, **userName**, **userEmail** e **currentValue** ao tipo complexo [deviceCompliancePolicySettingState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate) |
| Alteração           | Beta    | As propriedades **settingName**, **userId**, **userName**, **userEmail** e **currentValue** foram adicionadas ao tipo complexo [deviceConfigurationSettingState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) |
| Alteração           | Beta    | Foi adicionada a propriedade **unknownCount** ao tipo complexo [deviceOperatingSystemSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devices_deviceoperatingsystemsummary) |



## <a name="june-2017"></a>Junho de 2017

### <a name="project-rome"></a>Projeto Roma

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Adicionados os seguintes recursos e APIs:<br/>[Atividade](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/projectrome_activity)<br/>[Criar ou substituir uma atividade](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/projectrome_put_activity)<br/>[Excluir uma atividade](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/projectrome_delete_activity)<br/>[Item do histórico](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/projectrome_historyitem)<br/>[Criar ou substituir um item do histórico](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/projectrome_put_historyitem)<br/>[Excluir um item do histórico](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/projectrome_delete_historyitem) |

### <a name="outlook-calendar"></a>Calendário do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Foram promovidas as seguintes 4 propriedades de [calendar](https://graph.microsoft.io/pt-BR/docs/api-reference/v1.0/resources/calendar) para v1.0: **canEdit**, **canShare**, **canViewPrivateItems** e **owner**. |


### <a name="intune-apis"></a>APIs do Intune

| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Adição    | Beta    | Foram adicionadas novas entidades:<br/>[defaultDeviceCompliancePolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_defaultdevicecompliancepolicy)<br/>[deviceConfigurationUserStateSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuserstatesummary)<br/>[deviceManagementScriptDeviceState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptdevicestate)<br/>[deviceManagementScriptRunSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptrunsummary)<br/>[deviceManagementScriptUserState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscriptuserstate)<br/>[iosUpdateDeviceStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdatedevicestatus)<br/>[windowsManagedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanageddevice)<br/>[windowsManagementAppHealthState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapphealthstate)<br/>[windowsManagementAppHealthSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapphealthsummary)<br/> |
| Adição    | Beta    | Foram adicionados novos tipos complexos:<br/>[bitLockerFixedDrivePolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerfixeddrivepolicy)<br/>[bitLockerRecoveryOptions](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerrecoveryoptions)<br/>[bitLockerRemovableDrivePolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockerremovabledrivepolicy)<br/>[deleteUserFromSharedAppleDeviceActionResult](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devicefe_deleteuserfromsharedappledeviceactionresult)<br/>[iosNetworkUsageRule](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnetworkusagerule)<br/> |
| Exclusão    | Beta    | Foram removidas as seguintes entidades:<br/>**deviceManagementScriptState**<br/> |
| Exclusão    | Beta    | Foi removida a ação wipeByDeviceTag em [user](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devicefe_user) |
| Alteração      | Beta    | Foram adicionadas as propriedades **innerAuthenticationProtocolForEapTtls**, **innerAuthenticationProtocolForPeap** e **outerIdentityPrivacyTemporaryValue** à entidade [androidEnterpriseWiFiConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidenterprisewificonfiguration). |
| Alteração      | Beta    | Foram removidas as propriedades **nonEapAuthenticationMethodForEapTtls**, **nonEapAuthenticationMethodForPeap** e **enableOuterIdentityPrivacy** da entidade [androidEnterpriseWiFiConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidenterprisewificonfiguration). |
| Alteração      | Beta    | Foi adicionada a propriedade **deployedAppCount** à entidade [androidManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) |
| Alteração      | Beta    | Foram removidas as propriedades **instanceDisplayName** e **settingPlatform** da entidade [complianceSettingStateSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/complianceSettingStateSummary). |
| Alteração      | Beta    | Foi adicionada a propriedade **deployedAppCount** à entidade [defaultManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) |
| Alteração      | Beta    | Adicionada a propriedade **excludeGroup** à entidade [deviceCompliancePolicyGroupAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicygroupassignment) |
| Alteração      | Beta    | Foram removidas as propriedades **instanceDisplayName** e **settingPlatform** da entidade [deviceCompliancePolicySettingStateSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary) |
| Alteração      | Beta    | Foi removida a propriedade **devicePlatform** da entidade [deviceComplianceSettingState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate) |
| Alteração      | Beta    | Foram adicionadas as propriedades **assignmentStatus**, **assignmentProgress** e **assignmentErrorMessage** à entidade [deviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration)  |
| Alteração      | Beta    | Foi adicionada a propriedade **intuneBrand** à entidade [deviceManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) |
| Alteração      | Beta    | Foram adicionadas as propriedades **enforceSignatureCheck** e **fileName** à entidade [deviceManagementScript](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript) |
| Alteração      | Beta    | Foram adicionadas as propriedades **innerAuthenticationProtocolForEapTtls** e **outerIdentityPrivacyTemporaryValue** à entidade [iosEnterpriseWiFiConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosenterprisewificonfiguration) |
| Alteração      | Beta    | Foram removidas as propriedades **nonEapAuthenticationMethodForEapTtls** e **enableOuterIdentityPrivacy** da entidade [iosEnterpriseWiFiConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosenterprisewificonfiguration) |
| Alteração      | Beta    | Foram adicionadas as propriedades **classroomAppForceUnpromptedScreenObservation**, **keyboardBlockDictation**, **networkUsageRules** e **wiFiConnectOnlyToConfiguredNetworks** à entidade [iosGeneralDeviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration) |
| Alteração      | Beta    | Foi adicionada a propriedade **deployedAppCount** à entidade [iosManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) |
| Alteração      | Beta    | Foi adicionada a propriedade **preSharedKey** à entidade [iosWiFiConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswificonfiguration) |
| Alteração      | Beta    | Foram adicionadas as propriedades **innerAuthenticationProtocolForEapTtls** e **outerIdentityPrivacyTemporaryValue** à entidade [macOSEnterpriseWiFiConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosenterprisewificonfiguration) |
| Alteração      | Beta    | Foram removidas as propriedades **nonEapAuthenticationMethodForEapTtls** e **enableOuterIdentityPrivacy** da entidade [macOSEnterpriseWiFiConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosenterprisewificonfiguration) |
| Alteração      | Beta    | Foram removidas as entidades **lastModifiedTime** e **deployedAppCount** da entidade [managedAppPolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy) |
| Alteração      | Beta    | Foi adicionada a propriedade **serialNumber** à entidade [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Alteração      | Beta    | Foi removida a propriedade **managementAgents** da entidade [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Alteração      | Beta    | Foi adicionada a propriedade **deployedAppCount** à entidade [targetedManagedAppConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) |
| Alteração      | Beta    | Foram adicionadas as propriedades **bitLockerFixedDrivePolicy** e **bitLockerRemovableDrivePolicy** à entidade [windows10EndpointProtectionConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration) |
| Alteração      | Beta    | Foram adicionadas as propriedades **enterpriseCloudPrintDiscoveryEndPoint**, **enterpriseCloudPrintOAuthAuthority**, **enterpriseCloudPrintOAuthClientIdentifier**, **enterpriseCloudPrintResourceIdentifier**, **enterpriseCloudPrintDiscoveryMaxLimit**, **enterpriseCloudPrintMopriaDiscoveryResourceIdentifier**, **edgeBlockAddressBarDropdown**, **edgeBlockCompatibilityList**, **edgeClearBrowsingDataOnExit**, **edgeAllowStartPagesModification**, **edgeDisableFirstRunPage**, **edgeBlockLiveTileDataCollection** e **edgeSyncFavoritesWithInternetExplorer** à entidade [windows10GeneralConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) |
| Alteração      | Beta    | Foi adicionada a propriedade **availableVersion** à entidade [windowsManagementApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp) |
| Alteração      | Beta    | Foram removidas as propriedades **onboardingStatus**, **deployedVersion** e **lastModifiedTime** da entidade [windowsManagementApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp) |
| Alteração      | Beta    | Foi adicionada a propriedade **packageIdentityName** à entidade [windowsStoreForBusinessApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsstoreforbusinessapp) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **mobileAppIdentifierDeployments** e **deploymentSummary** à entidade [androidManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) |
| Alteração      | Beta    | Foi adicionada a propriedade de navegação **mobileAppIdentifierDeployments** à entidade [defaultManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **deviceConfigurationUserStateSummaries** e **iosUpdateStatuses** à entidade [deviceManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) |
| Alteração      | Beta    | Foi removida a propriedade de navegação **complianceSettingStateSummaries** da entidade [deviceManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **runSummary**, **deviceRunStates** e **userRunStates** à entidade [deviceManagementScript](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript) |
| Alteração      | Beta    | Foi removida a propriedade de navegação **runStates** da entidade [deviceManagementScript](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devicefe_devicemanagementscript) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **mobileAppIdentifierDeployments** e **deploymentSummary** à entidade [iosManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) |
| Alteração      | Beta    | Foram removidas as propriedades de navegação **mobileAppIdentifierDeployments** e **deploymentSummary** da entidade [managedAppPolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **mobileAppIdentifierDeployments** e **deploymentSummary** à entidade [targetedManagedAppConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **healthSummary** e **healthStates** à entidade [windowsManagementApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devicefe_windowsmanagementapp) |
| Alteração      | Beta    | Foram adicionadas as propriedades **applicationId**, **appName**, **platformId**, **userFailures** e **deviceFailures** ao tipo complexo [appInstallationFailure](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure) |
| Alteração      | Beta    | Foram adicionadas as propriedades **encryptionMethod**, **startupAuthenticationRequired**, **startupAuthenticationBlockWithoutTpmChip**, **startupAuthenticationTpmUsage**, **startupAuthenticationTpmPinUsage**, **startupAuthenticationTpmKeyUsage**, **startupAuthenticationTpmPinAndKeyUsage**, **recoveryOptions** e **prebootRecoveryEnableMessageAndUrl** ao tipo complexo [bitLockerSystemDrivePolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockersystemdrivepolicy) |
| Alteração      | Beta    | Foram removidas as propriedades **settingName**, **userId**, **userName**, **userEmail** e **currentValue** do tipo complexo [deviceCompliancePolicySettingState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate) |
| Alteração      | Beta    | Foram removidas as propriedades **settingName**, **userId**, **userName**, **userEmail** e **currentValue** do tipo complexo [deviceConfigurationSettingState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) |
| Alteração      | Beta    | Foram adicionadas as propriedades **windowsCommercialId** e **windowsCommercialIdLastModifiedTime** ao tipo complexo [deviceManagementSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings) |
| Alteração      | Beta    | Foi adicionada a propriedade **address** ao tipo complexo [vpnServer](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_vpnserver) |


## <a name="may-2017"></a>Maio de 2017

### <a name="application-api-changes"></a>Alterações da API do aplicativo

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | Atualização da API do aplicativo. Este é o primeiro conjunto de alterações incluindo renomeação de propriedade e restruturação da entidade [application](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/application).<br/>**Novas entidades:** [api](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/api]), [informationalUrl](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/informationalUrl), [installedClient](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/installedclient), [permissionScope](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/permissionscope), [preauthorizedApplication](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/preauthorizedapplication) e [web](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/web).<br/>**Propriedades removidas:** addIns, appRoles, availableToOtherOrganizations, knownClientApplications, oauth2AllowUrlPathMatching e recordConsentConditions.<br/>**Propriedades renomeadas:** appId agora é id, identifierUris agora é applicationAliases, availableToOtherTenants agora é orgRestrictions, mainLogo agora é logo, oauth2Permissions agora é publishedPermissionsScopes, publicClient agora é allowPublicClient e replyUrls agora é redirectUrls.<br/>**Novas propriedades:** tags. |

### <a name="remove-deprecated-planner-api"></a>Remover a API do Planner descontinuada
| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Exclusão        | Beta        | Foram removidas as seguintes entidades:<br/>**task**<br/>**plan**<br/>**bucket**<br/>**taskDetails**<br/>**planDetails**<br/>**taskBoardTaskFormat**<br/>**planTaskBoard** |

### <a name="project-rome"></a>Projeto Roma

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Adicionou suporte ao Projeto Roma, incluindo [obter uma lista de dispositivos](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/user_list_devices), [enviar um comando para um dispositivo](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/send_device_command) e [verificar o status de um comando](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/get_device_command_status). |
| Adição        | Beta        | Suporte adicionado para [atividades](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/projectrome_activity) e [historyItems](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/projectrome_historyitem) de usuário, inclusive [operação upsert para atividade](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/projectrome_put_activity) e [operação upsert para historyItem](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/projectrome_put_historyitem). |

### <a name="administrative-units-property-changes"></a>Alterações de propriedade de unidades administrativas

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | Alterou o tipo de propriedade roleMemberInfo para [identity](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/identity) para a entidade [scopedRoleMembership](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/scopedrolemembership) |
| Alteração          | Beta        | Alterou a propriedade de navegação de scopedAdministratorOf para scopedRoleMemberOf para a entidade [user](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/user) |
| Alteração          | Beta        | Alterou a propriedade de navegação de scopedAdministrators para scopedRoleMembers para a entidade [administrativeUnit](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/administrativeunit) |
| Alteração          | Beta        | Alterou a propriedade de navegação de scopedAdministrators para scopedMembers para a entidade [directoryRole](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/directoryrole) |

### <a name="add-users-and-groups-webhook-support-in-preview"></a>Adicionar usuários e grupos de suporte do webhook na visualização

|**Tipo de alteração**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
| Alteração        | Beta       | Adicionou suporte aos [webhooks](https://developer.microsoft.com/graph/docs/api-reference/beta/resources/webhooks) para usuários e grupos.

### <a name="add-delta-query-to-v10"></a>Adicionar a consulta delta para v1.0

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Adicionar o suporte à função delta para V1.0. Adicionar às seguintes entidades para realizar [consulta delta](https://developer.microsoft.com/pt-BR/graph/docs/concepts/delta_query_overview):<br/>contato<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>Confira os seguintes exemplos:<br/>[Obter as alterações incrementais para grupos](https://developer.microsoft.com/pt-BR/graph/docs/concepts/delta_query_groups)<br/>[Obter as alterações incrementais para as mensagens em uma pasta](https://developer.microsoft.com/pt-BR/graph/docs/concepts/delta_query_messages)<br/>[Obter as alterações incrementais para usuários](https://developer.microsoft.com/pt-BR/graph/docs/concepts/delta_query_users) |
| Alteração          | Beta        | Adicionar um novo recurso de filtragem de consulta opcional (por ID) para [users](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/user_delta) e [groups](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/group_delta). |

### <a name="added-user-resource-support-for-deleted-items"></a>Foi adicionado suporte a recursos de usuário para os itens excluídos

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Adicionou suporte para a [restauração e a exclusão permanente de usuários](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/directory). |

### <a name="added-onpremisesprovisioningerror"></a>Adicionou OnPremisesProvisioningError

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | beta        | Nova entidade: [OnPremisesProvisioningError](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/onpremisesprovisioningerror) |
| Alteração          | beta        | Adicionou a propriedade OnPremisesProvisioningError para [user](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/user), [group](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/group) e [orgcontact](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/orgcontact) |

### <a name="added-deleteddatetime-property"></a>Adicionou a propriedade deletedDateTime

|**Tipo de alteração**|**Versão**|**Descrição**|
|:-------------|:-----------|:--------------|
|Alteração|beta|Adicionou a propriedade deletedDateTime à entidade [user](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/user).
|Alteração|beta|Adicionou a propriedade deletedDateTime à entidade [group](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/group).
|Alteração|beta|Adicionou a propriedade deletedDateTime à entidade [application](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/application).

### <a name="added-domain-operations-to-v10"></a>Adicionou operações de domínio para v1.0

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | V1.0        | Adicionou operações em [domains](https://graph.microsoft.io/pt-BR/docs/api-reference/v1.0/resources/domain).<br/>Novas entidades:</br>[domain](https://graph.microsoft.io/pt-BR/docs/api-reference/v1.0/resources/domain)<br/>[domainDnsRecord](https://graph.microsoft.io/pt-BR/docs/api-reference/v1.0/resources/domaindnsrecord)<br/>[domainDnsCnameRecord](https://graph.microsoft.io/pt-BR/docs/api-reference/v1.0/resources/domainDnsCnameRecord)<br/>[domainDnsMxRecord](https://graph.microsoft.io/pt-BR/docs/api-reference/v1.0/resources/domainDnsMxRecord)<br/>[domainDnsSrvRecord](https://graph.microsoft.io/pt-BR/docs/api-reference/v1.0/resources/domainDnsSrvRecord)<br/>[domainDnsTxtRecord](https://graph.microsoft.io/pt-BR/docs/api-reference/v1.0/resources/domainDnsTxtRecord)<br/>[domainDnsUnavailableRecord](https://graph.microsoft.io/pt-BR/docs/api-reference/v1.0/resources/domainDnsUnavailableRecord)<br/>Novas ações:</br>[verify](https://graph.microsoft.io/pt-BR/docs/api-reference/v1.0/api/domain_verify) |

### <a name="added-contracts-to-v10"></a>Adicionou contratos para v1.0

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | V1.0        | Nova entidade:</br>[contract](https://graph.microsoft.io/pt-BR/docs/api-reference/v1.0/resources/contract) |

### <a name="added-licensedetails-to-v10"></a>Adicionou licenseDetails para v1.0

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Nova entidade:</br>[licenseDetails](https://graph.microsoft.io/pt-BR/docs/api-reference/v1.0/resources/licensedetails) |
| Alteração          | v1.0        | Nova propriedade de navegação [licensedetails](https://graph.microsoft.io/pt-BR/docs/api-reference/v1.0/api/user_list_licensedetails) em [users](https://graph.microsoft.io/pt-BR/docs/api-reference/v1.0/resources/user) |


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
| Adição        | v1.0          | Suporte para [openTypeExtension](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/opentypeextension) nos seguintes recursos – [device](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/device), [group](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/group),[organization](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/organization), [user](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/user). |
| Adição        | v1.0 e beta | Quando o usuário está conectado com uma conta pessoal da Microsoft, suporte para extensões abertas nos seguintes recursos – evento, postagem, grupo, mensagem, contato e usuário. (É um adicional para estes recursos, além do dispositivo, grupo, organização e usuário, suporte a extensões abertas quando o usuário entra usando uma conta corporativa ou de estudante.) |
| Adição        | v1.0 e beta | Suporte para `$expand` para [obter extensões abertas](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/opentypeextension_get) nos seguintes recursos: [device](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/device), [group](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/group),[organization](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/organization), [post](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/post), [user](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/user). |
| Adição        | Beta          | Suporte para `$expand` para [obter extensões abertas](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/opentypeextension_get) na [administrativeUnit](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/administrativeunit). |


### <a name="extensions-schema-extensions"></a>Extensões (extensões de esquema) 

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0          | Novo recurso [schemaExtension](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/schemaextension) e métodos CRUD para gerenciar definições de extensão para os seguintes recursos: [contact](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/contact), [device](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/device), [event](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/event), [group](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/group), [message](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/message), [organization](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/organization), [post](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/post), [user](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/user). Observe que seu suporte para [administrativeUnit](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/administrativeunit) ainda está limitado à versão beta como antes. |
| Adição        | v1.0          | Os métodos POST, GET e PATCH existentes dos seguintes recursos: [contact](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/contact), [device](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/device), [event](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/event), [group](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/group), [message](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/message), [organization](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/organization), [post](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/post), [user](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/user) – agora suportam a adição, obtenção e carregamento ou exclusão de dados personalizados armazenados como extensões de esquema nas instâncias de recursos correspondentes. |
| Adição        | v1.0 e beta | Agora, você pode usar o `$filter` para pesquisar instâncias de recursos com propriedades que correspondam a valores de propriedade de extensão específicos, como nome de extensão. Confira este [exemplo](https://devx.microsoft-tst.com/pt-BR/graph/docs/concepts/extensibility_schema_groups#5-get-a-group-and-its-extension-data) para obter detalhes. |
| Alteração          | v1.0 e beta | [Excluir um esquema de definição de extensões](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/schemaextension_delete) não afeta mais o acesso a dados personalizados que foram adicionados com base nessa definição. |
| Alteração          | v1.0 e beta | Agora você pode definir um tipo complexo de extensão de esquema como nulo, para remover uma extensão de esquema de uma instância de recurso. |


### <a name="group"></a>Group

|**Tipo de alteração**|**Versão**|**Descrição**|
|:--------------|:----------|:--------------|
| Adição | v1.0 e beta | Foram adicionadas as propriedades de navegação **drives** e **sites** a **group**.

### <a name="insights-apis"></a>APIs de informações

|**Tipo de alteração**|**Versão**|**Descrição**| 
|:-------------|:-----------|:--------------|
|Adição|Beta|Foi adicionada a [API compartilhada](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/insights_shared).<br />Novos recursos:<br />[sharingDetail](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/insights_sharingdetail) <br />[insightIdentity](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/insights_insightidentity) <br />
|Adição|Beta|Foi adicionada a [API usada](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/insights_used).<br />Novos recursos:<br />[usageDetails](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/insights_usagedetails) <br />
|Alteração|Beta|Propriedade Novo **Tipo**no:<br />recurso [resourceVisualization](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/insights_resourcevisualization). <br />
|Exclusão|Beta|Foram removidas as seguintes entidades:<br/>**workingWith**<br/>**trendingAround**<br/>|

### <a name="intune-apis"></a>APIs do Intune

| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Adição    | Beta    | Foram adicionadas novas entidades:<br/>[androidForWorkMobileAppConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_androidforworkmobileappconfiguration)<br/>[cartToClassAssociation](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_carttoclassassociation)<br/>[deviceCompliancePolicySettingStateSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstatesummary)<br/>[eBookInstallSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_books_ebookinstallsummary)<br/>[eBookVppGroupAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_books_ebookvppgroupassignment)<br/>[iosUpdateConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosupdateconfiguration)<br/>[remoteAssistancePartner](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_remoteassistance_remoteassistancepartner)<br/>[windows10EndpointProtectionConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10endpointprotectionconfiguration)<br/>[windowsDeviceMalwareState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_endpointprotection_windowsdevicemalwarestate)<br/>[windowsInformationProtectionAppLearningSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_wip_windowsinformationprotectionapplearningsummary)<br/>[windowsMalwareInformation](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_endpointprotection_windowsmalwareinformation)<br/>[windowsProtectionState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_endpointprotection_windowsprotectionstate)<br/> |
| Adição    | Beta    | Foram adicionados novos tipos complexos:<br/>[androidPermissionAction](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_androidpermissionaction)<br/>[bitLockerSystemDrivePolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_bitlockersystemdrivepolicy)<br/>[defenderDetectedMalwareActions](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_defenderdetectedmalwareactions)<br/>[settingSource](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_settingsource)<br/> |
| Adição    | Beta    | A ação [assign](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_books_managedebook_assign) foi adicionada no [managedEBook](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_books_managedebook) |
| Adição    | Beta    | A ação [beginOnboarding](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_remoteassistance_remoteassistancepartner_beginonboarding) foi adicionada no [remoteAssistancePartner](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_remoteassistance_remoteassistancepartner) |
| Adição    | Beta    | A ação [disconnect](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_remoteassistance_remoteassistancepartner_disconnect) foi adicionada no [remoteAssistancePartner](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_remoteassistance_remoteassistancepartner) |
| Exclusão    | Beta    | Foram removidas as seguintes entidades:<br/>**outlookTask**<br/>**outlookTaskFolder**<br/>**outlookTaskGroup**<br/>**outlookUser**<br/>**windowsManagementAppHealthState**<br/> |
| Exclusão    | Beta    | Foram removidos os seguintes tipos complexos:<br/>**applePushNotificationCertificateSetting**<br/>**eventCreationOptions**<br/> |
| Alteração      | Beta    | As propriedades **workProfilePasswordBlockFingerprintUnlock**, **workProfilePasswordBlockTrustAgents**, **workProfilePasswordExpirationDays**, **workProfilePasswordMinimumLength**, **workProfilePasswordMinutesOfInactivityBeforeScreenTimeout**, **workProfilePasswordPreviousPasswordBlockCount**, **workProfilePasswordSignInFailureCountBeforeFactoryReset**, **workProfilePasswordRequiredType** e **workProfileRequirePassword** foram adicionadas à entidade [androidForWorkGeneralDeviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkgeneraldeviceconfiguration) |
| Alteração      | Beta    | A propriedade **subjectAlternativeNameFormatString** foi adicionada à entidade [androidForWorkPkcsCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkpkcscertificateprofile) |
| Alteração      | Beta    | As propriedades **subjectNameFormatString** e **subjectAlternativeNameFormatString** foram adicionadas à entidade [androidForWorkScepCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile) |
| Alteração      | Beta    | A propriedade **kioskModeManagedApps** foi adicionada à entidade [androidGeneralDeviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) |
| Alteração      | Beta    | A propriedade **kioskModeManagedAppId** foi removida da entidade [androidGeneralDeviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) |
| Alteração      | Beta    | A propriedade **subjectAlternativeNameFormatString** foi adicionada à entidade [androidPkcsCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidpkcscertificateprofile) |
| Alteração      | Beta    | As propriedades **subjectNameFormatString** e **subjectAlternativeNameFormatString** foram adicionadas à entidade [androidScepCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidscepcertificateprofile) |
| Alteração      | Beta    | A propriedade **hexColor** foi removida da entidade [calendar](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/calendar) |
| Alteração      | Beta    | As propriedades **setting** e **platformType** foram adicionadas à entidade [complianceSettingStateSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_compliancesettingstatesummary) |
| Alteração      | Beta    | A propriedade **windowsManagementAppEnabled** foi removida da entidade [deviceAppManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) |
| Alteração      | Beta    | As propriedades **userName**, **deviceModel** e **platform** foram adicionadas à entidade [deviceComplianceDeviceStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedevicestatus) |
| Alteração      | Beta    | As propriedades **userPrincipalName** e **deviceModel** foram adicionadas à entidade [deviceComplianceSettingState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate) |
| Alteração      | Beta    | As propriedades **platformType**, **setting**, **userId** e **userEmail** foram adicionadas à entidade [deviceComplianceSettingState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate) |
| Alteração      | Beta    | A propriedade **inGracePeriodCount** foi adicionada à entidade [deviceCompliancePolicyDeviceStateSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary) |
| Alteração      | Beta    | As propriedades **userName**, **deviceModel** e **platform** foram adicionadas à entidade [deviceConfigurationDeviceStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatus) |
| Alteração      | Beta    | A propriedade **creationOptions** foi removida da entidade [event](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/event) |
| Alteração      | Beta    | A propriedade **isDelegated** foi removida da entidade [eventMessage](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/eventMessage) |
| Alteração      | Beta    | As propriedades **unseenConversationsCount** e **unseenMessagesCount** foram removidas da entidade [group](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/group) |
| Alteração      | Beta    | As propriedades **settingXml** e **settings** foram adicionadas à entidade [iosMobileAppConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_iosmobileappconfiguration) |
| Alteração      | Beta    | A propriedade **subjectAlternativeNameFormatString** foi adicionada à entidade [iosPkcsCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iospkcscertificateprofile) |
| Alteração      | Beta    | A propriedade **subjectAlternativeNameFormatString** foi adicionada à entidade [iosScepCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosscepcertificateprofile) |
| Alteração      | Beta    | A propriedade **systemIntegrityProtectionEnabled** foi adicionada à entidade [macOSCompliancePolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscompliancepolicy) |
| Alteração      | Beta    | A propriedade **subjectAlternativeNameFormatString** foi adicionada à entidade [macOSScepCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosscepcertificateprofile) |
| Alteração      | Beta    | As propriedades **complianceGracePeriodExpirationDateTime**, **userPrincipalName** e **imei** foram adicionadas à entidade [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Alteração      | Beta    | As propriedades **settingXml** e **settings** foram removidas da entidade [managedDeviceMobileAppConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration) |
| Alteração      | Beta    | As propriedades **useSharedComputerActivation**, **updateChannel**, **officePlatformArchitecture** e **localesToInstall** foram adicionadas à entidade [officeSuiteApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp) |
| Alteração      | Beta    | A propriedade **applePushNotificationCertificateSetting** foi removida da entidade [organization](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_onboarding_organization) |
| Alteração      | Beta    | As propriedades a seguir foram alteradas na entidade [post](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/post):<br/>**sender** de opcional para obrigatório<br/> |
| Alteração      | Beta    | As propriedades **compliantUserCount**, **nonCompliantUserCount**, **remediatedUserCount**, **errorUserCount**, **unknownUserCount**, **conflictUserCount** e **notApplicableUserCount** foram adicionadas à entidade [softwareUpdateStatusSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_softwareupdatestatussummary) |
| Alteração      | Beta    | As propriedades **bluetoothAllowedServices**, **bluetoothBlockPrePairing**, **cellularData**, **defenderDetectedMalwareActions**, **defenderPotentiallyUnwantedAppAction**, **lockScreenAllowTimeoutConfiguration**, **lockScreenBlockCortana**, **lockScreenBlockToastNotifications**, **lockScreenTimeoutInSeconds**, **passwordBlockSimple**, **privacyAutoAcceptPairingAndConsentPrompts**, **privacyBlockInputPersonalization**, **startMenuHideChangeAccountSettings**, **startMenuHideHibernate**, **startMenuHideLock**, **startMenuHideShutDown**, **startMenuHideSignOut**, **startMenuHideSleep**, **startMenuHideSwitchAccount**, **settingsBlockAppsPage**, **settingsBlockGamingPage**, **windowsSpotlightBlockConsumerSpecificFeatures**, **windowsSpotlightBlocked**, **windowsSpotlightBlockOnActionCenter**, **windowsSpotlightBlockTailoredExperiences**, **windowsSpotlightBlockThirdPartyNotifications**, **windowsSpotlightBlockWelcomeExperience**, **windowsSpotlightBlockWindowsTips**, **windowsSpotlightConfigureOnLockScreen** e **connectedDevicesServiceBlocked** foram adicionadas à entidade [windows10GeneralConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) |
| Alteração      | Beta    | As propriedades **automaticUpdateMode**, **automaticUpdateSchedule**, **automaticUpdateTime**, **prereleaseFeatures**, **experienceBlockWindowsSpotlight**, **experienceBlockWindowsTips** e **experienceBlockConsumerSpecificFeatures** foram removidas da entidade [windows10GeneralConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) |
| Alteração      | Beta    | A propriedade **subjectAlternativeNameFormatString** foi adicionada à entidade [windows10PkcsCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10pkcscertificateprofile) |
| Alteração      | Beta    | As propriedades **subjectNameFormatString** e **subjectAlternativeNameFormatString** foram adicionadas à entidade [windows81SCEPCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81scepcertificateprofile) |
| Alteração      | Beta    | As propriedades **indexingEncryptedStoresOrItemsBlocked** e **smbAutoEncryptedFileExtensions** foram adicionadas à entidade [windowsInformationProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection) |
| Alteração      | Beta    | As seguintes propriedades foram alteradas na entidade [windowsInformationProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection):<br/>**rightsManagementServicesTemplateId** de obrigatório para opcional<br/> |
| Alteração      | Beta    | As seguintes propriedades foram alteradas na entidade [windowsMobileMSI](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi):<br/>**productCode** de obrigatório para opcional<br/> |
| Alteração      | Beta    | As propriedades **subjectNameFormatString** e **subjectAlternativeNameFormatString** foram adicionadas à entidade [windowsPhone81SCEPCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81scepcertificateprofile) |
| Alteração      | Beta    | A propriedade de navegação **mobileAppConfigurations** foi adicionada à entidade [deviceAppManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) |
| Alteração      | Beta    | As propriedades de navegação **cartToClassAssociations**, **deviceCompliancePolicySettingStateSummaries**, **remoteAssistancePartners**, **windowsInformationProtectionAppLearningSummaries** e **windowsMalwareInformation** foram adicionadas à entidade [deviceManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) |
| Alteração      | Beta    | A propriedade de navegação **eBook** foi adicionada à entidade [eBookGroupAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_books_ebookgroupassignment) |
| Alteração      | Beta    | A propriedade de navegação **windowsProtectionState** foi adicionada à entidade [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Alteração      | Beta    | A propriedade de navegação **installSummary** foi adicionada à entidade [managedEBook](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_books_managedebook) |
| Alteração      | Beta    | A propriedade de navegação **outlook** foi removida da entidade [user](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_user) |
| Alteração      | Beta    | A propriedade de navegação **healthStates** foi removida da entidade [windowsManagementApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsmanagementapp) |
| Alteração      | Beta    | A propriedade **androidForWorkRestrictions** foi adicionada ao tipo complexo [defaultDeviceEnrollmentRestrictions](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_onboarding_defaultdeviceenrollmentrestrictions) |
| Alteração      | Beta    | As propriedades **userPrincipalName** e **sources** foram adicionadas ao tipo complexo [deviceCompliancePolicySettingState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate) |
| Alteração      | Beta    | As propriedades **userPrincipalName** e **sources** foram adicionadas ao tipo complexo [deviceConfigurationSettingState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) |
| Alteração      | Beta    | As propriedades **settingName**, **userId**, **userName**, **userEmail** e **currentValue** foram adicionadas ao tipo complexo [deviceConfigurationSettingState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate) |
| Alteração      | Beta    | A propriedade **archiveFolder** foi removida do tipo complexo [mailboxSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/mailboxSettings) |


### <a name="outlook-calendar"></a>Calendário do Outlook

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0 e beta | Para **findMeetingTimes**, adicionou o novo valor de enumeração **unrestricted** que você especifica como a propriedade **activityDomain**, parte do parâmetro **timeConstraint**. Isso permite que **findMeetingTimes** procure os horários apropriados para o tipo de atividade que você está agendando. Confira detalhes na seção [corpo da solicitação](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/user_findmeetingtimes#request-body). |
| Adição        | Beta          | Suporte para obter um corpo de **event** em um texto sem formatação, como alternativa ao formato HTML padrão. Confira os eventos [get](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/event_get) e [list](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/user_list_events) para obter detalhes. |

### <a name="outlook-mail"></a>Email do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | Suporte para obter um corpo de **message** em um texto sem formatação, como alternativa ao formato HTML padrão. Confira os eventos [get](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/message_get) e [list](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/user_list_messages) para obter detalhes. |


### <a name="outlook-tasks"></a>Tarefas do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Nova propriedade de navegação do **outlook** adicionado a [user](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/user), para acessar tarefas do Outlook. |
| Adição        | Beta        | Novas entidades: [outlookuser](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/outlookuser), [outlookTaskGroup](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/outlooktaskgroup), [outlookTaskFolder](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/outlooktaskfolder) e [outlookTask](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/outlooktask), e seus métodos suportam a organização e o acesso a tarefas do Outlook. |
| Adição        | Beta        | As tarefas do Outlook suportam anexos (recursos [attachment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/attachment), [fileAttachment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/fileattachment), [itemAttachment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/itemattachment) e [referenceAttachment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/referenceattachment)). |
| Adição        | Beta        | As tarefas do Outlook suportam [propriedades estendidas](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/extended-properties-overview) (recursos [singleValueLegacyExtendedProperty](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/singlevaluelegacyextendedproperty) e [multiValueLegacyExtendedProperty](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/multivaluelegacyextendedproperty)). |

### <a name="planner-apis"></a>APIs do Planner

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Adicionou a [API do Planner](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/planner_overview).<br />Novos recursos:<br />[plannerPlan](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/plannerPlan) <br />[plannerTask](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/plannerTask) <br />[plannerPlanDetails](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/plannerPlanDetails) <br />[plannerTaskDetails](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/plannerTaskDetails) <br />[plannerBucket](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/plannerBucket) <br />[plannerAssignedToTaskBoardTaskFormat](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/plannerassignedtotaskboardtaskformat) <br />[plannerBucketTaskBoardTaskFormat](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/plannerBuckettaskboardtaskformat) <br />[plannerProgressTaskBoardTaskFormat](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/plannerprogresstaskboardtaskformat) |

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

### <a name="application-and-serviceprincipal-api-changes"></a>Alterações da API Application e servicePrincipal

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | As APIs de [aplicativo](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/application) e [servicePrincipal](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/serviceprincipal) serão atualizadas na visualização (beta). O primeiro conjunto de alterações será aplicado em 15 de maio de 2017. As alterações incluem a renomeação e a reestruturação de propriedade. Algumas propriedades (como funções de aplicativos e suplementos) não estarão disponíveis até que as alterações sejam concluídas. As alterações serão lançadas na Visualização (beta) antes do lançamento da versão 1.0. |

### <a name="added-preview-support-for-cloud-solution-provider-developers"></a>Foi adicionado o suporte à visualização para desenvolvedores de Provedor de Soluções na Nuvem

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foram adicionados novos recursos de visualização para permitir que os aplicativos previamente consentidos do Provedor de Soluções na Nuvem chamem o Microsoft Graph, descrito em um novo [tópico de autorização](https://graph.microsoft.io/pt-BR/docs/concepts/auth_cloudsolutionprovider). |

### <a name="added-onpremises-properties-to-user-entity"></a>Adicionadas propriedades onPremises à entidade do usuário

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foram adicionadas novas propriedades onPremises, onPremisesDomainName, OnPremisesSamAccountName e onPremisesUserPrincipalName à entidade do [usuário](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/user). |

### <a name="new-planner-apis-and-an-update-to-the-group-visibility-property"></a>Novas APIs do Planner e uma atualização da propriedade de visibilidade do grupo

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | Foi adicionado o **HiddenMembership** como um valor adicional para a propriedade de visibilidade para a entidade de [Grupo](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/group) |
| Adição        | Beta        | Foi adicionada uma nova [API do Planner](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/planner_overview).<br />Novos recursos:<br />[plannerPlan](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/plannerPlan) <br />[plannerTask](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/plannerTask) <br />[plannerPlanDetails](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/plannerPlanDetails) <br />[plannerTaskDetails](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/plannerTaskDetails) <br />[plannerBucket](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/plannerBucket) <br />[plannerAssignedToTaskBoardTaskFormat](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/plannerassignedtotaskboardtaskformat) <br />[plannerBucketTaskBoardTaskFormat](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/plannerBuckettaskboardtaskformat) <br />[plannerProgressTaskBoardTaskFormat](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/plannerprogresstaskboardtaskformat) |

### <a name="intune-apis"></a>APIs do Intune
| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foram adicionadas novas entidades:<br/>[androidForWorkCompliancePolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkcompliancepolicy)<br/>[deviceComplianceSettingState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancesettingstate)<br/>[deviceInstallState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_books_deviceinstallstate)<br/>[deviceManagementScript](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscript)<br/>[deviceManagementScriptGroupAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscriptgroupassignment)<br/>[deviceManagementScriptState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscriptstate)<br/>[eBookGroupAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_books_ebookgroupassignment)<br/>[iosVppEBook](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_books_iosvppebook)<br/>[managedEBook](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_books_managedebook)<br/>[userInstallStateSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_books_userinstallstatesummary)<br/>[windowsManagementApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsmanagementapp)<br/>[windowsManagementAppHealthState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsmanagementapphealthstate)<br/> |
| Adição        | Beta        | Foram adicionados novos tipos complexos:<br/>[dailySchedule](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_dailyschedule)<br/>[hourlySchedule](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_hourlyschedule)<br/>[iosBookmark](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosbookmark)<br/>[iosWebContentFilterAutoFilter](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterautofilter)<br/>[iosWebContentFilterBase](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterbase)<br/>[iosWebContentFilterSpecificWebsitesAccess](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioswebcontentfilterspecificwebsitesaccess)<br/>[runSchedule](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_runschedule)<br/>[sharedAppleDeviceUser](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedappledeviceuser)<br/>[windows10NetworkProxyServer](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10networkproxyserver)<br/> |
| Adição        | Beta        | Foi adicionada a ação [requestRemoteAssistance](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_requestremoteassistance) ao [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Adição        | Beta        | Foi adicionada a ação [cleanWindowsDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_cleanwindowsdevice) ao [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Adição        | Beta        | Foi adicionada a ação [logoutSharedAppleDeviceActiveUser](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_logoutsharedappledeviceactiveuser) ao [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Adição        | Beta        | Foi adicionada a ação [deleteUserFromSharedAppleDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_deleteuserfromsharedappledevice) ao [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Adição        | Beta        | Foi adicionada a ação [assign](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_deviceconfig_devicemanagementscript_assign) ao [deviceManagementScript](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementscript) |
| Adição        | Beta        | Foi adicionada a ação [syncLicenses](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_onboarding_applevolumepurchaseprogramtoken_synclicenses) ao [appleVolumePurchaseProgramToken](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_applevolumepurchaseprogramtoken) |
| Adição        | Beta        | Foi adicionada a função **getTopMobileApps** à coleção [mobileApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) |
| Adição        | Beta        | Foi adicionada a função [downloadApplePushNotificationCertificateSigningRequest](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_deviceconfig_applepushnotificationcertificate_downloadapplepushnotificationcertificatesigningrequest) a [applePushNotificationCertificate](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_applepushnotificationcertificate) |
| Adição        | Beta        | Foi adicionada a função [getDeviceComplianceSettingStates](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_deviceconfig_devicemanagement_getdevicecompliancesettingstates) a [deviceManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) |
| Adição        | Beta        | Foi adicionada a função [deviceConfigurationUserActivity](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_deviceconfig_reportroot_deviceconfigurationuseractivity) a [reportRoot](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_reportroot) |
| Adição        | Beta        | Foi adicionada a função [deviceConfigurationDeviceActivity](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_deviceconfig_reportroot_deviceconfigurationdeviceactivity) a [reportRoot](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_reportroot) |
| Exclusão        | Beta        | Foram removidos os seguintes tipos complexos:<br/>**enterpriseCloudResource**<br/>**windowsInformationProtectionAppRule**<br/>**windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate**<br/>**windowsInformationProtectionAppRuleDesktopTemplate**<br/>**windowsInformationProtectionAppRuleStoreAppTemplate**<br/>**windowsInformationProtectionAppRuleTemplate**<br/>**windowsInformationProtectionCorporateNetworkLocation**<br/>**windowsInformationProtectionProtectedLocation**<br/>**windowsInformationProtectionProtectedLocationEnterpriseCloudResources**<br/>**windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges**<br/>**windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames**<br/>**windowsInformationProtectionProtectedLocationEnterpriseProxyServers**<br/>**windowsInformationProtectionProtectedLocationNeutralResources**<br/> |
| Alteração          | Beta        | Foi adicionada a propriedade **deviceSharingAllowed** à entidade [androidGeneralDeviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) |
| Alteração          | Beta        | Foi removida a propriedade **deviceSharingBlocked** à entidade [androidGeneralDeviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) |
| Alteração          | Beta        | Foi adicionada a propriedade **minimumRequiredSdkVersion** à entidade [defaultManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_defaultmanagedappprotection) |
| Alteração          | Beta        | Foi adicionada a propriedade **windowsManagementAppEnabled** à entidade [deviceAppManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) |
| Alteração          | Beta        | Adicionada a propriedade **notificationTemplateId** à entidade [deviceComplianceActionItem](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceactionitem) |
| Alteração          | Beta        | Foi adicionada a propriedade **excludeGroup** à entidade [deviceConfigurationGroupAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationgroupassignment) |
| Alteração          | Beta        | Foram alteradas as seguintes propriedades na entidade [iosCustomConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioscustomconfiguration):<br/>**payloadFileName** de obrigatório para opcional<br/> |
| Alteração          | Beta        | Foi adicionada a propriedade **contentFilterSettings** à entidade [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration) |
| Alteração          | Beta        | Adicionadas as propriedades **cellularBlockPersonalHotspot** e **passcodeBlockFingerprintModification** à entidade [iosGeneralDeviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration) |
| Alteração          | Beta        | Foi adicionada a propriedade **minimumRequiredSdkVersion** à entidade [iosManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) |
| Alteração          | Beta        | Foram alteradas as seguintes propriedades na entidade [macOSCustomConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscustomconfiguration):<br/>**payloadFileName** de obrigatório para opcional<br/> |
| Alteração          | Beta        | Foram adicionadas as propriedades **disableAppPinIfDevicePinIsSet**, **minimumRequiredOsVersion**, **minimumWarningOsVersion**, **minimumRequiredAppVersion** e **minimumWarningAppVersion** à entidade [managedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_managedappprotection) |
| Alteração          | Beta        | Foram adicionadas as propriedades **remoteAssistanceSessionUrl**, **isEncrypted**, **modelo** e **fabricante** à entidade [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Alteração          | Beta        | As propriedades a seguir foram alteradas na entidade [getMobileAppCount](https://developer.microsoft.com/pt-BR/graph/docs/docs/api-reference/beta/api/intune_apps_mobileapp_getmobileappcount):<br/>**bindingParameter** de **mobileApp** para uma **collection** de *mobileApp*<br/>**status** de um GUID para uma Cadeia de caracteres<br/> |
| Alteração          | Beta        | Foi adicionada a propriedade **vpnConfigurationId** à entidade [mobileAppGroupAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileappgroupassignment) |
| Alteração          | Beta        | Foi removida a propriedade **fromEmailAddress** da entidade [notificationMessageTemplate](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_notificationmessagetemplate) |
| Alteração          | Beta        | Foi adicionada a propriedade **excludedApps** à entidade [officeSuiteApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp) |
| Alteração          | Beta        | Foi removida a propriedade **excludedOfficeApps** da entidade [officeSuiteApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp) |
| Alteração          | Beta        | Foi adicionada a propriedade **enabled** à entidade [sharedPCConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcconfiguration) |
| Alteração          | Beta        | Foram adicionadas as propriedades **networkProxyApplySettingsDeviceWide**, **networkProxyDisableAutoDetect**, **networkProxyAutomaticConfigurationUrl**, **networkProxyServer**, **bluetoothDeviceName**, **wiFiScanInterval**, **wirelessDisplayBlockProjectionToThisDevice**, **wirelessDisplayBlockUserInputFromReceiver**, **wirelessDisplayRequirePinForPairing**, **experienceBlockDeviceDiscovery**, **experienceBlockErrorDialogWhenNoSIM**, **experienceBlockTaskSwitcher**, ** startMenuPinnedFolderDocuments**, **startMenuPinnedFolderDownloads**, **startMenuPinnedFolderFileExplorer**, **startMenuPinnedFolderHomeGroup**, **startMenuPinnedFolderMusic**, **startMenuPinnedFolderNetwork**, **startMenuPinnedFolderPersonalFolder**, **startMenuPinnedFolderPictures**, **startMenuPinnedFolderSettings**, **startMenuPinnedFolderVideos**, **startMenuAppListVisibility**, **startMenuHideFrequentlyUsedApps**, ** startMenuHideRecentJumpLists**, **startMenuHideRecentlyAddedApps**, **startMenuHideRestartOptions**, **startMenuHideUserTile**, **startMenuHidePowerButton**, **startMenuLayoutEdgeAssetsXml**, **personalizationDesktopImageUrl** e **personalizationLockScreenImageUrl** à entidade [windows10GeneralConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) |
| Alteração          | Beta        | Foi alterado o tipo das seguintes propriedades na entidade [windowsMobileMSI](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi):<br/>**productCode** do Guid para a cadeia de caracteres<br/> |
| Alteração          | Beta        | Foram alteradas as seguintes propriedades na entidade [windowsPhone81AppX](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx):<br/>**phoneProductIdentifier** de obrigatório para opcional<br/>**phonePublisherId** de obrigatório para opcional<br/> |
| Alteração          | Beta        | Foram alteradas as seguintes propriedades na entidade [windowsPhone81AppXBundle](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appxbundle):<br/>**appXPackageInformationList** de obrigatório para opcional<br/> |
| Alteração          | Beta        | Foram adicionadas as propriedades **productKey** e **licenseType** à entidade [windowsStoreForBusinessApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsstoreforbusinessapp) |
| Alteração          | Beta        | Foi adicionada a propriedade **previewBuildSetting** à entidade [windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration) |
| Alteração          | Beta        | Foram adicionadas as propriedades de navegação **windowsManagementApp** e **managedEBooks** à entidade [deviceAppManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) |
| Alteração          | Beta        | Foram adicionadas as propriedades de navegação **deviceManagementScripts**, **managedDeviceOverview** e **cloudPkiSubscriptions** à entidade [deviceManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) |
| Alteração          | Beta        | Foram adicionadas as propriedades **osMinimumVersion** e **osMaximumVersion** ao tipo complexo [deviceEnrollmentPlatformRestrictions](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_onboarding_deviceenrollmentplatformrestrictions) |
| Alteração          | Beta        | Foram adicionadas as propriedades **isSharedDevice** e **sharedDeviceCachedUsers** ao tipo complexo [hardwareInformation](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_hardwareinformation) |
| Alteração          | Beta        | Foram alteradas as seguintes propriedades no tipo complexo [omaSettingBase64](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_omasettingbase64):<br/>**fileName** de obrigatório para opcional<br/> |
| Alteração          | Beta        | Foram alteradas as seguintes propriedades no tipo complexo [omaSettingStringXml](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_omasettingstringxml):<br/>**fileName** de obrigatório para opcional<br/> |

## <a name="march-2017"></a>Março de 2017

### <a name="intune-apis"></a>APIs do Intune

| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Adição    | Beta    | Foram adicionadas novas entidades:<br/>[androidForWorkApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_androidforworkapp)<br/>[androidForWorkAppConfigurationSchema](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationschema)<br/>[androidForWorkSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings)<br/>[androidForWorkVpnConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkvpnconfiguration)<br/>[applePushNotificationCertificate](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_applepushnotificationcertificate)<br/>[complianceSettingStateSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_compliancesettingstatesummary)<br/>[deviceCompliancePolicyDeviceStateSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicydevicestatesummary)<br/>[deviceCompliancePolicyState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicystate)<br/>[deviceConfigurationDeviceStateSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatesummary)<br/>[deviceConfigurationState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationstate)<br/>[enterpriseCodeSigningCertificate](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_enterprisecodesigningcertificate)<br/>[iosEduDeviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosedudeviceconfiguration)<br/>[managedDeviceCertificateState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevicecertificatestate)<br/>[managedDeviceMobileAppConfigurationDeviceSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicesummary)<br/>[managedDeviceMobileAppConfigurationUserSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationusersummary)<br/>[mdmWindowsInformationProtectionPolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_mdmwindowsinformationprotectionpolicy)<br/>[mobileAppInstallSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallsummary)<br/>[mobileAppProvisioningConfigGroupAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileappprovisioningconfiggroupassignment)<br/>[mobileThreatDefenseConnector](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_onboarding_mobilethreatdefenseconnector)<br/>[officeSuiteApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_officesuiteapp)<br/>[settingStateDeviceSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_settingstatedevicesummary)<br/>[softwareUpdateStatusSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_softwareupdatestatussummary)<br/>[symantecCodeSigningCertificate](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_symanteccodesigningcertificate)<br/>[windowsDefenderAdvancedThreatProtectionConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsdefenderadvancedthreatprotectionconfiguration)<br/>[windowsInformationProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection)<br/>[windowsInformationProtectionAppLockerFile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionapplockerfile)<br/>[windowsInformationProtectionPolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionpolicy)<br/>[windowsMobileMSI](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsmobilemsi)<br/> |
| Adição    | Beta    | Foram adicionados novos tipos complexos:<br/>[androidForWorkAppConfigurationExample](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationexample)<br/>[androidForWorkAppConfigurationExampleJson](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationexamplejson)<br/>[androidForWorkAppConfigurationSchemaItem](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworkappconfigurationschemaitem)<br/>[deviceCompliancePolicySettingState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicysettingstate)<br/>[deviceConfigurationSettingState](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationsettingstate)<br/>[deviceExchangeAccessStateSummary](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceexchangeaccessstatesummary)<br/>[edgeSearchEngine](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchengine)<br/>[edgeSearchEngineBase](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchenginebase)<br/>[edgeSearchEngineCustom](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_edgesearchenginecustom)<br/>[excludedApps](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_excludedapps)<br/>[iosEduCertificateSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducertificatesettings)<br/>[ipRange](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iprange)<br/>[windowsInformationProtectionApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionapp)<br/>[windowsInformationProtectionCloudResource](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioncloudresource)<br/>[windowsInformationProtectionCloudResourceCollection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioncloudresourcecollection)<br/>[windowsInformationProtectionDesktopApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondesktopapp)<br/>[windowsInformationProtectionIPRangeCollection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectioniprangecollection)<br/>[windowsInformationProtectionResourceCollection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionresourcecollection)<br/>[windowsInformationProtectionStoreApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionstoreapp)<br/> |
| Adição    | Beta    | Foi adicionada a ação [requestSignupUrl](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_requestsignupurl) ao [androidForWorkSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) |
| Adição    | Beta    | Foi adicionada a ação [completeSignup](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_completesignup) ao [androidForWorkSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) |
| Adição    | Beta    | Foi adicionada a ação [syncApps](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_syncapps) ao [androidForWorkSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) |
| Adição    | Beta    | Foi adicionada a ação [unbind](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_androidforwork_androidforworksettings_unbind) ao [androidForWorkSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_androidforworksettings) |
| Adição    | Beta    | Foi adicionada a ação [assign](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_apps_ioslobappprovisioningconfiguration_assign) a [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) |
| Adição    | Beta    | Foi adicionada a ação [recoverPasscode](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_deviceconfig_manageddevice_recoverpasscode) a [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Adição    | Beta    | Foi adicionada a ação [removeApplePushNotificationCertificate](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_onboarding_organization_removeapplepushnotificationcertificate) a [organization](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_onboarding_organization) |
| Adição    | Beta    | Foi adicionada a ação [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_mam_iosmanagedappprotection_updatemobileappidentifierdeployments) a [iosManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) |
| Adição    | Beta    | Foi adicionada a ação [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_mam_androidmanagedappprotection_updatemobileappidentifierdeployments) a [androidManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) |
| Adição    | Beta    | Foi adicionada a ação [updateMobileAppIdentifierDeployments](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_mam_targetedmanagedappconfiguration_updatemobileappidentifierdeployments) a [targetedManagedAppConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) |
| Adição    | Beta    | Foi adicionada a ação [updateTargetedSecurityGroups](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_mam_iosmanagedappprotection_updatetargetedsecuritygroups) a [iosManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_iosmanagedappprotection) |
| Adição    | Beta    | Foi adicionada a ação [updateTargetedSecurityGroups](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_mam_androidmanagedappprotection_updatetargetedsecuritygroups) a [androidManagedAppProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_androidmanagedappprotection) |
| Adição    | Beta    | Foi adicionada a ação [updateTargetedSecurityGroups](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_mam_windowsinformationprotection_updatetargetedsecuritygroups) a [windowsInformationProtection](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotection) |
| Adição    | Beta    | Foi adicionada a ação [updateTargetedSecurityGroups](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_mam_windowsinformationprotection_updatetargetedsecuritygroups) a [windowsInformationProtectionPolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectionpolicy) |
| Adição    | Beta    | Foi adicionada a ação [updateTargetedSecurityGroups](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_mam_mdmwindowsinformationprotectionpolicy_updatetargetedsecuritygroups) a [mdmWindowsInformationProtectionPolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_mdmwindowsinformationprotectionpolicy) |
| Adição    | Beta    | Foi adicionada a ação [wipeManagedAppRegistrationByDeviceTag](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_mam_user_wipemanagedappregistrationbydevicetag) a [user](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_user) |
| Adição    | Beta    | Foi adicionada a função [getTopMobileApps](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_apps_mobileapp_gettopmobileapps) a [mobileApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) |
| Adição    | Beta    | Foi adicionada a função [verifyWindowsEnrollmentAutoDiscovery](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_corpenrollment_devicemanagement_verifywindowsenrollmentautodiscovery) a [deviceManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) |
| Exclusão    | Beta    | Foram removidas as seguintes entidades:<br/>**appProvisioningConfigGroupAssignment**<br/>**defaultManagedAppConfiguration**<br/>**enterpriseCertificate**<br/>**managedDeviceMobileAppProvisioningConfigurationDeviceStatus**<br/>**symantecCertificate**<br/>**windows10WindowsInformationProtectionConfiguration**<br/> |
| Exclusão    | Beta    | Foram removidos os seguintes tipos complexos:<br/>**mobileAppInstallSummary**<br/>**windowsArchitecture**<br/>**windowsDeviceType**<br/> |
| Alteração      | Beta    | Foi adicionada a propriedade **webBrowserBlockPopups** à entidade [androidGeneralDeviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) |
| Alteração      | Beta    | Foi removida a propriedade **webBrowserAllowPopups** da entidade [androidGeneralDeviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidgeneraldeviceconfiguration) |
| Alteração      | Beta    | Foi adicionada a propriedade **appIdentifier** à entidade [androidStoreApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_androidstoreapp) |
| Alteração      | Beta    | Foram removidas as propriedades **applicationCount**, **failedApplicationCount** e **appInstallFailures** da entidade [appReportingOverviewStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/appReportingOverviewStatus) |
| Alteração      | Beta    | Foram adicionadas as propriedades **sharedIPadMaximumUserCount** e **enableSharedIPad** à entidade [depEnrollmentProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_corpenrollment_depenrollmentprofile) |
| Alteração      | Beta    | Foram adicionadas as propriedades **shareTokenWithSchoolDataSyncService** e **lastSyncErrorCode** à entidade [depOnboardingSetting](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_onboarding_deponboardingsetting) |
| Alteração      | Beta    | Foram adicionadas as propriedades **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** e **configurationVersion** à entidade [deviceComplianceDeviceOverview](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview) |
| Alteração      | Beta    | Foram removidas as propriedades **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** e **policyRevision** da entidade [deviceComplianceDeviceOverview](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview) |
| Alteração      | Beta    | Foram adicionadas as propriedades **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** e **configurationVersion** à entidade [deviceComplianceUserOverview](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview) |
| Alteração      | Beta    | Foram removidas as propriedades **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** e **policyRevision** da entidade [deviceComplianceUserOverview](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview) |
| Alteração      | Beta    | Foram adicionadas as propriedades **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** e **configurationVersion** à entidade [deviceConfigurationDeviceOverview](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview) |
| Alteração      | Beta    | Foram removidas as propriedades **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** e **policyRevision** da entidade [deviceConfigurationDeviceOverview](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview) |
| Alteração      | Beta    | Foram adicionadas as propriedades **pendingCount**, **successCount**, **errorCount**, **failedCount**, **lastUpdateDateTime** e **configurationVersion** à entidade [deviceConfigurationUserOverview](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview) |
| Alteração      | Beta    | Foram removidas as propriedades **numberOfPendingDevices**, **numberOfSucceededDevices**, **numberOfErrorDevices**, **numberOfFailedDevices**, **lastUpdateTime** e **policyRevision** da entidade [deviceConfigurationUserOverview](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview) |
| Alteração      | Beta    | Foi adicionada a propriedade **subscriptionState** à entidade [deviceManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) |
| Alteração      | Beta    | Foi adicionada a propriedade **managedEmailProfileRequired** à entidade [iosCompliancePolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioscompliancepolicy) |
| Alteração      | Beta    | Foi adicionada a propriedade **appsSingleAppModeList** à entidade [iosGeneralDeviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration) |
| Alteração      | Beta    | Foi removida a propriedade **appsSingleAppModeBundleIds** da entidade [iosGeneralDeviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration) |
| Alteração      | Beta    | Foi adicionada a propriedade **expirationDateTime** à entidade [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) |
| Alteração      | Beta    | Foi removida a propriedade **expiration** da entidade [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) |
| Alteração      | Beta    | Foram adicionadas as propriedades **passwordMinimumCharacterSetCount**, **osMinimumVersion**, **osMaximumVersion**, **deviceThreatProtectionEnabled**, **deviceThreatProtectionRequiredSecurityLevel** e **storageRequireEncryption** à entidade [macOSCompliancePolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_macoscompliancepolicy) |
| Alteração      | Beta    | Foi removida a propriedade **manifest** da entidade [managedAndroidLobApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_managedandroidlobapp) |
| Alteração      | Beta    | Foram adicionadas as propriedades **isSupervised**, **exchangeLastSuccessfulSyncDateTime**, **exchangeAccessState** e **exchangeAccessStateReason** à entidade [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Alteração      | Beta    | Foi adicionada a propriedade **deviceExchangeAccessStateSummary** à entidade [managedDeviceOverview](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddeviceoverview) |
| Alteração      | Beta    | Foi removida a propriedade **manifest** da entidade [managedIOSLobApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_managedioslobapp) |
| Alteração      | Beta    | Foi removida a propriedade **installSummary** da entidade [mobileApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) |
| Alteração      | Beta    | Foi adicionada a propriedade **uploadState** à entidade [mobileAppContentFile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile) |
| Alteração      | Beta    | Foram alteradas as seguintes propriedades na entidade [mobileAppContentFile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile):<br/>**azureStorageUriExpirationDateTime** de obrigatório para opcional<br/> |
| Alteração      | Beta    | Foram adicionadas as propriedades **initiatedByUserPrincipalName**, **deviceOwnerUserPrincipalName**, **deviceIMEI** e **actionState** à entidade [remoteActionAudit](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_remoteactionaudit) |
| Alteração      | Beta    | Foram adicionadas as propriedades **oneDriveDisableFileSync**, **safeSearchFilter**, **edgeSearchEngine**, **settingsBlockSettingsApp**, **settingsBlockSystemPage**, **settingsBlockDevicesPage**, **settingsBlockNetworkInternetPage**, **settingsBlockPersonalizationPage**, **settingsBlockAccountsPage**, **settingsBlockTimeLanguagePage**, **settingsBlockEaseOfAccessPage**, **settingsBlockPrivacyPage**, **settingsBlockUpdateSecurityPage**, ** experienceBlockWindowsSpotlight**, **experienceBlockWindowsTips**, **experienceBlockConsumerSpecificFeatures**, **startMenuLayoutXml**, **startMenuMode**, **logonBlockFastUserSwitching** e **startBlockUnpinningAppsFromTaskbar** à entidade [windows10GeneralConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration) |
| Alteração      | Beta    | Foram adicionadas as propriedades **allowPrinting**, **allowScreenCapture** e **allowTextSuggestion** à entidade [windows10SecureAssessmentConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration) |
| Alteração      | Beta    | Foram removidas as propriedades **blockPrinting**, **blockScreenCapture** e **blockTextSuggestion** da entidade [windows10SecureAssessmentConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration) |
| Alteração      | Beta    | Foi adicionada a propriedade **identityName** à entidade [windowsAppX](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsappx) |
| Alteração      | Beta    | Foi alterado o tipo das seguintes propriedades na entidade [windowsAppX](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsappx):<br/>**applicableArchitectures** de [windowsArchitecture](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/windowsArchitecture) para cadeia de caracteres<br/> |
| Alteração      | Beta    | Foi adicionada a propriedade **identityName** à entidade [windowsPhone81AppX](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx) |
| Alteração      | Beta    | Foi alterado o tipo das seguintes propriedades na entidade [windowsPhone81AppX](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx):<br/>**applicableArchitectures** de [windowsArchitecture](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/windowsArchitecture) para cadeia de caracteres<br/> |
| Alteração      | Beta    | Foram adicionadas as propriedades **identityName**, **identityPublisherHash** e **identityResourceIdentifier** à entidade [windowsUniversalAppX](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx) |
| Alteração      | Beta    | Foi alterado o tipo das seguintes propriedades na entidade [windowsUniversalAppX](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx):<br/>**applicableArchitectures** de [windowsArchitecture](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/windowsArchitecture) para cadeia de caracteres<br/>**applicableDeviceTypes** de [windowsDeviceType](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/windowsDeviceType) para a cadeia de caracteres<br/> |
| Alteração      | Beta    | Foi adicionada a propriedade **restartMode** à entidade [windowsUpdateForBusinessConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsupdateforbusinessconfiguration) |
| Alteração      | Beta    | Foi adicionada a propriedade de navegação **managedDeviceCertificateStates** à entidade [androidForWorkScepCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile) |
| Alteração      | Beta    | Foi adicionada a propriedade de navegação **managedDeviceCertificateStates** à entidade [androidScepCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidscepcertificateprofile) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **enterpriseCodeSigningCertificates**, **symantecCodeSigningCertificate**, **sideLoadingKeys**, **managedAppPolicies**, **iosManagedAppProtections**, **androidManagedAppProtections**, **defaultManagedAppProtections**, **targetedManagedAppConfigurations**, **mdmWindowsInformationProtectionPolicies**, **windowsInformationProtectionPolicies**, **managedAppRegistrations** e **managedAppStatuses** à entidade [deviceAppManagement ](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) |
| Alteração      | Beta    | Foram removidas as propriedades de navegação **appReportingOverview**, **enterpriseCerts** e **symantecCert** da entidade [deviceAppManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) |
| Alteração      | Beta    | Foi adicionada a propriedade de navegação **deviceSettingStateSummaries** à entidade [deviceCompliancePolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy) |
| Alteração      | Beta    | Foi adicionada a propriedade de navegação **deviceSettingStateSummaries** à entidade [deviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **termsAndConditions**, **androidForWorkSettings**, **androidForWorkAppConfigurationSchemas**, **applePushNotificationCertificate**, **softwareUpdateStatusSummary**, **deviceCompliancePolicyDeviceStateSummary**, **complianceSettingStateSummaries**, **deviceConfigurationDeviceStateSummaries** e **mobileThreatDefenseConnectors** à entidade [deviceManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_androidforwork_devicemanagement) |
| Alteração      | Beta    | Foram removidas as propriedades de navegação **teacherRootCertificates**, **teacherIdentityCertificate**, **studentRootCertificates** e **studentIdentityCertificate** da entidade [iosEducationDeviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration) |
| Alteração      | Beta    | Foi alterado o tipo das seguintes propriedades na entidade [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration):<br/>**deviceStatuses** da coleção [managedDeviceMobileAppProvisioningConfigurationDeviceStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/managedDeviceMobileAppProvisioningConfigurationDeviceStatus) para a coleção [managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus)<br/>**groupAssignments** da coleção [appProvisioningConfigGroupAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/appProvisioningConfigGroupAssignment) para a coleção [mobileAppProvisioningConfigGroupAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileappprovisioningconfiggroupassignment)<br/> |
| Alteração      | Beta    | Foi adicionada a propriedade de navegação **managedDeviceCertificateStates** à entidade [iosScepCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosscepcertificateprofile) |
| Alteração      | Beta    | Foi adicionada a propriedade de navegação **managedDeviceCertificateStates** à entidade [macOSScepCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosscepcertificateprofile) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **deviceConfigurationStates** e **deviceCompliancePolicyStates** à entidade [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_manageddevice) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **deviceStatusSummary** e **userStatusSummary** à entidade [managedDeviceMobileAppConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfiguration) |
| Alteração      | Beta    | Foi adicionada a propriedade de navegação **installSummary** à entidade [mobileApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileapp) |
| Alteração      | Beta    | Foi removida a propriedade de navegação **sideLoadingKeys** da entidade [organization](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_onboarding_organization) |
| Alteração      | Beta    | Foi adicionada a propriedade de navegação **managedDeviceCertificateStates** à entidade [windows81SCEPCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81scepcertificateprofile) |
| Alteração      | Beta    | Foi adicionada a propriedade de navegação **managedDeviceCertificateStates** à entidade [windowsPhone81SCEPCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81scepcertificateprofile) |
| Alteração      | Beta    | Foram removidas as propriedades **applicationId**, **appName**, **platformId**, **userFailures** e **deviceFailures** do tipo complexo [appInstallationFailure](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure) |
| Alteração      | Beta    | Foi adicionada a propriedade **displayName** ao tipo complexo [iosHomeScreenFolderPage](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolderpage) |
| Alteração      | Beta    | Foi adicionada a propriedade **displayName** ao tipo complexo [iosHomeScreenPage](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenpage) |
| Alteração      | Beta    | Foram adicionadas as propriedades **subjectName**, **description**, **expirationDateTime** e **certificate** ao tipo complexo [windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondatarecoverycertificate) |
| Alteração      | Beta    | Foram removidas as propriedades **dataRecoveryCertificate** e **certificateFileName** do tipo complexo [windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_windowsinformationprotectiondatarecoverycertificate) |
| Alteração      | Beta    | Foi adicionada a propriedade **displayName** ao tipo complexo [windowsPackageInformation](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation) |
| Alteração      | Beta    | Foi alterado o tipo das seguintes propriedades no tipo complexo [windowsPackageInformation](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation):<br/>**applicableArchitecture** de [windowsArchitecture](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/windowsArchitecture) para cadeia de caracteres<br/> |
| Alteração      | Beta    | Foram alteradas as seguintes propriedades no tipo complexo [windowsPackageInformation](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation):<br/>**applicableArchitecture** de opcional para obrigatório<br/> |

### <a name="add-contracts-to-microsoft-graph"></a>Adicionar contratos ao Microsoft Graph

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Novo recurso:</br>[contract](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/contract) |

### <a name="add-domain-operations-to-microsoft-graph"></a>Adicionar operações de domínio ao Microsoft Graph

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Adicionou funções nos [domínios](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/domain).<br/>Novas entidades:</br>[domain](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/domain)<br/>[domainDnsRecord](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/domaindnsrecord)<br/>[domainDnsCnameRecord](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/domainDnsCnameRecord)<br/>[domainDnsMxRecord](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/domainDnsMxRecord)<br/>[domainDnsSrvRecord](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/domainDnsSrvRecord)<br/>[domainDnsTxtRecord](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/domainDnsTxtRecord)<br/>[domainDnsUnavailableRecord](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/domainDnsUnavailableRecord)<br/>Novas ações:</br>[forceDelete](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/api/domain_forcedelete)</br>[verify](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/api/domain_verify) |

### <a name="add-custom-data-to-microsoft-graph-using-schema-extensions"></a>Adicionar dados personalizados ao Microsoft Graph usando extensões de esquema

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Estenda o Microsoft Graph com dados de aplicativos usando [extensões de esquema](https://developer.microsoft.com/pt-BR/graph/docs/concepts/extensibility_overview#schema-extensions-preview).  Isso é suportado nos seguintes recursos:<br/>administrative unit<br/>calendar event<br/>device<br/>group<br/>message<br/>organization<br/>personal contact<br/>post<br/>user<br/>Veja o seguinte exemplo:<br/>[Adicionar dados personalizados a grupos usando Extensões do Esquema (visualização)](https://developer.microsoft.com/pt-BR/graph/docs/concepts/extensibility_schema_groups) |
| Adição        | Beta        | Foi fornecido uma maneira alternativa de criar uma definição de extensão do esquema sem a necessidade de um domínio personalizado .com verificado. Consulte [extensões de esquema](https://developer.microsoft.com/pt-BR/graph/docs/concepts/extensibility_overview#schema-extensions-preview) para obter detalhes. |

### <a name="add-custom-data-to-microsoft-graph-using-open-extensions"></a>Adicionar dados personalizados ao Microsoft Graph usando extensões abertas

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Alteração          | v1.0 e beta | As "extensões de dados do Office 365" anteriores foram renomeadas como "abrir extensões". |
| Adição        | Beta          | Foram adicionados recursos que oferecem suporte a [extensões abertas](https://developer.microsoft.com/pt-BR/graph/docs/concepts/extensibility_overview#open-extensions): <br/>administrative unit<br/>device<br/>group<br/>organization<br/>user<br/>Veja o seguinte exemplo:<br/>[Adicionar dados personalizados aos usuários usando extensões abertas (visualização)](https://developer.microsoft.com/pt-BR/graph/docs/concepts/extensibility_open_users) |

### <a name="directory-apis"></a>APIs de diretório

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foi adicionado o suporte para a [restauração e a exclusão permanente de grupos](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/directory).<br/>Nova entidade: diretório com a propriedade de navegação deleteditems. |
| Adição        | Beta        | Nova entidade:</br>[Ponto de extremidade](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/endpoint) |
| Alteração          | Beta        | Nova propriedade de navegação nos [pontos de extremidade](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/api/group_list_endpoints) em [grupos](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/group) |
| Adição        | Beta        | Nova entidade:</br>[licenseDetails](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/licensedetails) |
| Alteração          | Beta        | Nova propriedade de navegação [licensedetails](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/api/user_list_licensedetails) em [users](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/user) |

### <a name="reports-apis"></a>APIs de relatórios

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foi introduzida a nova API de visualização para relatórios do Office 365. Você pode usá-la para obter relatórios de uso sobre como as pessoas em sua empresa estão usando serviços do Office 365. Por exemplo, você pode identificar quem está usando muito um serviço e atingindo cotas, ou quem pode não precisar de uma licença do Office 365. Para obter mais detalhes, consulte o [relatório](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/report). |

### <a name="directory-apis"></a>APIs de diretório

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Nova entidade:</br>[contract](https://graph.microsoft.io/pt-BR/docs/api-reference/beta/resources/contract) |

## <a name="february-2017"></a>Fevereiro de 2017

### <a name="intune-apis"></a>APIs do Intune

| Tipo de alteração | Versão | Descrição                              |
| :---------- | :------ | :--------------------------------------- |
| Adição    | Beta    | Foram adicionadas novas entidades:<br/>[androidForWorkCertificateProfileBase](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkcertificateprofilebase)<br/>[androidForWorkEasEmailProfileBase](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkeasemailprofilebase)<br/>[androidForWorkEnterpriseWiFiConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkenterprisewificonfiguration)<br/>[androidForWorkGmailEasConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkgmaileasconfiguration)<br/>[androidForWorkNineWorkEasConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworknineworkeasconfiguration)<br/>[androidForWorkPkcsCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkpkcscertificateprofile)<br/>[androidForWorkScepCertificateProfile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkscepcertificateprofile)<br/>[androidForWorkTrustedRootCertificate](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworktrustedrootcertificate)<br/>[androidForWorkWiFiConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_androidforworkwificonfiguration)<br/>[appleDeviceFeaturesConfigurationBase](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_appledevicefeaturesconfigurationbase)<br/>[appProvisioningConfigGroupAssignment](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_appprovisioningconfiggroupassignment)<br/>[deviceComplianceUserOverview](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuseroverview)<br/>[deviceConfigurationUserOverview](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuseroverview)<br/>[enterpriseCertificate](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_enterprisecertificate)<br/>[iosEducationDeviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration)<br/>[macOSDeviceFeaturesConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_macosdevicefeaturesconfiguration)<br/>[managedAndroidLobApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_managedandroidlobapp)<br/>[managedDeviceMobileAppProvisioningConfigurationDeviceStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappprovisioningconfigurationdevicestatus)<br/>[managedIOSLobApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_managedioslobapp)<br/>[managedMobileLobApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_managedmobilelobapp)<br/>[symantecCertificate](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_symanteccertificate)<br/>[windowsAppX](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsappx)<br/>[windowsCertificateProfileBase](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowscertificateprofilebase)<br/>[windowsPhone81AppX](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appx)<br/>[windowsPhone81AppXBundle](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsphone81appxbundle)<br/>[windowsPhoneXAP](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsphonexap)<br/>[windowsUniversalAppX](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsuniversalappx)<br/> |
| Adição    | Beta    | Foram adicionados novos tipos complexos:<br/>[airPrintDestination](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_airprintdestination)<br/>[windowsArchitecture](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsarchitecture)<br/>[windowsDeviceType](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsdevicetype)<br/>[windowsMinimumOperatingSystem](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowsminimumoperatingsystem)<br/>[windowsPackageInformation](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_windowspackageinformation)<br/> |
| Adição    | Beta    | Foi adicionada a ação [atribuir](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_apps_ioslobappprovisioningconfiguration_assign) à entidade [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) |
| Adição    | Beta    | Foi adicionada a ação [scheduleActionsForRules](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_deviceconfig_devicecompliancepolicy_scheduleactionsforrules) à entidade [deviceCompliancePolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy) |
| Adição    | Beta    | Foi adicionada a ação [updateTargetedSecurityGroups](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_mam_targetedmanagedappconfiguration_updatetargetedsecuritygroups) à entidade [targetedManagedAppConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) |
| Adição    | Beta    | Foi adicionada função [getScopesForUser](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/intune_rbac_resourceoperation_getscopesforintune_devices_user) à entidade [resourceOperation](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_rbac_resourceoperation) |
| Alteração      | Beta    | Removido a propriedade **manifesto** a partir da entidade [androidLobApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_androidlobapp)  |
| Alteração      | Beta    | Foram adicionadas as propriedades **assetTagTemplate**, **lockScreenFootnote**, **homeScreenDockIcons** e **homeScreenPages** à entidade [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration)  |
| Alteração      | Beta    | Foram removidas as propriedades **deviceSharingAssetTagInformation** **deviceSharingLockScreenFootnote**, **homeScreenLayoutDockIcons** e **homeScreenLayoutPages** da entidade [iosDeviceFeaturesConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration)  |
| Alteração      | Beta    | Foi adicionada a propriedade **appsSingleAppModeBundleIds** à entidade [iosGeneralDeviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosgeneraldeviceconfiguration) |
| Alteração      | Beta    | Foi removida a propriedade **manifesto** da entidade [iosLobApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_ioslobapp) |
| Alteração      | Beta    | Foram adicionadas as propriedades **createdDateTime**, **descrição**, **lastModifiedDateTime**, **displayName** e **versão** à entidade [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) |
| Alteração      | Beta    | Foram adicionadas as propriedades **createdDateTime** e **lastModifiedDateTime** à entidade [managedAppPolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_managedapppolicy)  |
| Alteração      | Beta    | Foi removida a propriedade **deviceRegistrationState** da entidade [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devices_manageddevice) |
| Alteração      | Beta    | Foi adicionada a propriedade **manifesto** à entidade [mobileAppContentFile](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileappcontentfile) |
| Alteração      | Beta    | Foram adicionadas as propriedades **osDescription** e **userName** à entidade [mobileAppInstallStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus) |
| Alteração      | Beta    | Foi removida a propriedade **deviceType** da entidade [mobileAppInstallStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus) |
| Alteração      | Beta    | Foi alterado o tipo das seguintes propriedades na entidade [mobileAppInstallStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileappinstallstatus):<br/>**mobileAppInstallStatusValue** de Int32 para String |
| Alteração      | Beta    | Foram adicionadas as propriedades **targetedSecurityGroupIds** e **targetedSecurityGroupsCount** à entidade [targetedManagedAppConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) entidade |
| Alteração      | Beta    | Foi removida a propriedade **numberOfTargetedSecurityGroups** da entidade [targetedManagedAppConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_targetedmanagedappconfiguration) |
| Alteração      | Beta    | Foi adicionada a propriedade **id** à entidade [user](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_devices_user)  |
| Alteração      | Beta    | Foram removidas as propriedades **renewalThresholdPercentage**, **keyStorageProvider**, **subjectNameFormat**, **subjectAlternativeNameType**, **certificateValidityPeriodValue** e **certificateValidityPeriodScale** da entidade [windows10CertificateProfileBase](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10certificateprofilebase)  |
| Alteração      | Beta    | Foram removidas as propriedades **renewalThresholdPercentage**, **keyStorageProvider**, **subjectNameFormat**, **subjectAlternativeNameType**, **certificateValidityPeriodValue** e **certificateValidityPeriodScale** da entidade [windows81CertificateProfileBase](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows81certificateprofilebase) |
| Alteração      | Beta    | Foi removida a propriedade **applyToWindows10Mobile** da entidade [windowsPhone81GeneralConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsphone81generalconfiguration)  |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **enterpriseCerts**, **iosLobAppProvisioningConfigurations** e **symantecCert** à entidade [deviceAppManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement) |
| Alteração      | Beta    | Foi adicionada a propriedade de navegação **userStatusOverview** à entidade [deviceCompliancePolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy) |
| Alteração      | Beta    | Foi adicionada a propriedade de navegação **userStatusOverview** à entidade [deviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) |
| Alteração      | Beta    | Foram adicionadas as propriedades de navegação **groupAssignments**, **deviceStatuses** e **userStatuses** à entidade [iosLobAppProvisioningConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration) |
| Alteração      | Beta    | Foi alterado o tipo das seguintes propriedades na entidade [windows10VpnConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10vpnconfiguration):<br/>**identityCertificate** de [windows10CertificateProfileBase](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10certificateprofilebase) para [windowsCertificateProfileBase](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowscertificateprofilebase) |
| Alteração      | Beta    | Foram adicionadas as propriedades **deviceComplianceCheckinThresholdDays** e **isScheduledActionEnabled**ao tipo complexo [deviceManagementSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings) |
| Alteração      | Beta    | Foram removidas as propriedades **windowsCommercialId** e **windowsCommercialIdLastModifiedTime** do tipo complexo [deviceManagementSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagementsettings) |
| Alteração      | Beta    | Foram adicionadas as propriedades **bundleID**, **appName**, **publisher**, **habilitado** e **showOnLockScreen** ao tipo complexo [iosNotificationSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings)  |
| Alteração      | Beta    | Foram removidas as propriedades **bundleIdentifier**, **notificationsEnabled** e **showInLockScreen** do tipo complexo [iosNotificationSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings) |



## <a name="january-2017"></a>Janeiro de 2017

### <a name="outlook-calendar"></a>Calendário do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Nova ação [findMeetingTimes](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/user_findmeetingtimes) para o recurso [user](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/user). |
| Adição        | v1.0        | Novo tipo complexo [attendeeBase](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/attendeebase), que consiste em uma propriedade de tipo para o tipo attendee. |
| Adição        | v1.0        | Novos tipos complexos:<br/>[attendeeAvailability](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/attendeeavailability)<br/>[locationConstraint](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/locationconstraint) <br/>[locationConstraintItem](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/locationconstraintitem)<br/>[meetingTimeSuggestion](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/meetingtimesuggestion)<br/>[meetingTimeSuggestionsResult](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/meetingtimesuggestionsresult)<br/>[timeConstraint](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/timeconstraint)<br/>[timeSlot](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/timeslot) |
| Alteração          | v1.0        | O tipo complexo [attendee](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/attendee) agora deriva de attendeeBase,que, por sua vez, é derivado do [recipient](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/recipient). Incluindo as propriedades herdadas, ele consiste nas mesmas propriedades de antes: **status**, **type** e **emailAddress**. |
| Adição        | Beta        | hexColor adicionado ao recurso [calendar](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/calendar). |

### <a name="intune-apis"></a>APIs do Intune

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foram adicionadas novas entidades: <br/>[appReportingOverviewStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_appreportingoverviewstatus)<br/>[deviceComplianceDeviceOverview](https://developer.microsoft.com/pt-BR/graph/docs//api-reference/beta/resources/intune_deviceconfig_devicecompliancedeviceoverview)<br/>[deviceConfigurationDeviceOverview](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdeviceoverview)<br/>[deviceManagementExchangeOnpremisesPolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_onboarding_devicemanagementexchangeonpremisespolicy)<br/>[iosDeviceFeaturesConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosdevicefeaturesconfiguration)<br/>[iosEducationDeviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioseducationdeviceconfiguration)<br/>[iosLobAppProvisioningConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_ioslobappprovisioningconfiguration)<br/>[onpremisesConditionalAccessSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_onboarding_onpremisesconditionalaccesssettings)<br/>[sharedPCConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcconfiguration)<br/>[windows10EnterpriseModernAppManagementConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10enterprisemodernappmanagementconfiguration)<br/>[windows10SecureAssessmentConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10secureassessmentconfiguration)<br/>[windows10WindowsInformationProtectionConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10windowsinformationprotectionconfiguration) |
|Adição|Beta|Foram adicionados novos tipos complexos: <br/> [appInstallationFailure](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_appinstallationfailure)<br/>[enterpriseCloudResource](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_enterprisecloudresource)<br/>[iosHomeScreenApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenapp)<br/>[iosHomeScreenFolder](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolder)<br/>[iosHomeScreenFolderPage](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenfolderpage)<br/>[iosHomeScreenItem](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenitem)<br/>[iosHomeScreenPage](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ioshomescreenpage)<br/>[iosNotificationSettings](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_iosnotificationsettings)<br/>[iPv6Range](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_ipv6range)<br/>[sharedPCAccountManagerPolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_sharedpcaccountmanagerpolicy)<br/>[windowsInformationProtectionAppRule](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionapprule)<br/>[windowsInformationProtectionAppRuleAppLockerPolicyFileTemplate](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruleapplockerpolicyfiletemplate)<br/>[windowsInformationProtectionAppRuleDesktopTemplate](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruledesktoptemplate)<br/>[windowsInformationProtectionAppRuleStoreAppTemplate](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionapprulestoreapptemplate)<br/>[windowsInformationProtectionAppRuleTemplate](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionappruletemplate)<br/>[windowsInformationProtectionCorporateNetworkLocation](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectioncorporatenetworklocation)<br/>[windowsInformationProtectionDataRecoveryCertificate](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectiondatarecoverycertificate)<br/>[windowsInformationProtectionProtectedLocation](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocation)<br/>[windowsInformationProtectionProtectedLocationEnterpriseCloudResources](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterprisecloudresources)<br/>[windowsInformationProtectionProtectedLocationEnterpriseInternalProxyServers](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseinternalproxyservers)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv4Ranges](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseipv4ranges)<br/>[windowsInformationProtectionProtectedLocationEnterpriseIPv6Ranges](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseipv6ranges)<br/>[windowsInformationProtectionProtectedLocationEnterpriseNetworkDomainNames](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterprisenetworkdomainnames)<br/>[windowsInformationProtectionProtectedLocationEnterpriseProxyServers](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationenterpriseproxyservers)<br/>[windowsInformationProtectionProtectedLocationNeutralResources](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windowsinformationprotectionprotectedlocationneutralresources)
|Exclusão|Beta|Removido os seguintes tipos complexos e substituídos por microsoft.graph.Json:<br/>managedAppDeploymentSummary <br/>managedAppSummary<br /> |
|Alteração|Beta|Foi substituído o tipo de propriedade appConfigComplianceStatus por complianceStatus nas seguintes entidades: <br/>[managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus)<br/>[managedDeviceMobileAppConfigurationUserStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationuserstatus)|
|Alteração|Beta|Para o recurso [managedAppStatusRaw](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_managedappstatusraw), foi alterado o tipo de conteúdo de propriedade de managedAppSummary para Json.|
|Alteração|Beta|Foi removida a função getUsersWithFlaggedAppRegistration da coleção [managedAppRegistration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_mam_managedappregistration).|
|Alteração|Beta|Foi alterada a propriedade de navegação **vppToken** da entidade [iosVppApp](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_iosvppapp) para que ela deixasse de ser uma coleção contida.|
|Alteração|Beta|Foi adicionada a propriedade **deviceStatusOverview** às entidades [deviceConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfiguration) e [deviceCompliancePolicy](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancepolicy).|
|Alteração|Beta|Foi adicionada a propriedade **appReportingOverview** ao singleton [deviceAppManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_deviceappmanagement).|
|Alteração|Beta|Foram adicionadas as propriedades **deviceDisplayName** e **userPrincipalName** às entidades [deviceConfigurationDeviceStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationdevicestatus), [deviceComplianceDeviceStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancedevicestatus) e [managedDeviceMobileAppConfigurationDeviceStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationdevicestatus).|
|Alteração|Beta|Foi adicionada a propriedade **ruleName** à entidade [deviceComplianceScheduledActionForRule](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecompliancescheduledactionforrule).|
|Alteração|Beta|Foram adicionadas as propriedades **devicesCount**, **userDisplayName** e **userPrincipalName** às entidades [deviceConfigurationUserStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_deviceconfigurationuserstatus), [deviceComplianceUserStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicecomplianceuserstatus) e [managedDeviceMobileAppConfigurationUserStatus](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_manageddevicemobileappconfigurationuserstatus).|
|Alteração|Beta|Foi adicionada a coleção [notificationMessageTemplates](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_notification_notificationmessagetemplate) ao singleton [deviceManagement](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_devicemanagement).|
|Alteração|Beta|Foram adicionadas as propriedades **isDefault**, **lastModifiedDateTime**, **locale**, **messageTemplate** e **subject** à entidade [localizedNotificationMessage](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_localizednotificationmessage).|
|Alteração|Beta|Foram adicionadas as propriedades **azureActiveDirectoryDeviceId**, **deviceCategory**, **deviceRegistrationState** e **managementAgent** à entidade [managedDevice](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_onboarding_manageddevice).|
|Alteração|Beta|Foi adicionada a propriedade **lastModifiedDateTime** à entidade [mobileAppCategory](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_apps_mobileappcategory).|
|Alteração|Beta|Foram adicionadas as propriedades **brandingOptions**, **defaultLocale**, **displayName**, **fromEmailAddress**, **lastModifiedDateTime**, **localizedNotificationMessages** à entidade [notificationMessageTemplate](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_notification_notificationmessagetemplate).|
|Alteração|Beta|Foram adicionadas as propriedades **appsAllowTrustedAppsSideloading**, **appsBlockWindowsStoreOriginatedApps**, **developerUnlockSetting**, **edgeBlockAccessToAboutFlags**, **edgeBlockDeveloperTools**, **edgeBlockExtensions**, **edgeBlockInPrivateBrowsing**, **edgeFirstRunUrl**, **edgeHomepageUrls**, **gameDvrBlocked**, **settingsBlockAddProvisioningPackage**, **settingsBlockChangeLanguage**, **settingsBlockChangePowerSleep**, ** settingsBlockChangeRegion**, **settingsBlockChangeSystemTime**, **settingsBlockEditDeviceName**, **settingsBlockRemoveProvisioningPackage**, **sharedUserAppDataAllowed**, **smartScreenBlockPromptOverride**, **smartScreenBlockPromptOverrideForFiles**, **storageRestrictAppDataToSystemVolume**, **storageRestrictAppInstallToSystemVolume**, **webRtcBlockLocalhostIpAddress**, **windowsStoreBlockAutoUpdate** e **windowsStoreEnablePrivateStoreOnly** à entidade [windows10GeneralConfiguration](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_deviceconfig_windows10generalconfiguration).|

## <a name="december-2016"></a>Dezembro de 2016

### <a name="delta-query"></a>Consulta delta

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Adicionar uma nova função delta para as seguintes entidades realizem [consulta delta](https://developer.microsoft.com/pt-BR/graph/docs/concepts/delta_query_overview):<br/>contato<br/>contactFolder<br/>event<br/>group<br/>mailFolder<br/>message<br/>user<br/>Confira os seguintes exemplos:<br/>[Obter as alterações incrementais para grupos (visualização)](https://developer.microsoft.com/pt-BR/graph/docs/concepts/delta_query_groups)<br/>[Obter as alterações incrementais para as mensagens em uma pasta (visualização)](https://developer.microsoft.com/pt-BR/graph/docs/concepts/delta_query_messages)<br/>[Obter as alterações incrementais para usuários (visualização)](https://developer.microsoft.com/pt-BR/graph/docs/concepts/delta_query_users) |

### <a name="excel-apis"></a>APIs do Excel

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Foi adicionado o recurso workbookPivotTable, as ações refresh e refreshAll a Tabelas Dinâmicas, o recurso workbookRangeView, a ação visibleView ao intervalo filtrado para retornar workbookRangeView para o usuário, extrair coleção de linhas e recurso de intervalo de visibleView, columnsAfter, columnsBefore, resizedRange, rowsAbove, e funções rowsBelow do recurso de intervalo, e novas propriedades de tabela. |

### <a name="intune-apis"></a>APIs do Intune

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Recursos adicionados e APIs de método para o Microsoft Intune. Este é um conjunto de recursos e métodos para dar suporte à visualização pública de Intune no Portal do Azure. Para saber mais sobre o serviço do Intune, veja a [documentação do Intune ](https://go.microsoft.com/fwlink/?linkid=836405). Para saber mais sobre os recursos do Intune e APIs, veja [Trabalho com o Intune no Microsoft Graph](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/intune_graph_overview). |

## <a name="october-2016"></a>Outubro de 2016

### <a name="authorization-provider"></a>Provedor de autorização

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0 e beta | O ponto de extremidade de autenticação v2.0 agora dá suporte à concessão do OAuth client_credentials, que pode ser usada para [daemon e processos com execução longa em cenários de negócios](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-v2-protocols-oauth-client-creds/). |
| Adição        | v1.0 e beta | O ponto de extremidade de autenticação v2.0 agora dá suporte a [escopos de permissão que exigem consentimento do administrador](http://developer.microsoft.com/pt-BR/graph/docs/concepts/permissions_reference), por meio do [ponto de extremidade de consentimento de administração](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-v2-scopes/#admin-restricted-scopes). |
| Adição        | v1.0 e beta | O ponto de extremidade de autenticação v2.0 agora dá suporte ao consentimento administrativo para todos os usuários de um locatário, por meio do [ponto de extremidade de consentimento de administração](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-v2-scopes/#admin-restricted-scopes). |

### <a name="invitation-apis"></a>APIs de convite

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foi adicionada a propriedade invitedUserType ao tipo de entidade de convite, que define o tipo de usuário (**Convidado** ou **Membro**) que é convidado. |
| Exclusão        | Beta        | Removeremos a propriedade invitedToGroups do tipo de entidade de convite em 11/11/2016. Isso significa que você não poderá mais adicionar um usuário convidado a um grupo usando essa API. Em vez disso, use a [API adicionar membro](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/api/group_post_members) para adicionar um usuário a um grupo. |

## <a name="september-2016"></a>Setembro de 2016

### <a name="azure-ad-application-proxy"></a>Proxy de aplicativo do Azure AD

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | O as APIs de Proxy de Aplicativo do Azure AD agora estão disponíveis nos pontos de extremidade beta do Microsoft Graph. Essas APIs permitem publicações seguras de aplicativos locais para usuários fora da rede corporativa que estejam usando o Azure AD como o plano de controle comum para acesso. Você pode usar as APIs publicadas para gravar os aplicativos que podem recuperar e atualizar diversos aspectos do proxy de aplicativo, como as configurações _conectores_, _connectorGroups_ e _onPremisesPublishing_ de um aplicativo. |

### <a name="drive"></a>Unidade

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foi adicionada a coleção _shared_ para permitir o acesso aos driveItems compartilhados pela URL shareId ou sharing. |
| Adição        | Beta        | Foi adicionada a função _search_ a uma unidade, o que permite pesquisar mais itens do que apenas aqueles que constam na pasta raiz da unidade. |


### <a name="driveitem"></a>DriveItem

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Suporte adicional para _createUploadSession_, o que permite carregar arquivos com mais de 4 MB no OneDrive, no OneDrive for Business e em bibliotecas de documentos do SharePoint. |
| Adição        | Beta        | Foi adicionada a propriedade _sharepointIds_ ao driveItem que retorna identificadores de API do SharePoint tradicionais para driveItems armazenados no SharePoint. |
| Adição        | Beta        | Outras propriedades foram adicionadas ao _remoteItem_. |
| Adição        | Beta        | Foi adicionado o valor _quickXorHash_ aos arquivos no OneDrive for Business. |
| Adição        | Beta        | O escopo para _createSharingLink_ foi adicionado para permitir a criação de links compartilháveis da empresa ou links de compartilhamento anônimos. |

### <a name="extended-properties"></a>Propriedades estendidas

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | As [propriedades estendidas](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/extended-properties-overview) agora são compatíveis com os seguintes recursos:message, mailFolder, event, calendar, contact, contactFolder, group event, group calendar, group post. |

### <a name="groups"></a>Grupos

Suporte adicionado para a associação de grupo dinâmico através de visualização pública API, incluindo as adições listados na tabela a seguir.

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foi adicionada a propriedade **membershipRule** que contém regras de controle das associações a esse grupo, se o grupo for um grupo dinâmico |
| Adição        | Beta        | Foi adicionada a propriedade **membershipRuleProcessingState** para controlar se o processamento de associação dinâmica está ativado ou pausado para esse grupo. |
| Adição        | Beta        | Defina a propriedade **groupTypes** para conter **"DynamicMembership"** a fim de ativar o recurso de grupos dinâmicos para esse grupo. |
| Adição        | Beta        | Foi adicionada a propriedade **preferredLanguage** para indicar o idioma de preferência para um grupo do Office 365. |
| Adição        | Beta        | Foi adicionada propriedade **theme** para especificar o tema da cor de um grupo do Office 365. |

### <a name="hybrid-deployment-support"></a>Suporte à implantação híbrida

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Os aplicativos podem usar a versão 1.0 das APIs de Email, Calendário e Contatos do Outlook para acessar caixas de correio locais em uma implantação híbrida com a Atualização Cumulativa 3 (CU3) do Exchange 2016. Veja mais detalhes sobre o suporte à API REST em [implantações híbridas](https://developer.microsoft.com/pt-BR/graph/docs/overview/hybrid_rest_support) específicas. **Observação:** se você estiver usando os conjuntos da API na versão 1.0, agora é possível que seus aplicativos, incluindo aplicativos de produção, funcionem com caixas de correio locais que atendam a requisitos de implantação híbrida específicos. Esse recurso só está disponível na visualização. |

### <a name="identityriskevents"></a>IdentityRiskEvents

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | Como parte da alteração de esquema em que o tipo de duas propriedades de local está sendo substituído por um novo tipo complexo no ponto de extremidade identityRiskEvents, as seguintes propriedades são alteradas/adicionadas no ponto de extremidade identityRiskEvents:</br>**location**  alterado de Edm.String para ComplexType signInLocation.<br/>**previousLocation** alterado de Edm.String para ComplexType signInLocation.<br/>**signInLocation** novo ComplexType que contém as propriedades city, state, countryOrRegion e geoCoordinates.<br/>**geoCoordinates** novo ComplexType que contém as propriedades latitude e longitude. |

### <a name="invitation-manager"></a>Gerenciador de convites

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | As APIs do gerenciador de convites agora estão disponíveis nos pontos de extremidade do Microsoft Graph na versão Beta. Você pode usar as APIs do gerenciador de convites para que o gerenciador de convites crie um convite para adicionar um usuário externo à organização. Como parte do convite, você também pode optar por adicionar o usuário convidado a um grupo do Office 365. Para obter mais detalhes, veja [gerenciador de convite](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/invitation). |

### <a name="onedrive"></a>OneDrive

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Foi adicionado o método **CreateUploadSession** ao **driveItem**, que permite arquivos grandes e carregamentos retomáveis. |
| Adição        | v1.0        | Foram adicionadas as propriedades para rastrear as IDs do SharePoint em itens do SharePoint (**sharepointIds**) e uma propriedade para identificar pastas-raiz (**root**). |
| Adição        | v1.0        | Foi adicionado o conjunto-raiz **Shares**, que pode ser usado com shareIds ou links de compartilhamento para acessar itens compartilhados no OneDrive e no SharePoint. Retorna um novo tipo, sharedDriveItem. |
| Adição        | v1.0        | Foi adicionado o método**Invite** ao driveItem, que permite adicionar permissões a itens. |
| Adição        | v1.0        | Foi adicionado o método **Search** à unidade, que permite pesquisar itens na unidade e itens compartilhados. |
| Adição        | v1.0        | Foi adicionada a propriedade **processingMetadata** à propriedade quickXorHash do tipo complexo no tipo complexo hashes. |
| Adição        | v1.0        | Foi adicionada a propriedade **quickXorHash** ao tipo complexo hashes. |

### <a name="outlook-calendar"></a>Calendário do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Foi adicionada a propriedade **onlineMeetingUrl** ao recurso [event](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/event). |
| Adição        | Beta        | Foi adicionada a ação [forward](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/event_forward) ao recurso event. |
| Adição        | Beta        | Foram adicionadas as propriedades ao recurso [calendar](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/calendar) para dar suporte ao compartilhamento de calendários: **canEdit**, **canShare**, **canViewPrivateItems**, **isShared**, **isShareWithMe** e **owner**. |

### <a name="outlook-mail"></a>Email do Outlook

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Foi adicionado o tipo complexo [mailboxSettings](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/mailboxsettings), que inclui as propriedades **automaticRepliesSetting**, **timeZone** e **language**. |
| Adição        | v1.0        | Foi adicionada a propriedade **mailboxSettings** ao recurso [user](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/v1.0/resources/user). |
| Adição        | Beta        | Foi adicionado o suporte para criar, listar, obter e excluir uma ou mais instâncias de [mencionar](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/mention) em uma mensagem. As menções dão suporte a chamadas para chamar a atenção dos outros usuários em uma mensagem. |
| Adição        | Beta        | Foi adicionado suporte para a ação [getMailTips](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/user_getmailtips) para obter Dicas de Email para destinatários específicos. Foram adicionados os seguintes recursos: automaticRepliesMailTips, mailTips, mailTipsError. |

### <a name="query-parameters"></a>Parâmetros de consulta

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | Os prefixos de parâmetros de consulta sem $ são suportados a partir de 26/09/16. O prefixo $ nos parâmetros de consulta é opcional. Para obter mais detalhes, confira [Suporte a parâmetros da consulta sem prefixos $ no post do blog do Microsoft Graph](http://dev.office.com/queryparametersinMicrosoftGraph). |

### <a name="sharepoint"></a>SharePoint

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Acesso a sites do SharePoint e [listas por ID](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/list_get) ou [caminho/URL](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/api/baseitem_getbyurl) |
| Adição        | Beta        | Suporte para [listar, criar, obter e excluir instâncias de listItem](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/listitem). |

### <a name="users"></a>Usuários

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Foi adicionada a propriedade somente leitura para **refreshTokensValidFromDateTime** para indicar quando os tokens de sessão e de atualização são válidos. Qualquer token emitido antes desse momento será inválido, e qualquer tentativa de usá-lo forçará uma nova entrada do usuário. |
| Adição        | Beta        | Foi adicionada a propriedade **showInAddressList** para você controlar se a lista de endereços global do Outlook deve conter este usuário. |
| Adição        | Beta        | Foi adicionada a ação de serviço **invalidateAllRefreshTokens** que invalida todos os tokens de sessão e de atualização do usuário emitidos para aplicativos, redefinindo a propriedade do usuário **refreshTokensValidFromDateTime** para a data e a hora atuais. |


### <a name="webhooks"></a>Webhooks

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Os itens de raiz de unidade adicionados aos Webhooks como um recurso que está disponível para se inscrever. |

## <a name="august-2016"></a>Agosto de 2016

### <a name="contacts"></a>Contatos

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Como parte da mudança do esquema onde algumas propriedades estão sendo removidas e conjuntos de correspondentes estão sendo adicionados ao ponto de extremidade de contatos, as seguintes propriedades foram adicionadas ao ponto de extremidade de contatos: _Websites Collection(ComplexType: Website)_,_Phones Collection (ComplexType: Phone)_, _PostalAddress Collection(ComplexType: PhysicalAddress)_. Para obter detalhes, veja a postagem de blog [Upcoming changes to Contacts and People APIs](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/) (Futuras alterações nas APIs de Contatos e Pessoas). |
| Exclusão        | Beta        | Como parte da mudança do esquema onde algumas propriedades estão sendo removidas e conjuntos de correspondentes estão sendo adicionados ao ponto de extremidade de contatos, as seguintes propriedades foram removidas do ponto de extremidade de contatos: _BusinessHomePage_,_HomePhones_, _MobilePhone1_, _BusinessPhones_, _HomeAddress_, _BusinessAddress_, _OtherAddress_. Para obter detalhes, veja a postagem de blog [Upcoming changes to Contacts and People APIs](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/) (Futuras alterações nas APIs de Contatos e Pessoas). |

### <a name="excel-apis"></a>APIs do Excel

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | v1.0        | Em geral, a API REST do Excel no Microsoft Graph está disponível. Agora, você pode criar integrações avançadas e profundas com pastas de trabalho do Excel no Office 365. Consulte o [Turbine seus aplicativos com a nova API REST do Excel no Microsoft Graph](http://dev.office.com/blogs/power-your-apps-with-the-new-excel-rest-api) na postagem do blog para obter mais detalhes. |

### <a name="people"></a>Pessoas

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Alteração          | Beta        | A propriedade _WebSite_ será renomeada como _WebSite_. Para obter detalhes, veja [Futuras Alterações nas APIs de Contatos e Pessoas](https://blogs.msdn.microsoft.com/exchangedev/2016/06/09/upcoming-changes-to-contacts-and-people-apis/). |

### <a name="privileged-identity-management"></a>Privileged Identity Management

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | As APIs REST de Privileged Identity Management (PIM) agora estão disponíveis no ponto de extremidade beta do Microsoft Graph. O [Privileged Identity Management](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-privileged-identity-management-configure/) fornece ativação "just in time" para funções organizacionais privilegiadas do Azure AD, como Administrador Global, Administrador de Cobrança, etc. As APIs publicadas permitem que os desenvolvedores criem aplicativos que recuperem e atualizem as atribuições de funções privilegiadas e ativem usuários em funções. Para obter detalhes, veja [Microsoft Graph: APIs de Pré-Visualização do Azure AD Privileged Identity Management disponíveis na versão Beta](http://dev.office.com/blogs/microsoft-graph-azure-ad-privileged-identity-management-apis-beta) e o [Azure AD Privileged Identity Management](https://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/privilegedidentitymanagement_root). |

## <a name="july-2016"></a>Julho de 2016

### <a name="administrative-units"></a>Unidades administrativas

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Introduziu a nova API de pré-visualização das Unidades Administrativas. As unidades administrativas permitem às organizações subdividir seu Azure Active Directory e delegar tarefas administrativas a essas subdivisões. As subdivisões podem representar regiões, departamentos, centros de custo etc. Agora, isso pode ser gerenciado por meio da API do Microsoft Graph. |

## <a name="june-2016"></a>Junho de 2016

### <a name="identityriskevents"></a>IdentityRiskEvents

|**Tipo de alteração**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Adição|Beta|Introduziu a nova API de visualização de IdentityRiskEvents. Essa API funciona em conjunto com o Azure Active Directory Identity Protection. É possível utilizá-la para consultar eventos de risco gerados pelo Identity Protection. Para obter mais detalhes, veja a [Introdução de uma nova API de visualização do Microsoft Graph: Postagem do blog ](http://dev.office.com/blogs/identityriskevents-api-preview)IdentityRiskEvents

### <a name="subscriptions"></a>Assinaturas

| **Tipo de alteração** | **Versão** | **Descrição**                          |
| :-------------- | :---------- | :--------------------------------------- |
| Adição        | Beta        | Os escopos somente aplicativo agora têm suporte para assinaturas de _email_ e _contatos_. |

## <a name="may-2016"></a>Maio de 2016

### <a name="calendar"></a>Calendário

|**Tipo de alteração**|**Versão**|**Descrição**|
|:--------------|:-----------|:--------------|
|Alteração significativa|Beta|Alterações na API findMeetingTimes. Para saber mais, veja a postagem de blog para a [ atualização da API findMeetingTimes do Microsoft Graph](http://dev.office.com/microsoft-graph-findmeetingtimes-api-update). Essa alteração entrou em vigor em 19 de maio de 2016.

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
| Adição        | Beta          | Foi adicionado suporte para o segmento de conversão no caminho de expansão. Por exemplo, 'https://graph.microsoft.com/v1.0/me/messages?$expand=microsoft.graph.eventMessage/event'. |

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
| Adição        | Beta        | Estamos adicionando novas APIs REST do Excel que permitem a leitura e a modificação de dados em uma pasta de trabalho do Excel. Agora é possível criar aplicativos inteligentes que permitem que os usuários obtenham valor do conteúdo armazenado em uma pasta de trabalho do Excel, fornecendo informações aos dados. Aproveite o potencial analítico do Excel, crie tabelas e gráficos e extraia imagens do gráfico visualmente atraentes - tudo isso a partir do seu aplicativo. Para obter mais detalhes, veja [Trabalhando com o Excel no Microsoft Graph](http://developer.microsoft.com/pt-BR/graph/docs/api-reference/beta/resources/excel). |

### <a name="general"></a>Geral

| **Tipo de alteração** | **Versão**   | **Descrição**                          |
| :-------------- | :------------ | :--------------------------------------- |
| Adição        | v1.0 e beta | Melhorar mensagens de erro ao resolver tokens JWT (AAD) rejeitados e alias do locatário. |
| Adição        | v1.0 e beta | A localização do ponto de extremidade do serviço de autorização agora é retornada no cabeçalho _www-authenticate_ quando uma solicitação é recebida com um token de portador vazio. |
| Adição        | v1.0 e beta | A capacidade de filtrar na propriedade de id da entidade já está corrigida. Exemplo: GET https://graph.microsoft.com/v1.0/users?$filter=id+eq+'x'<br/>Antes, qualquer solicitação POST para ações de serviço e funções exigia a prefixação do nome da função ou ação com o prefixo microsoft.graph. Por exemplo: POST https://graph.microsoft.com/v1.0/me/Microsoft.Graph.getMemberGroups<br/>Agora, o prefixo não é mais necessário (embora ele ainda possa ser especificado). Portanto, o seguinte também funcionará agora: POST https://graph.microsoft.com/v1.0/me/getMemberGroups |
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
| Adição        | v1.0 e beta | A propriedade _internetMessageId_ foi adicionada. A ID da mensagem no formato especificado por [RFC2822](http://www.ietf.org/rfc/rfc2822.txt). |
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
| Adição        | Beta        | validação de notificationUrl na criação da assinatura. Para obter detalhes, veja [Microsoft Graph WebHooks Update - janeiro de 2016](http://dev.office.com/blogs/Microsoft-Graph-WebHooks-Update-January-2016). |
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
