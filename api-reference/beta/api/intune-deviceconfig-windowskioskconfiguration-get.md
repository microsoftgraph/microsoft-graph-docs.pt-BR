---
title: Obter windowsKioskConfiguration
description: Leia as propriedades e os relacionamentos do objeto windowsKioskConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 23af378bba3fe360b9869d80b91d427d32b55c9d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411719"
---
# <a name="get-windowskioskconfiguration"></a><span data-ttu-id="50ce3-103">Obter windowsKioskConfiguration</span><span class="sxs-lookup"><span data-stu-id="50ce3-103">Get windowsKioskConfiguration</span></span>

> <span data-ttu-id="50ce3-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="50ce3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="50ce3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="50ce3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="50ce3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="50ce3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50ce3-107">Leia as propriedades e os relacionamentos do objeto [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="50ce3-107">Read properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50ce3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50ce3-108">Prerequisites</span></span>
<span data-ttu-id="50ce3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="50ce3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="50ce3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="50ce3-111">Permission type</span></span>|<span data-ttu-id="50ce3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="50ce3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50ce3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="50ce3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50ce3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="50ce3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="50ce3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="50ce3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50ce3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50ce3-116">Not supported.</span></span>|
|<span data-ttu-id="50ce3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="50ce3-117">Application</span></span>|<span data-ttu-id="50ce3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="50ce3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="50ce3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50ce3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="50ce3-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="50ce3-120">Optional query parameters</span></span>
<span data-ttu-id="50ce3-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="50ce3-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50ce3-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50ce3-122">Request headers</span></span>
|<span data-ttu-id="50ce3-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="50ce3-123">Header</span></span>|<span data-ttu-id="50ce3-124">Valor</span><span class="sxs-lookup"><span data-stu-id="50ce3-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50ce3-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="50ce3-125">Authorization</span></span>|<span data-ttu-id="50ce3-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50ce3-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50ce3-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="50ce3-127">Accept</span></span>|<span data-ttu-id="50ce3-128">application/json</span><span class="sxs-lookup"><span data-stu-id="50ce3-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50ce3-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50ce3-129">Request body</span></span>
<span data-ttu-id="50ce3-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="50ce3-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50ce3-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="50ce3-131">Response</span></span>
<span data-ttu-id="50ce3-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50ce3-132">If successful, this method returns a `200 OK` response code and [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50ce3-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50ce3-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="50ce3-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50ce3-134">Request</span></span>
<span data-ttu-id="50ce3-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50ce3-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="50ce3-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="50ce3-136">Response</span></span>
<span data-ttu-id="50ce3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="50ce3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2016

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
              "appUserModelId": "App User Model Id value",
              "appId": "App Id value",
              "containedAppId": "Contained App Id value"
            }
          ],
          "showTaskBar": true,
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
    "edgeKioskResetAfterIdleTimeInMinutes": 4
  }
}
```




