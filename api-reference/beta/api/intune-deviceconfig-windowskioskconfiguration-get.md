---
title: Obter windowsKioskConfiguration
description: Leia as propriedades e as relações do objeto windowsKioskConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b38beb41a6786789061b0efaeb167f596b2869a
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963069"
---
# <a name="get-windowskioskconfiguration"></a><span data-ttu-id="52d4c-103">Obter windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="52d4c-103">Get windowsKioskConfiguration</span></span>

> <span data-ttu-id="52d4c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52d4c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52d4c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52d4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52d4c-106">Leia as propriedades e as relações do objeto [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="52d4c-106">Read properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="52d4c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="52d4c-107">Prerequisites</span></span>
<span data-ttu-id="52d4c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="52d4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52d4c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="52d4c-110">Permission type</span></span>|<span data-ttu-id="52d4c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="52d4c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="52d4c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="52d4c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="52d4c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="52d4c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="52d4c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="52d4c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="52d4c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52d4c-115">Not supported.</span></span>|
|<span data-ttu-id="52d4c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="52d4c-116">Application</span></span>|<span data-ttu-id="52d4c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="52d4c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="52d4c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="52d4c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="52d4c-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="52d4c-119">Optional query parameters</span></span>
<span data-ttu-id="52d4c-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="52d4c-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52d4c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="52d4c-121">Request headers</span></span>
|<span data-ttu-id="52d4c-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="52d4c-122">Header</span></span>|<span data-ttu-id="52d4c-123">Valor</span><span class="sxs-lookup"><span data-stu-id="52d4c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="52d4c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="52d4c-124">Authorization</span></span>|<span data-ttu-id="52d4c-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="52d4c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="52d4c-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="52d4c-126">Accept</span></span>|<span data-ttu-id="52d4c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="52d4c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="52d4c-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="52d4c-128">Request body</span></span>
<span data-ttu-id="52d4c-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="52d4c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52d4c-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="52d4c-130">Response</span></span>
<span data-ttu-id="52d4c-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="52d4c-131">If successful, this method returns a `200 OK` response code and [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="52d4c-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="52d4c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="52d4c-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="52d4c-133">Request</span></span>
<span data-ttu-id="52d4c-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="52d4c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="52d4c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="52d4c-135">Response</span></span>
<span data-ttu-id="52d4c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="52d4c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2052

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
    "id": "146a990b-990b-146a-0b99-6a140b996a14",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
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
    "edgeKioskEnablePublicBrowsing": true
  }
}
```




