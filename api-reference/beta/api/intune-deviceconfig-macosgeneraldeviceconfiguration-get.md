---
title: Get macOSGeneralDeviceConfiguration
description: Ler propriedades e relações do objeto macOSGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bbcc485fe055290a0bb4dbe2cca6eae76fa2a335
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33922413"
---
# <a name="get-macosgeneraldeviceconfiguration"></a><span data-ttu-id="aaf90-103">Get macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="aaf90-103">Get macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="aaf90-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aaf90-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aaf90-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aaf90-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aaf90-106">Ler propriedades e relações do objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="aaf90-106">Read properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aaf90-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="aaf90-107">Prerequisites</span></span>
<span data-ttu-id="aaf90-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaf90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaf90-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="aaf90-110">Permission type</span></span>|<span data-ttu-id="aaf90-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="aaf90-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aaf90-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="aaf90-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aaf90-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="aaf90-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="aaf90-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="aaf90-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aaf90-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aaf90-115">Not supported.</span></span>|
|<span data-ttu-id="aaf90-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="aaf90-116">Application</span></span>|<span data-ttu-id="aaf90-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="aaf90-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aaf90-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="aaf90-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aaf90-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="aaf90-119">Optional query parameters</span></span>
<span data-ttu-id="aaf90-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="aaf90-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aaf90-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aaf90-121">Request headers</span></span>
|<span data-ttu-id="aaf90-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="aaf90-122">Header</span></span>|<span data-ttu-id="aaf90-123">Valor</span><span class="sxs-lookup"><span data-stu-id="aaf90-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aaf90-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="aaf90-124">Authorization</span></span>|<span data-ttu-id="aaf90-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="aaf90-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aaf90-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="aaf90-126">Accept</span></span>|<span data-ttu-id="aaf90-127">application/json</span><span class="sxs-lookup"><span data-stu-id="aaf90-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaf90-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="aaf90-128">Request body</span></span>
<span data-ttu-id="aaf90-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="aaf90-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aaf90-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaf90-130">Response</span></span>
<span data-ttu-id="aaf90-131">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="aaf90-131">If successful, this method returns a `200 OK` response code and [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaf90-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="aaf90-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="aaf90-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="aaf90-133">Request</span></span>
<span data-ttu-id="aaf90-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="aaf90-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="aaf90-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="aaf90-135">Response</span></span>
<span data-ttu-id="aaf90-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="aaf90-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2656

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
    "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
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
    "emailInDomainSuffixes": [
      "Email In Domain Suffixes value"
    ],
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumCharacterSetCount": 0,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequiredType": "alphanumeric",
    "passwordRequired": true,
    "keychainBlockCloudSync": true,
    "airPrintBlocked": true,
    "airPrintForceTrustedTLS": true,
    "airPrintBlockiBeaconDiscovery": true,
    "safariBlockAutofill": true,
    "cameraBlocked": true,
    "iTunesBlockMusicService": true,
    "spotlightBlockInternetResults": true,
    "keyboardBlockDictation": true,
    "definitionLookupBlocked": true,
    "appleWatchBlockAutoUnlock": true,
    "iTunesBlockFileSharing": true,
    "iCloudBlockDocumentSync": true,
    "iCloudBlockMail": true,
    "iCloudBlockAddressBook": true,
    "iCloudBlockCalendar": true,
    "iCloudBlockReminders": true,
    "iCloudBlockBookmarks": true,
    "iCloudBlockNotes": true,
    "airDropBlocked": true,
    "passwordBlockModification": true,
    "passwordBlockFingerprintUnlock": true,
    "passwordBlockAutoFill": true,
    "passwordBlockProximityRequests": true,
    "passwordBlockAirDropSharing": true,
    "softwareUpdatesEnforcedDelayInDays": 2,
    "softwareUpdatesForceDelayed": true,
    "contentCachingBlocked": true,
    "iCloudBlockPhotoLibrary": true,
    "screenCaptureBlocked": true,
    "classroomAppBlockRemoteScreenObservation": true,
    "classroomAppForceUnpromptedScreenObservation": true,
    "classroomForceAutomaticallyJoinClasses": true,
    "classroomForceRequestPermissionToLeaveClasses": true,
    "classroomForceUnpromptedAppAndDeviceLock": true
  }
}
```




