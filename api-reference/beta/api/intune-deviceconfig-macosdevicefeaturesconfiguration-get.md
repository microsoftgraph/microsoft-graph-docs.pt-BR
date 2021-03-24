---
title: Obter macOSDeviceFeaturesConfiguration
description: Ler propriedades e relações do objeto macOSDeviceFeaturesConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2348bb9dd3aa5425d59f740a4c827b4e258ffd1a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147648"
---
# <a name="get-macosdevicefeaturesconfiguration"></a><span data-ttu-id="01a40-103">Obter macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="01a40-103">Get macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="01a40-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01a40-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01a40-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="01a40-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01a40-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="01a40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01a40-107">Ler propriedades e relações do objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="01a40-107">Read properties and relationships of the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="01a40-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="01a40-108">Prerequisites</span></span>
<span data-ttu-id="01a40-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01a40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01a40-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="01a40-111">Permission type</span></span>|<span data-ttu-id="01a40-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="01a40-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01a40-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="01a40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="01a40-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01a40-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="01a40-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="01a40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01a40-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="01a40-116">Not supported.</span></span>|
|<span data-ttu-id="01a40-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="01a40-117">Application</span></span>|<span data-ttu-id="01a40-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01a40-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="01a40-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="01a40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="01a40-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="01a40-120">Optional query parameters</span></span>
<span data-ttu-id="01a40-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="01a40-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01a40-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="01a40-122">Request headers</span></span>
|<span data-ttu-id="01a40-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="01a40-123">Header</span></span>|<span data-ttu-id="01a40-124">Valor</span><span class="sxs-lookup"><span data-stu-id="01a40-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01a40-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="01a40-125">Authorization</span></span>|<span data-ttu-id="01a40-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="01a40-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="01a40-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="01a40-127">Accept</span></span>|<span data-ttu-id="01a40-128">application/json</span><span class="sxs-lookup"><span data-stu-id="01a40-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01a40-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="01a40-129">Request body</span></span>
<span data-ttu-id="01a40-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="01a40-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01a40-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="01a40-131">Response</span></span>
<span data-ttu-id="01a40-132">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="01a40-132">If successful, this method returns a `200 OK` response code and [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01a40-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="01a40-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="01a40-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="01a40-134">Request</span></span>
<span data-ttu-id="01a40-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="01a40-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="01a40-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="01a40-136">Response</span></span>
<span data-ttu-id="01a40-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="01a40-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 6199

{
  "value": {
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
    "appAssociatedDomains": [
      {
        "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem",
        "applicationIdentifier": "Application Identifier value",
        "domains": [
          "Domains value"
        ],
        "directDownloadsEnabled": true
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
}
```




