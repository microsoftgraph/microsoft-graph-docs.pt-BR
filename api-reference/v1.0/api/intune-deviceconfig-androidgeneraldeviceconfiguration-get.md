---
title: Acessar androidGeneralDeviceConfiguration
description: Leia as propriedades e relações do objeto androidGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d2702dc21f9892db759188ddbef3b050302d18e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32553537"
---
# <a name="get-androidgeneraldeviceconfiguration"></a><span data-ttu-id="179d9-103">Acessar androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="179d9-103">Get androidGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="179d9-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="179d9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="179d9-105">Leia as propriedades e relações do objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="179d9-105">Read properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="179d9-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="179d9-106">Prerequisites</span></span>
<span data-ttu-id="179d9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="179d9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="179d9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="179d9-109">Permission type</span></span>|<span data-ttu-id="179d9-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="179d9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="179d9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="179d9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="179d9-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="179d9-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="179d9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="179d9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="179d9-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="179d9-114">Not supported.</span></span>|
|<span data-ttu-id="179d9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="179d9-115">Application</span></span>|<span data-ttu-id="179d9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="179d9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="179d9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="179d9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="179d9-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="179d9-118">Optional query parameters</span></span>
<span data-ttu-id="179d9-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="179d9-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="179d9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="179d9-120">Request headers</span></span>
|<span data-ttu-id="179d9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="179d9-121">Header</span></span>|<span data-ttu-id="179d9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="179d9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="179d9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="179d9-123">Authorization</span></span>|<span data-ttu-id="179d9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="179d9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="179d9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="179d9-125">Accept</span></span>|<span data-ttu-id="179d9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="179d9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="179d9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="179d9-127">Request body</span></span>
<span data-ttu-id="179d9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="179d9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="179d9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="179d9-129">Response</span></span>
<span data-ttu-id="179d9-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="179d9-130">If successful, this method returns a `200 OK` response code and [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="179d9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="179d9-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="179d9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="179d9-132">Request</span></span>
<span data-ttu-id="179d9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="179d9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="179d9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="179d9-134">Response</span></span>
<span data-ttu-id="179d9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="179d9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3414

{
  "value": {
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
}
```



