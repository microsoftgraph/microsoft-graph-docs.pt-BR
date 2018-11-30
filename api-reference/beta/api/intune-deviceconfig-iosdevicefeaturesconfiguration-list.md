---
title: Listar iosDeviceFeaturesConfigurations
description: Listar propriedades e relações dos objetos iosDeviceFeaturesConfiguration.
ms.openlocfilehash: dffe7300f243f1c374889b56f9e17aa4c31ba6d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033273"
---
# <a name="list-iosdevicefeaturesconfigurations"></a><span data-ttu-id="5b4f6-103">Listar iosDeviceFeaturesConfigurations</span><span class="sxs-lookup"><span data-stu-id="5b4f6-103">List iosDeviceFeaturesConfigurations</span></span>

> <span data-ttu-id="5b4f6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5b4f6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b4f6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5b4f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b4f6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5b4f6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b4f6-107">Listar propriedades e relações dos objetos [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5b4f6-107">List properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5b4f6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5b4f6-108">Prerequisites</span></span>
<span data-ttu-id="5b4f6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b4f6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b4f6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b4f6-111">Permission type</span></span>|<span data-ttu-id="5b4f6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5b4f6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b4f6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b4f6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b4f6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5b4f6-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5b4f6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b4f6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b4f6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b4f6-116">Not supported.</span></span>|
|<span data-ttu-id="5b4f6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b4f6-117">Application</span></span>|<span data-ttu-id="5b4f6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b4f6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b4f6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b4f6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5b4f6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b4f6-120">Request headers</span></span>
|<span data-ttu-id="5b4f6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b4f6-121">Header</span></span>|<span data-ttu-id="5b4f6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5b4f6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b4f6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b4f6-123">Authorization</span></span>|<span data-ttu-id="5b4f6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b4f6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b4f6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5b4f6-125">Accept</span></span>|<span data-ttu-id="5b4f6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b4f6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b4f6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b4f6-127">Request body</span></span>
<span data-ttu-id="5b4f6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5b4f6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5b4f6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b4f6-129">Response</span></span>
<span data-ttu-id="5b4f6-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b4f6-130">If successful, this method returns a `200 OK` response code and a collection of [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b4f6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b4f6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="5b4f6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b4f6-132">Request</span></span>
<span data-ttu-id="5b4f6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b4f6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="5b4f6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b4f6-134">Response</span></span>
<span data-ttu-id="5b4f6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b4f6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4152

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
      "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "airPrintDestinations": [
        {
          "@odata.type": "microsoft.graph.airPrintDestination",
          "ipAddress": "Ip Address value",
          "resourcePath": "Resource Path value",
          "port": 4,
          "forceTls": true
        }
      ],
      "assetTagTemplate": "Asset Tag Template value",
      "contentFilterSettings": {
        "@odata.type": "microsoft.graph.iosWebContentFilterSpecificWebsitesAccess",
        "specificWebsitesOnly": [
          {
            "@odata.type": "microsoft.graph.iosBookmark",
            "url": "Url value",
            "bookmarkFolder": "Bookmark Folder value",
            "displayName": "Display Name value"
          }
        ],
        "websiteList": [
          {
            "@odata.type": "microsoft.graph.iosBookmark",
            "url": "Url value",
            "bookmarkFolder": "Bookmark Folder value",
            "displayName": "Display Name value"
          }
        ]
      },
      "lockScreenFootnote": "Lock Screen Footnote value",
      "homeScreenDockIcons": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolder",
          "displayName": "Display Name value",
          "pages": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
              "displayName": "Display Name value",
              "apps": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenApp",
                  "displayName": "Display Name value",
                  "bundleID": "Bundle ID value"
                }
              ]
            }
          ]
        }
      ],
      "homeScreenPages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenPage",
          "displayName": "Display Name value",
          "icons": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenFolder",
              "displayName": "Display Name value",
              "pages": [
                {
                  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
                  "displayName": "Display Name value",
                  "apps": [
                    {
                      "@odata.type": "microsoft.graph.iosHomeScreenApp",
                      "displayName": "Display Name value",
                      "bundleID": "Bundle ID value"
                    }
                  ]
                }
              ]
            }
          ]
        }
      ],
      "notificationSettings": [
        {
          "@odata.type": "microsoft.graph.iosNotificationSettings",
          "bundleID": "Bundle ID value",
          "appName": "App Name value",
          "publisher": "Publisher value",
          "enabled": true,
          "showInNotificationCenter": true,
          "showOnLockScreen": true,
          "alertType": "banner",
          "badgesEnabled": true,
          "soundsEnabled": true
        }
      ],
      "singleSignOnSettings": {
        "@odata.type": "microsoft.graph.iosSingleSignOnSettings",
        "allowedAppsList": [
          {
            "@odata.type": "microsoft.graph.appListItem",
            "name": "Name value",
            "publisher": "Publisher value",
            "appStoreUrl": "https://example.com/appStoreUrl/",
            "appId": "App Id value"
          }
        ],
        "allowedUrls": [
          "Allowed Urls value"
        ],
        "displayName": "Display Name value",
        "kerberosPrincipalName": "Kerberos Principal Name value",
        "kerberosRealm": "Kerberos Realm value"
      }
    }
  ]
}
```





