---
title: Obter androidDeviceOwnerGeneralDeviceConfiguration
description: Leia as propriedades e as relações do objeto androidDeviceOwnerGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f152ae3341605525bda34b67e51e6d357d039b71
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793126"
---
# <a name="get-androiddeviceownergeneraldeviceconfiguration"></a><span data-ttu-id="d5afe-103">Obter androidDeviceOwnerGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d5afe-103">Get androidDeviceOwnerGeneralDeviceConfiguration</span></span>

<span data-ttu-id="d5afe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5afe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5afe-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d5afe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5afe-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5afe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5afe-107">Leia as propriedades e as relações do objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="d5afe-107">Read properties and relationships of the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5afe-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d5afe-108">Prerequisites</span></span>
<span data-ttu-id="d5afe-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="d5afe-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="d5afe-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d5afe-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5afe-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d5afe-111">Permission type</span></span>|<span data-ttu-id="d5afe-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d5afe-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5afe-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d5afe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d5afe-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5afe-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d5afe-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d5afe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5afe-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d5afe-116">Not supported.</span></span>|
|<span data-ttu-id="d5afe-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d5afe-117">Application</span></span>|<span data-ttu-id="d5afe-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5afe-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5afe-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d5afe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d5afe-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d5afe-120">Optional query parameters</span></span>
<span data-ttu-id="d5afe-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d5afe-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5afe-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d5afe-122">Request headers</span></span>
|<span data-ttu-id="d5afe-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d5afe-123">Header</span></span>|<span data-ttu-id="d5afe-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d5afe-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5afe-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d5afe-125">Authorization</span></span>|<span data-ttu-id="d5afe-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d5afe-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5afe-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d5afe-127">Accept</span></span>|<span data-ttu-id="d5afe-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d5afe-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5afe-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d5afe-129">Request body</span></span>
<span data-ttu-id="d5afe-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d5afe-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5afe-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5afe-131">Response</span></span>
<span data-ttu-id="d5afe-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d5afe-132">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5afe-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d5afe-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5afe-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d5afe-134">Request</span></span>
<span data-ttu-id="d5afe-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d5afe-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d5afe-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d5afe-136">Response</span></span>
<span data-ttu-id="d5afe-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="d5afe-137">Here is an example of the response.</span></span> <span data-ttu-id="d5afe-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="d5afe-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="d5afe-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="d5afe-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5491

{
  "value": {
    "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
    "id": "edad943d-943d-edad-3d94-aded3d94aded",
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
    "accountsBlockModification": true,
    "appsAllowInstallFromUnknownSources": true,
    "appsAutoUpdatePolicy": "userChoice",
    "appsDefaultPermissionPolicy": "prompt",
    "appsRecommendSkippingFirstUseHints": true,
    "bluetoothBlockConfiguration": true,
    "bluetoothBlockContactSharing": true,
    "cameraBlocked": true,
    "cellularBlockWiFiTethering": true,
    "certificateCredentialConfigurationDisabled": true,
    "microsoftLauncherConfigurationEnabled": true,
    "microsoftLauncherCustomWallpaperEnabled": true,
    "microsoftLauncherCustomWallpaperImageUrl": "https://example.com/microsoftLauncherCustomWallpaperImageUrl/",
    "microsoftLauncherCustomWallpaperAllowUserModification": true,
    "microsoftLauncherFeedEnabled": true,
    "microsoftLauncherFeedAllowUserModification": true,
    "microsoftLauncherDockPresenceConfiguration": "show",
    "microsoftLauncherDockPresenceAllowUserModification": true,
    "microsoftLauncherSearchBarPlacementConfiguration": "top",
    "microsoftLauncherSearchBarPlacementAllowUserModification": true,
    "enrollmentProfile": "dedicatedDevice",
    "dataRoamingBlocked": true,
    "dateTimeConfigurationBlocked": true,
    "factoryResetDeviceAdministratorEmails": [
      "Factory Reset Device Administrator Emails value"
    ],
    "factoryResetBlocked": true,
    "globalProxy": {
      "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
      "proxyAutoConfigURL": "Proxy Auto Config URL value"
    },
    "googleAccountsBlocked": true,
    "kioskModeScreenSaverConfigurationEnabled": true,
    "kioskModeScreenSaverImageUrl": "https://example.com/kioskModeScreenSaverImageUrl/",
    "kioskModeScreenSaverDisplayTimeInSeconds": 8,
    "kioskModeScreenSaverStartDelayInSeconds": 7,
    "kioskModeScreenSaverDetectMediaDisabled": true,
    "kioskModeApps": [
      {
        "@odata.type": "microsoft.graph.appListItem",
        "name": "Name value",
        "publisher": "Publisher value",
        "appStoreUrl": "https://example.com/appStoreUrl/",
        "appId": "App Id value"
      }
    ],
    "kioskModeWallpaperUrl": "https://example.com/kioskModeWallpaperUrl/",
    "kioskModeExitCode": "Kiosk Mode Exit Code value",
    "kioskModeVirtualHomeButtonEnabled": true,
    "kioskModeVirtualHomeButtonType": "swipeUp",
    "kioskModeBluetoothConfigurationEnabled": true,
    "kioskModeWiFiConfigurationEnabled": true,
    "kioskModeFlashlightConfigurationEnabled": true,
    "kioskModeMediaVolumeConfigurationEnabled": true,
    "microphoneForceMute": true,
    "networkEscapeHatchAllowed": true,
    "nfcBlockOutgoingBeam": true,
    "passwordBlockKeyguard": true,
    "passwordBlockKeyguardFeatures": [
      "camera"
    ],
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinimumLetterCharacters": 15,
    "passwordMinimumLowerCaseCharacters": 2,
    "passwordMinimumNonLetterCharacters": 2,
    "passwordMinimumNumericCharacters": 0,
    "passwordMinimumSymbolCharacters": 15,
    "passwordMinimumUpperCaseCharacters": 2,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordPreviousPasswordCountToBlock": 4,
    "passwordRequiredType": "required",
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "playStoreMode": "allowList",
    "safeBootBlocked": true,
    "screenCaptureBlocked": true,
    "securityAllowDebuggingFeatures": true,
    "securityRequireVerifyApps": true,
    "statusBarBlocked": true,
    "stayOnModes": [
      "ac"
    ],
    "storageAllowUsb": true,
    "storageBlockExternalMedia": true,
    "storageBlockUsbFileTransfer": true,
    "systemUpdateWindowStartMinutesAfterMidnight": 11,
    "systemUpdateWindowEndMinutesAfterMidnight": 9,
    "systemUpdateInstallType": "postpone",
    "systemWindowsBlocked": true,
    "usersBlockAdd": true,
    "usersBlockRemove": true,
    "volumeBlockAdjustment": true,
    "vpnAlwaysOnLockdownMode": true,
    "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
    "wifiBlockEditConfigurations": true,
    "wifiBlockEditPolicyDefinedConfigurations": true
  }
}
```



