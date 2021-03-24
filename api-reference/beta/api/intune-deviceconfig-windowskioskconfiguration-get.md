---
title: Obter windowsKioskConfiguration
description: Leia propriedades e relações do objeto windowsKioskConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3c2984e881e616d1f404eaf843adf14b29ed845d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132342"
---
# <a name="get-windowskioskconfiguration"></a><span data-ttu-id="cf7a8-103">Obter windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf7a8-103">Get windowsKioskConfiguration</span></span>

<span data-ttu-id="cf7a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf7a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cf7a8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cf7a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf7a8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf7a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf7a8-107">Leia propriedades e relações do [objeto windowsKioskConfiguration.](../resources/intune-deviceconfig-windowskioskconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cf7a8-107">Read properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cf7a8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cf7a8-108">Prerequisites</span></span>
<span data-ttu-id="cf7a8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cf7a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf7a8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cf7a8-111">Permission type</span></span>|<span data-ttu-id="cf7a8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cf7a8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf7a8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cf7a8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cf7a8-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf7a8-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf7a8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cf7a8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf7a8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cf7a8-116">Not supported.</span></span>|
|<span data-ttu-id="cf7a8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cf7a8-117">Application</span></span>|<span data-ttu-id="cf7a8-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf7a8-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf7a8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cf7a8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf7a8-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cf7a8-120">Optional query parameters</span></span>
<span data-ttu-id="cf7a8-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="cf7a8-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf7a8-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cf7a8-122">Request headers</span></span>
|<span data-ttu-id="cf7a8-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cf7a8-123">Header</span></span>|<span data-ttu-id="cf7a8-124">Valor</span><span class="sxs-lookup"><span data-stu-id="cf7a8-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf7a8-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="cf7a8-125">Authorization</span></span>|<span data-ttu-id="cf7a8-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cf7a8-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf7a8-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cf7a8-127">Accept</span></span>|<span data-ttu-id="cf7a8-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cf7a8-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf7a8-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cf7a8-129">Request body</span></span>
<span data-ttu-id="cf7a8-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cf7a8-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf7a8-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf7a8-131">Response</span></span>
<span data-ttu-id="cf7a8-132">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cf7a8-132">If successful, this method returns a `200 OK` response code and [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf7a8-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cf7a8-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf7a8-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cf7a8-134">Request</span></span>
<span data-ttu-id="cf7a8-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cf7a8-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="cf7a8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="cf7a8-136">Response</span></span>
<span data-ttu-id="cf7a8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cf7a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3186

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
    "id": "146a990b-990b-146a-0b99-6a140b996a14",
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
    "kioskProfiles": [
      {
        "@odata.type": "microsoft.graph.windowsKioskProfile",
        "profileId": "Profile Id value",
        "profileName": "Profile Name value",
        "appConfiguration": {
          "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
          "apps": [
            {
              "@odata.type": "microsoft.graph.windowsKioskUWPApp",
              "startLayoutTileSize": "small",
              "name": "Name value",
              "appType": "store",
              "autoLaunch": true,
              "appUserModelId": "App User Model Id value",
              "appId": "App Id value",
              "containedAppId": "Contained App Id value"
            }
          ],
          "showTaskBar": true,
          "allowAccessToDownloadsFolder": true,
          "disallowDesktopApps": true,
          "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
        },
        "userAccountsConfiguration": [
          {
            "@odata.type": "microsoft.graph.windowsKioskVisitor"
          }
        ]
      }
    ],
    "kioskBrowserDefaultUrl": "https://example.com/kioskBrowserDefaultUrl/",
    "kioskBrowserEnableHomeButton": true,
    "kioskBrowserEnableNavigationButtons": true,
    "kioskBrowserEnableEndSessionButton": true,
    "kioskBrowserRestartOnIdleTimeInMinutes": 6,
    "kioskBrowserBlockedURLs": [
      "Kiosk Browser Blocked URLs value"
    ],
    "kioskBrowserBlockedUrlExceptions": [
      "Kiosk Browser Blocked Url Exceptions value"
    ],
    "edgeKioskEnablePublicBrowsing": true,
    "windowsKioskForceUpdateSchedule": {
      "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "recurrence": "daily",
      "dayofWeek": "monday",
      "dayofMonth": 10,
      "runImmediatelyIfAfterStartDateTime": true
    }
  }
}
```




