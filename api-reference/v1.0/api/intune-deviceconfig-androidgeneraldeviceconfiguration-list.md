---
title: Listar androidGeneralDeviceConfigurations
description: Listar propriedades e relações dos objetos androidGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 629b83c58e87c5b1a9183143aef72716e47675b0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553243"
---
# <a name="list-androidgeneraldeviceconfigurations"></a><span data-ttu-id="945e6-103">Listar androidGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="945e6-103">List androidGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="945e6-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="945e6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="945e6-105">Listar propriedades e relações dos objetos [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="945e6-105">List properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="945e6-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="945e6-106">Prerequisites</span></span>
<span data-ttu-id="945e6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="945e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="945e6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="945e6-109">Permission type</span></span>|<span data-ttu-id="945e6-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="945e6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="945e6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="945e6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="945e6-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="945e6-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="945e6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="945e6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="945e6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="945e6-114">Not supported.</span></span>|
|<span data-ttu-id="945e6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="945e6-115">Application</span></span>|<span data-ttu-id="945e6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="945e6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="945e6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="945e6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="945e6-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="945e6-118">Request headers</span></span>
|<span data-ttu-id="945e6-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="945e6-119">Header</span></span>|<span data-ttu-id="945e6-120">Valor</span><span class="sxs-lookup"><span data-stu-id="945e6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="945e6-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="945e6-121">Authorization</span></span>|<span data-ttu-id="945e6-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="945e6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="945e6-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="945e6-123">Accept</span></span>|<span data-ttu-id="945e6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="945e6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="945e6-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="945e6-125">Request body</span></span>
<span data-ttu-id="945e6-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="945e6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="945e6-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="945e6-127">Response</span></span>
<span data-ttu-id="945e6-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="945e6-128">If successful, this method returns a `200 OK` response code and a collection of [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="945e6-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="945e6-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="945e6-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="945e6-130">Request</span></span>
<span data-ttu-id="945e6-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="945e6-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="945e6-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="945e6-132">Response</span></span>
<span data-ttu-id="945e6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="945e6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3618

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
      "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "appsBlockClipboardSharing": true,
      "appsBlockCopyPaste": true,
      "appsBlockYouTube": true,
      "bluetoothBlocked": true,
      "cameraBlocked": true,
      "cellularBlockDataRoaming": true,
      "cellularBlockMessaging": true,
      "cellularBlockVoiceRoaming": true,
      "cellularBlockWiFiTethering": true,
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
      "diagnosticDataBlockSubmission": true,
      "locationServicesBlocked": true,
      "googleAccountBlockAutoSync": true,
      "googlePlayStoreBlocked": true,
      "kioskModeBlockSleepButton": true,
      "kioskModeBlockVolumeButtons": true,
      "kioskModeApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "nfcBlocked": true,
      "passwordBlockFingerprintUnlock": true,
      "passwordBlockTrustAgents": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordRequiredType": "alphabetic",
      "passwordRequired": true,
      "powerOffBlocked": true,
      "factoryResetBlocked": true,
      "screenCaptureBlocked": true,
      "deviceSharingAllowed": true,
      "storageBlockGoogleBackup": true,
      "storageBlockRemovableStorage": true,
      "storageRequireDeviceEncryption": true,
      "storageRequireRemovableStorageEncryption": true,
      "voiceAssistantBlocked": true,
      "voiceDialingBlocked": true,
      "webBrowserBlockPopups": true,
      "webBrowserBlockAutofill": true,
      "webBrowserBlockJavaScript": true,
      "webBrowserBlocked": true,
      "webBrowserCookieSettings": "blockAlways",
      "wiFiBlocked": true,
      "appsInstallAllowList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "appsLaunchBlockList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "appsHideList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "securityRequireVerifyApps": true
    }
  ]
}
```



