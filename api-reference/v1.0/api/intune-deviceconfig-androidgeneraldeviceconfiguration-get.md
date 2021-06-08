---
title: Acessar androidGeneralDeviceConfiguration
description: Leia as propriedades e relações do objeto androidGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 99a821923c7c16548c793e0fe25dcc9945a7a318
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760661"
---
# <a name="get-androidgeneraldeviceconfiguration"></a><span data-ttu-id="3b0f6-103">Acessar androidGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3b0f6-103">Get androidGeneralDeviceConfiguration</span></span>

<span data-ttu-id="3b0f6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b0f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b0f6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b0f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b0f6-106">Leia as propriedades e relações do objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="3b0f6-106">Read properties and relationships of the [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b0f6-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b0f6-107">Prerequisites</span></span>
<span data-ttu-id="3b0f6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b0f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b0f6-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b0f6-110">Permission type</span></span>|<span data-ttu-id="3b0f6-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3b0f6-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b0f6-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b0f6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b0f6-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b0f6-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3b0f6-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b0f6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b0f6-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b0f6-115">Not supported.</span></span>|
|<span data-ttu-id="3b0f6-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b0f6-116">Application</span></span>|<span data-ttu-id="3b0f6-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b0f6-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b0f6-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b0f6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3b0f6-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3b0f6-119">Optional query parameters</span></span>
<span data-ttu-id="3b0f6-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3b0f6-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3b0f6-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b0f6-121">Request headers</span></span>
|<span data-ttu-id="3b0f6-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b0f6-122">Header</span></span>|<span data-ttu-id="3b0f6-123">Valor</span><span class="sxs-lookup"><span data-stu-id="3b0f6-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b0f6-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b0f6-124">Authorization</span></span>|<span data-ttu-id="3b0f6-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b0f6-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b0f6-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b0f6-126">Accept</span></span>|<span data-ttu-id="3b0f6-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3b0f6-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b0f6-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b0f6-128">Request body</span></span>
<span data-ttu-id="3b0f6-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3b0f6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b0f6-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b0f6-130">Response</span></span>
<span data-ttu-id="3b0f6-131">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b0f6-131">If successful, this method returns a `200 OK` response code and [androidGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b0f6-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b0f6-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b0f6-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b0f6-133">Request</span></span>
<span data-ttu-id="3b0f6-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b0f6-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="3b0f6-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b0f6-135">Response</span></span>
<span data-ttu-id="3b0f6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b0f6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




