---
title: Listar macOSDeviceFeaturesConfigurations
description: Listar propriedades e relações dos objetos macOSDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6da2f640451547f74c61d310176453ae9ec2636b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066114"
---
# <a name="list-macosdevicefeaturesconfigurations"></a><span data-ttu-id="21d1e-103">Listar macOSDeviceFeaturesConfigurations</span><span class="sxs-lookup"><span data-stu-id="21d1e-103">List macOSDeviceFeaturesConfigurations</span></span>

<span data-ttu-id="21d1e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21d1e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21d1e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21d1e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21d1e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21d1e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21d1e-107">Listar propriedades e relações dos objetos [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="21d1e-107">List properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21d1e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21d1e-108">Prerequisites</span></span>
<span data-ttu-id="21d1e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21d1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21d1e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21d1e-111">Permission type</span></span>|<span data-ttu-id="21d1e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21d1e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21d1e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21d1e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="21d1e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="21d1e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="21d1e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21d1e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21d1e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21d1e-116">Not supported.</span></span>|
|<span data-ttu-id="21d1e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="21d1e-117">Application</span></span>|<span data-ttu-id="21d1e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="21d1e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21d1e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21d1e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="21d1e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21d1e-120">Request headers</span></span>
|<span data-ttu-id="21d1e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21d1e-121">Header</span></span>|<span data-ttu-id="21d1e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="21d1e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21d1e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="21d1e-123">Authorization</span></span>|<span data-ttu-id="21d1e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21d1e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21d1e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21d1e-125">Accept</span></span>|<span data-ttu-id="21d1e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="21d1e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21d1e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21d1e-127">Request body</span></span>
<span data-ttu-id="21d1e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="21d1e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21d1e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="21d1e-129">Response</span></span>
<span data-ttu-id="21d1e-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21d1e-130">If successful, this method returns a `200 OK` response code and a collection of [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21d1e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21d1e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="21d1e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21d1e-132">Request</span></span>
<span data-ttu-id="21d1e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21d1e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="21d1e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="21d1e-134">Response</span></span>
<span data-ttu-id="21d1e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21d1e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 6245

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
      "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
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
      "autoLaunchItems": [
        {
          "@odata.type": "microsoft.graph.macOSLaunchItem",
          "path": "Path value",
          "hide": true
        }
      ],
      "adminShowHostInfo": true,
      "loginWindowText": "Login Window Text value",
      "authorizedUsersListHidden": true,
      "authorizedUsersListHideLocalUsers": true,
      "authorizedUsersListHideMobileAccounts": true,
      "authorizedUsersListIncludeNetworkUsers": true,
      "authorizedUsersListHideAdminUsers": true,
      "authorizedUsersListShowOtherManagedUsers": true,
      "shutDownDisabled": true,
      "restartDisabled": true,
      "sleepDisabled": true,
      "consoleAccessDisabled": true,
      "shutDownDisabledWhileLoggedIn": true,
      "restartDisabledWhileLoggedIn": true,
      "powerOffDisabledWhileLoggedIn": true,
      "logOutDisabledWhileLoggedIn": true,
      "screenLockDisableImmediate": true,
      "associatedDomains": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "singleSignOnExtension": {
        "@odata.type": "microsoft.graph.credentialSingleSignOnExtension",
        "extensionIdentifier": "Extension Identifier value",
        "teamIdentifier": "Team Identifier value",
        "domains": [
          "Domains value"
        ],
        "realm": "Realm value",
        "configurations": [
          {
            "@odata.type": "microsoft.graph.keyStringValuePair",
            "key": "Key value",
            "value": "Value value"
          }
        ]
      },
      "macOSSingleSignOnExtension": {
        "@odata.type": "microsoft.graph.macOSKerberosSingleSignOnExtension",
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
      "contentCachingEnabled": true,
      "contentCachingType": "userContentOnly",
      "contentCachingMaxSizeBytes": 10,
      "contentCachingDataPath": "Content Caching Data Path value",
      "contentCachingDisableConnectionSharing": true,
      "contentCachingForceConnectionSharing": true,
      "contentCachingClientPolicy": "clientsInLocalNetwork",
      "contentCachingClientListenRanges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "contentCachingPeerPolicy": "peersInLocalNetwork",
      "contentCachingPeerListenRanges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "contentCachingPeerFilterRanges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "contentCachingParentSelectionPolicy": "roundRobin",
      "contentCachingParents": [
        "Content Caching Parents value"
      ],
      "contentCachingLogClientIdentities": true,
      "contentCachingPublicRanges": [
        {
          "@odata.type": "microsoft.graph.iPv6Range",
          "lowerAddress": "Lower Address value",
          "upperAddress": "Upper Address value"
        }
      ],
      "contentCachingBlockDeletion": true,
      "contentCachingShowAlerts": true,
      "contentCachingKeepAwake": true,
      "contentCachingPort": 2
    }
  ]
}
```






