---
title: Get iosDeviceFeaturesConfiguration
description: Ler propriedades e relações do objeto iosDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 14f8d9c8fa6283bb22e6b2264c32423222868081
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132671"
---
# <a name="get-iosdevicefeaturesconfiguration"></a><span data-ttu-id="e1f27-103">Get iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1f27-103">Get iosDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="e1f27-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1f27-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1f27-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e1f27-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1f27-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e1f27-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1f27-107">Ler propriedades e relações do objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="e1f27-107">Read properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1f27-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1f27-108">Prerequisites</span></span>
<span data-ttu-id="e1f27-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1f27-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e1f27-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1f27-111">Permission type</span></span>|<span data-ttu-id="e1f27-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1f27-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1f27-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1f27-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1f27-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1f27-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1f27-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1f27-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1f27-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1f27-116">Not supported.</span></span>|
|<span data-ttu-id="e1f27-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1f27-117">Application</span></span>|<span data-ttu-id="e1f27-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1f27-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1f27-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1f27-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1f27-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e1f27-120">Optional query parameters</span></span>
<span data-ttu-id="e1f27-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e1f27-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e1f27-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1f27-122">Request headers</span></span>
|<span data-ttu-id="e1f27-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1f27-123">Header</span></span>|<span data-ttu-id="e1f27-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e1f27-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1f27-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1f27-125">Authorization</span></span>|<span data-ttu-id="e1f27-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1f27-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1f27-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1f27-127">Accept</span></span>|<span data-ttu-id="e1f27-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e1f27-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1f27-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1f27-129">Request body</span></span>
<span data-ttu-id="e1f27-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1f27-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1f27-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1f27-131">Response</span></span>
<span data-ttu-id="e1f27-132">Se bem-sucedido, este método retornará um código de resposta `200 OK` e um objeto [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1f27-132">If successful, this method returns a `200 OK` response code and [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e1f27-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1f27-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1f27-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1f27-134">Request</span></span>
<span data-ttu-id="e1f27-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1f27-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="e1f27-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1f27-136">Response</span></span>
<span data-ttu-id="e1f27-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1f27-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 7435

{
  "value": {
    "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
    "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
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
                "bundleID": "Bundle ID value",
                "isWebClip": true
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
                    "bundleID": "Bundle ID value",
                    "isWebClip": true
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
        "soundsEnabled": true,
        "previewVisibility": "alwaysShow"
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
    },
    "wallpaperDisplayLocation": "lockScreen",
    "wallpaperImage": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "singleSignOnExtension": {
      "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension",
      "realm": "Realm value",
      "domains": [
        "Domains value"
      ],
      "blockAutomaticLogin": true,
      "cacheName": "Cache Name value",
      "credentialBundleIdAccessControlList": [
        "Credential Bundle Id Access Control List value"
      ],
      "domainRealms": [
        "Domain Realms value"
      ],
      "isDefaultRealm": true,
      "passwordBlockModification": true,
      "passwordExpirationDays": 6,
      "passwordExpirationNotificationDays": 2,
      "userPrincipalName": "User Principal Name value",
      "passwordRequireActiveDirectoryComplexity": true,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordMinimumLength": 5,
      "passwordMinimumAgeDays": 6,
      "passwordRequirementsDescription": "Password Requirements Description value",
      "requireUserPresence": true,
      "activeDirectorySiteCode": "Active Directory Site Code value",
      "passwordEnableLocalSync": true,
      "blockActiveDirectorySiteAutoDiscovery": true,
      "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
    },
    "iosSingleSignOnExtension": {
      "@odata.type": "microsoft.graph.iosKerberosSingleSignOnExtension",
      "realm": "Realm value",
      "domains": [
        "Domains value"
      ],
      "blockAutomaticLogin": true,
      "cacheName": "Cache Name value",
      "credentialBundleIdAccessControlList": [
        "Credential Bundle Id Access Control List value"
      ],
      "domainRealms": [
        "Domain Realms value"
      ],
      "isDefaultRealm": true,
      "passwordBlockModification": true,
      "passwordExpirationDays": 6,
      "passwordExpirationNotificationDays": 2,
      "userPrincipalName": "User Principal Name value",
      "passwordRequireActiveDirectoryComplexity": true,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordMinimumLength": 5,
      "passwordMinimumAgeDays": 6,
      "passwordRequirementsDescription": "Password Requirements Description value",
      "requireUserPresence": true,
      "activeDirectorySiteCode": "Active Directory Site Code value",
      "passwordEnableLocalSync": true,
      "blockActiveDirectorySiteAutoDiscovery": true,
      "passwordChangeUrl": "https://example.com/passwordChangeUrl/"
    }
  }
}
```




