---
title: Listar windowsKioskConfigurations
description: Listar Propriedades e relações dos objetos windowsKioskConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 58c071000b60ae98b62c821bc01854e3d8939136
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30570686"
---
# <a name="list-windowskioskconfigurations"></a><span data-ttu-id="69bed-103">Listar windowsKioskConfigurations</span><span class="sxs-lookup"><span data-stu-id="69bed-103">List windowsKioskConfigurations</span></span>

> <span data-ttu-id="69bed-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="69bed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69bed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="69bed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69bed-106">Listar Propriedades e relações dos objetos [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="69bed-106">List properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69bed-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="69bed-107">Prerequisites</span></span>
<span data-ttu-id="69bed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="69bed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="69bed-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="69bed-110">Permission type</span></span>|<span data-ttu-id="69bed-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="69bed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69bed-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="69bed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69bed-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69bed-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="69bed-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="69bed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69bed-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69bed-115">Not supported.</span></span>|
|<span data-ttu-id="69bed-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="69bed-116">Application</span></span>|<span data-ttu-id="69bed-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="69bed-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69bed-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="69bed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="69bed-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="69bed-119">Request headers</span></span>
|<span data-ttu-id="69bed-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="69bed-120">Header</span></span>|<span data-ttu-id="69bed-121">Valor</span><span class="sxs-lookup"><span data-stu-id="69bed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69bed-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="69bed-122">Authorization</span></span>|<span data-ttu-id="69bed-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="69bed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69bed-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="69bed-124">Accept</span></span>|<span data-ttu-id="69bed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69bed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69bed-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="69bed-126">Request body</span></span>
<span data-ttu-id="69bed-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="69bed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69bed-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="69bed-128">Response</span></span>
<span data-ttu-id="69bed-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="69bed-129">If successful, this method returns a `200 OK` response code and a collection of [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69bed-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="69bed-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="69bed-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="69bed-131">Request</span></span>
<span data-ttu-id="69bed-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="69bed-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="69bed-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="69bed-133">Response</span></span>
<span data-ttu-id="69bed-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="69bed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2174

{
  "value": [
    {
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
  ]
}
```




