---
title: Listar windowsKioskConfigurations
description: Listar Propriedades e relações dos objetos windowsKioskConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fd2004fa3ecd99fac5186ca53eefc975e8a546c5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32513325"
---
# <a name="list-windowskioskconfigurations"></a><span data-ttu-id="1e148-103">Listar windowsKioskConfigurations</span><span class="sxs-lookup"><span data-stu-id="1e148-103">List windowsKioskConfigurations</span></span>

> <span data-ttu-id="1e148-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1e148-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e148-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e148-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e148-106">Listar Propriedades e relações dos objetos [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1e148-106">List properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e148-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e148-107">Prerequisites</span></span>
<span data-ttu-id="1e148-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e148-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e148-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e148-110">Permission type</span></span>|<span data-ttu-id="1e148-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1e148-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e148-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e148-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e148-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1e148-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1e148-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e148-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e148-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e148-115">Not supported.</span></span>|
|<span data-ttu-id="1e148-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e148-116">Application</span></span>|<span data-ttu-id="1e148-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e148-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e148-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e148-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1e148-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e148-119">Request headers</span></span>
|<span data-ttu-id="1e148-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e148-120">Header</span></span>|<span data-ttu-id="1e148-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1e148-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e148-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e148-122">Authorization</span></span>|<span data-ttu-id="1e148-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e148-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e148-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1e148-124">Accept</span></span>|<span data-ttu-id="1e148-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1e148-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e148-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e148-126">Request body</span></span>
<span data-ttu-id="1e148-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1e148-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e148-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e148-128">Response</span></span>
<span data-ttu-id="1e148-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e148-129">If successful, this method returns a `200 OK` response code and a collection of [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e148-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e148-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e148-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e148-131">Request</span></span>
<span data-ttu-id="1e148-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e148-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="1e148-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e148-133">Response</span></span>
<span data-ttu-id="1e148-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e148-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





