---
title: Listar androidDeviceOwnerGeneralDeviceConfigurations
description: Listar Propriedades e relações dos objetos androidDeviceOwnerGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c190b2a3eb2342dd758d506222b9b2ff5f2b85de
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35958120"
---
# <a name="list-androiddeviceownergeneraldeviceconfigurations"></a><span data-ttu-id="63dbb-103">Listar androidDeviceOwnerGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="63dbb-103">List androidDeviceOwnerGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="63dbb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="63dbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63dbb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63dbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63dbb-106">Listar Propriedades e relações dos objetos [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="63dbb-106">List properties and relationships of the [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63dbb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="63dbb-107">Prerequisites</span></span>
<span data-ttu-id="63dbb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63dbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63dbb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63dbb-110">Permission type</span></span>|<span data-ttu-id="63dbb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="63dbb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63dbb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63dbb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63dbb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="63dbb-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="63dbb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63dbb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63dbb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63dbb-115">Not supported.</span></span>|
|<span data-ttu-id="63dbb-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63dbb-116">Application</span></span>|<span data-ttu-id="63dbb-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63dbb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63dbb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63dbb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="63dbb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="63dbb-119">Request headers</span></span>
|<span data-ttu-id="63dbb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="63dbb-120">Header</span></span>|<span data-ttu-id="63dbb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="63dbb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63dbb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="63dbb-122">Authorization</span></span>|<span data-ttu-id="63dbb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="63dbb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63dbb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="63dbb-124">Accept</span></span>|<span data-ttu-id="63dbb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="63dbb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63dbb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63dbb-126">Request body</span></span>
<span data-ttu-id="63dbb-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="63dbb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63dbb-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="63dbb-128">Response</span></span>
<span data-ttu-id="63dbb-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="63dbb-129">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerGeneralDeviceConfiguration](../resources/intune-deviceconfig-androiddeviceownergeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63dbb-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="63dbb-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="63dbb-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="63dbb-131">Request</span></span>
<span data-ttu-id="63dbb-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="63dbb-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="63dbb-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="63dbb-133">Response</span></span>
<span data-ttu-id="63dbb-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="63dbb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4295

{
  "value": [
    {
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
      "dataRoamingBlocked": true,
      "dateTimeConfigurationBlocked": true,
      "factoryResetDeviceAdministratorEmails": [
        "Factory Reset Device Administrator Emails value"
      ],
      "factoryResetBlocked": true,
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
      "kioskModeBluetoothConfigurationEnabled": true,
      "kioskModeWiFiConfigurationEnabled": true,
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
      "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
      "vpnAlwaysOnLockdownMode": true,
      "wifiBlockEditConfigurations": true,
      "wifiBlockEditPolicyDefinedConfigurations": true
    }
  ]
}
```





