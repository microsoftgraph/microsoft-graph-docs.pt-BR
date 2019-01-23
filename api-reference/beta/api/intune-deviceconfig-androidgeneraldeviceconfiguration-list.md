---
title: Listar androidGeneralDeviceConfigurations
description: Listar propriedades e relações dos objetos androidGeneralDeviceConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 29238ec219823824f75ff32d1fea085d6de3b513
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418355"
---
# <a name="list-androidgeneraldeviceconfigurations"></a><span data-ttu-id="f79ab-103">Listar androidGeneralDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="f79ab-103">List androidGeneralDeviceConfigurations</span></span>

> <span data-ttu-id="f79ab-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f79ab-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f79ab-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f79ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f79ab-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f79ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f79ab-107">Listar propriedades e relações dos objetos [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f79ab-107">List properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f79ab-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f79ab-108">Prerequisites</span></span>
<span data-ttu-id="f79ab-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f79ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f79ab-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f79ab-111">Permission type</span></span>|<span data-ttu-id="f79ab-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f79ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f79ab-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f79ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f79ab-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="f79ab-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="f79ab-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f79ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f79ab-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f79ab-116">Not supported.</span></span>|
|<span data-ttu-id="f79ab-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f79ab-117">Application</span></span>|<span data-ttu-id="f79ab-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f79ab-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f79ab-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f79ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f79ab-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f79ab-120">Request headers</span></span>
|<span data-ttu-id="f79ab-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f79ab-121">Header</span></span>|<span data-ttu-id="f79ab-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f79ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f79ab-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f79ab-123">Authorization</span></span>|<span data-ttu-id="f79ab-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f79ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f79ab-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f79ab-125">Accept</span></span>|<span data-ttu-id="f79ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f79ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f79ab-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f79ab-127">Request body</span></span>
<span data-ttu-id="f79ab-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f79ab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f79ab-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f79ab-129">Response</span></span>
<span data-ttu-id="f79ab-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f79ab-130">If successful, this method returns a `200 OK` response code and a collection of [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f79ab-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f79ab-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="f79ab-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f79ab-132">Request</span></span>
<span data-ttu-id="f79ab-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f79ab-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="f79ab-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f79ab-134">Response</span></span>
<span data-ttu-id="f79ab-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f79ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3766

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
      "id": "9e00d534-d534-9e00-34d5-009e34d5009e",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
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
      "dateAndTimeBlockChanges": true,
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




