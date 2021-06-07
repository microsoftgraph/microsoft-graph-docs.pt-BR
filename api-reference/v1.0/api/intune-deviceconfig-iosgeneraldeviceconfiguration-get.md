---
title: Get iosGeneralDeviceConfiguration
description: Ler propriedades e relações do objeto iosGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a346f34c6c9f48cbe05bb21009b368b6f8f63de1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757070"
---
# <a name="get-iosgeneraldeviceconfiguration"></a><span data-ttu-id="d968b-103">Get iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d968b-103">Get iosGeneralDeviceConfiguration</span></span>

<span data-ttu-id="d968b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d968b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d968b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d968b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d968b-106">Ler propriedades e relações do objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d968b-106">Read properties and relationships of the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d968b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d968b-107">Prerequisites</span></span>
<span data-ttu-id="d968b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d968b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d968b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d968b-110">Permission type</span></span>|<span data-ttu-id="d968b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d968b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d968b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d968b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d968b-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d968b-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d968b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d968b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d968b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d968b-115">Not supported.</span></span>|
|<span data-ttu-id="d968b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d968b-116">Application</span></span>|<span data-ttu-id="d968b-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d968b-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d968b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d968b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d968b-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d968b-119">Optional query parameters</span></span>
<span data-ttu-id="d968b-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d968b-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d968b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d968b-121">Request headers</span></span>
|<span data-ttu-id="d968b-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d968b-122">Header</span></span>|<span data-ttu-id="d968b-123">Valor</span><span class="sxs-lookup"><span data-stu-id="d968b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d968b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="d968b-124">Authorization</span></span>|<span data-ttu-id="d968b-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d968b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d968b-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d968b-126">Accept</span></span>|<span data-ttu-id="d968b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d968b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d968b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d968b-128">Request body</span></span>
<span data-ttu-id="d968b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d968b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d968b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d968b-130">Response</span></span>
<span data-ttu-id="d968b-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d968b-131">If successful, this method returns a `200 OK` response code and [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d968b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d968b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d968b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d968b-133">Request</span></span>
<span data-ttu-id="d968b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d968b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d968b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="d968b-135">Response</span></span>
<span data-ttu-id="d968b-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d968b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8470

{
  "value": {
    "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
    "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "accountBlockModification": true,
    "activationLockAllowWhenSupervised": true,
    "airDropBlocked": true,
    "airDropForceUnmanagedDropTarget": true,
    "airPlayForcePairingPasswordForOutgoingRequests": true,
    "appleWatchBlockPairing": true,
    "appleWatchForceWristDetection": true,
    "appleNewsBlocked": true,
    "appsSingleAppModeList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "appsVisibilityList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "appsVisibilityListType": "appsInListCompliant",
    "appStoreBlockAutomaticDownloads": true,
    "appStoreBlocked": true,
    "appStoreBlockInAppPurchases": true,
    "appStoreBlockUIAppInstallation": true,
    "appStoreRequirePassword": true,
    "bluetoothBlockModification": true,
    "cameraBlocked": true,
    "cellularBlockDataRoaming": true,
    "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
    "cellularBlockPerAppDataModification": true,
    "cellularBlockPersonalHotspot": true,
    "cellularBlockVoiceRoaming": true,
    "certificatesBlockUntrustedTlsCertificates": true,
    "classroomAppBlockRemoteScreenObservation": true,
    "classroomAppForceUnpromptedScreenObservation": true,
    "compliantAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "compliantAppListType": "appsInListCompliant",
    "configurationProfileBlockChanges": true,
    "definitionLookupBlocked": true,
    "deviceBlockEnableRestrictions": true,
    "deviceBlockEraseContentAndSettings": true,
    "deviceBlockNameModification": true,
    "diagnosticDataBlockSubmission": true,
    "diagnosticDataBlockSubmissionModification": true,
    "documentsBlockManagedDocumentsInUnmanagedApps": true,
    "documentsBlockUnmanagedDocumentsInManagedApps": true,
    "emailInDomainSuffixes": [
      "Email In Domain Suffixes value"
    ],
    "enterpriseAppBlockTrust": true,
    "enterpriseAppBlockTrustModification": true,
    "faceTimeBlocked": true,
    "findMyFriendsBlocked": true,
    "gamingBlockGameCenterFriends": true,
    "gamingBlockMultiplayer": true,
    "gameCenterBlocked": true,
    "hostPairingBlocked": true,
    "iBooksStoreBlocked": true,
    "iBooksStoreBlockErotica": true,
    "iCloudBlockActivityContinuation": true,
    "iCloudBlockBackup": true,
    "iCloudBlockDocumentSync": true,
    "iCloudBlockManagedAppsSync": true,
    "iCloudBlockPhotoLibrary": true,
    "iCloudBlockPhotoStreamSync": true,
    "iCloudBlockSharedPhotoStream": true,
    "iCloudRequireEncryptedBackup": true,
    "iTunesBlockExplicitContent": true,
    "iTunesBlockMusicService": true,
    "iTunesBlockRadio": true,
    "keyboardBlockAutoCorrect": true,
    "keyboardBlockDictation": true,
    "keyboardBlockPredictive": true,
    "keyboardBlockShortcuts": true,
    "keyboardBlockSpellCheck": true,
    "kioskModeAllowAssistiveSpeak": true,
    "kioskModeAllowAssistiveTouchSettings": true,
    "kioskModeAllowAutoLock": true,
    "kioskModeAllowColorInversionSettings": true,
    "kioskModeAllowRingerSwitch": true,
    "kioskModeAllowScreenRotation": true,
    "kioskModeAllowSleepButton": true,
    "kioskModeAllowTouchscreen": true,
    "kioskModeAllowVoiceOverSettings": true,
    "kioskModeAllowVolumeButtons": true,
    "kioskModeAllowZoomSettings": true,
    "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
    "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
    "kioskModeRequireAssistiveTouch": true,
    "kioskModeRequireColorInversion": true,
    "kioskModeRequireMonoAudio": true,
    "kioskModeRequireVoiceOver": true,
    "kioskModeRequireZoom": true,
    "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
    "lockScreenBlockControlCenter": true,
    "lockScreenBlockNotificationView": true,
    "lockScreenBlockPassbook": true,
    "lockScreenBlockTodayView": true,
    "mediaContentRatingAustralia": {
      "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingCanada": {
      "@odata.type": "microsoft.graph.mediaContentRatingCanada",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingFrance": {
      "@odata.type": "microsoft.graph.mediaContentRatingFrance",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingGermany": {
      "@odata.type": "microsoft.graph.mediaContentRatingGermany",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingIreland": {
      "@odata.type": "microsoft.graph.mediaContentRatingIreland",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingJapan": {
      "@odata.type": "microsoft.graph.mediaContentRatingJapan",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingNewZealand": {
      "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingUnitedKingdom": {
      "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "mediaContentRatingUnitedStates": {
      "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
      "movieRating": "allBlocked",
      "tvRating": "allBlocked"
    },
    "networkUsageRules": [
      {
        "@odata.type": "microsoft.graph.iosNetworkUsageRule",
        "managedApps": [
          {
            "@odata.type": "microsoft.graph.appListItem",
            "name": "Name value",
            "publisher": "Publisher value",
            "appStoreUrl": "https://example.com/appStoreUrl/",
            "appId": "App Id value"
          }
        ],
        "cellularDataBlockWhenRoaming": true,
        "cellularDataBlocked": true
      }
    ],
    "mediaContentRatingApps": "allBlocked",
    "messagesBlocked": true,
    "notificationsBlockSettingsModification": true,
    "passcodeBlockFingerprintUnlock": true,
    "passcodeBlockFingerprintModification": true,
    "passcodeBlockModification": true,
    "passcodeBlockSimple": true,
    "passcodeExpirationDays": 6,
    "passcodeMinimumLength": 5,
    "passcodeMinutesOfInactivityBeforeLock": 5,
    "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
    "passcodeMinimumCharacterSetCount": 0,
    "passcodePreviousPasscodeBlockCount": 2,
    "passcodeSignInFailureCountBeforeWipe": 4,
    "passcodeRequiredType": "alphanumeric",
    "passcodeRequired": true,
    "podcastsBlocked": true,
    "safariBlockAutofill": true,
    "safariBlockJavaScript": true,
    "safariBlockPopups": true,
    "safariBlocked": true,
    "safariCookieSettings": "blockAlways",
    "safariManagedDomains": [
      "Safari Managed Domains value"
    ],
    "safariPasswordAutoFillDomains": [
      "Safari Password Auto Fill Domains value"
    ],
    "safariRequireFraudWarning": true,
    "screenCaptureBlocked": true,
    "siriBlocked": true,
    "siriBlockedWhenLocked": true,
    "siriBlockUserGeneratedContent": true,
    "siriRequireProfanityFilter": true,
    "spotlightBlockInternetResults": true,
    "voiceDialingBlocked": true,
    "wallpaperBlockModification": true,
    "wiFiConnectOnlyToConfiguredNetworks": true
  }
}
```




