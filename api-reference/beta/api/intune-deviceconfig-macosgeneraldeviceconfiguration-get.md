---
title: Get macOSGeneralDeviceConfiguration
description: Ler propriedades e relações do objeto macOSGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: acc88c96ad41218b8c4f6b463ec439595846f006
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724814"
---
# <a name="get-macosgeneraldeviceconfiguration"></a><span data-ttu-id="36e17-103">Get macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="36e17-103">Get macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="36e17-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="36e17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="36e17-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="36e17-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="36e17-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="36e17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="36e17-107">Ler propriedades e relações do objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="36e17-107">Read properties and relationships of the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="36e17-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="36e17-108">Prerequisites</span></span>
<span data-ttu-id="36e17-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36e17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36e17-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="36e17-111">Permission type</span></span>|<span data-ttu-id="36e17-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="36e17-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="36e17-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="36e17-113">Delegated (work or school account)</span></span>|<span data-ttu-id="36e17-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="36e17-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="36e17-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="36e17-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="36e17-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="36e17-116">Not supported.</span></span>|
|<span data-ttu-id="36e17-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="36e17-117">Application</span></span>|<span data-ttu-id="36e17-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="36e17-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="36e17-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="36e17-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="36e17-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="36e17-120">Optional query parameters</span></span>
<span data-ttu-id="36e17-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="36e17-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="36e17-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="36e17-122">Request headers</span></span>
|<span data-ttu-id="36e17-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="36e17-123">Header</span></span>|<span data-ttu-id="36e17-124">Valor</span><span class="sxs-lookup"><span data-stu-id="36e17-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="36e17-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="36e17-125">Authorization</span></span>|<span data-ttu-id="36e17-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="36e17-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="36e17-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="36e17-127">Accept</span></span>|<span data-ttu-id="36e17-128">application/json</span><span class="sxs-lookup"><span data-stu-id="36e17-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="36e17-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="36e17-129">Request body</span></span>
<span data-ttu-id="36e17-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="36e17-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="36e17-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="36e17-131">Response</span></span>
<span data-ttu-id="36e17-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="36e17-132">If successful, this method returns a `200 OK` response code and [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="36e17-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="36e17-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="36e17-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="36e17-134">Request</span></span>
<span data-ttu-id="36e17-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="36e17-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="36e17-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="36e17-136">Response</span></span>
<span data-ttu-id="36e17-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="36e17-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5135

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
    "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
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
    "passwordMaximumAttemptCount": 11,
    "passwordMinutesUntilFailedLoginReset": 4,
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
    "updateDelayPolicy": "delayOSUpdateVisibility",
    "contentCachingBlocked": true,
    "iCloudBlockPhotoLibrary": true,
    "screenCaptureBlocked": true,
    "classroomAppBlockRemoteScreenObservation": true,
    "classroomAppForceUnpromptedScreenObservation": true,
    "classroomForceAutomaticallyJoinClasses": true,
    "classroomForceRequestPermissionToLeaveClasses": true,
    "classroomForceUnpromptedAppAndDeviceLock": true,
    "iCloudBlockActivityContinuation": true,
    "privacyAccessControls": [
      {
        "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem",
        "displayName": "Display Name value",
        "identifier": "Identifier value",
        "identifierType": "path",
        "codeRequirement": "Code Requirement value",
        "staticCodeValidation": true,
        "blockCamera": true,
        "blockMicrophone": true,
        "blockScreenCapture": true,
        "blockListenEvent": true,
        "speechRecognition": "enabled",
        "accessibility": "enabled",
        "addressBook": "enabled",
        "calendar": "enabled",
        "reminders": "enabled",
        "photos": "enabled",
        "mediaLibrary": "enabled",
        "fileProviderPresence": "enabled",
        "systemPolicyAllFiles": "enabled",
        "systemPolicySystemAdminFiles": "enabled",
        "systemPolicyDesktopFolder": "enabled",
        "systemPolicyDocumentsFolder": "enabled",
        "systemPolicyDownloadsFolder": "enabled",
        "systemPolicyNetworkVolumes": "enabled",
        "systemPolicyRemovableVolumes": "enabled",
        "postEvent": "enabled",
        "appleEventsAllowedReceivers": [
          {
            "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
            "codeRequirement": "Code Requirement value",
            "identifier": "Identifier value",
            "identifierType": "path",
            "allowed": true
          }
        ]
      }
    ]
  }
}
```





