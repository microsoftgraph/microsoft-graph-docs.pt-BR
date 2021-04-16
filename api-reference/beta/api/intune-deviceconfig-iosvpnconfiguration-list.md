---
title: Listar iosVpnConfigurations
description: Listar propriedades e relações dos objetos iosVpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0b52e4c9859acaadfbeaf9b56eeac8011ed2103d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868208"
---
# <a name="list-iosvpnconfigurations"></a><span data-ttu-id="1eb67-103">Listar iosVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="1eb67-103">List iosVpnConfigurations</span></span>

<span data-ttu-id="1eb67-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1eb67-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1eb67-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1eb67-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1eb67-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1eb67-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1eb67-107">Listar propriedades e relações dos [objetos iosVpnConfiguration.](../resources/intune-deviceconfig-iosvpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1eb67-107">List properties and relationships of the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1eb67-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1eb67-108">Prerequisites</span></span>
<span data-ttu-id="1eb67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1eb67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1eb67-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1eb67-111">Permission type</span></span>|<span data-ttu-id="1eb67-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1eb67-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1eb67-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1eb67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1eb67-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1eb67-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1eb67-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1eb67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1eb67-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1eb67-116">Not supported.</span></span>|
|<span data-ttu-id="1eb67-117">Application</span><span class="sxs-lookup"><span data-stu-id="1eb67-117">Application</span></span>|<span data-ttu-id="1eb67-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1eb67-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1eb67-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1eb67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1eb67-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb67-120">Request headers</span></span>
|<span data-ttu-id="1eb67-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1eb67-121">Header</span></span>|<span data-ttu-id="1eb67-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1eb67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1eb67-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1eb67-123">Authorization</span></span>|<span data-ttu-id="1eb67-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1eb67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1eb67-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1eb67-125">Accept</span></span>|<span data-ttu-id="1eb67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1eb67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1eb67-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb67-127">Request body</span></span>
<span data-ttu-id="1eb67-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1eb67-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1eb67-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1eb67-129">Response</span></span>
<span data-ttu-id="1eb67-130">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1eb67-130">If successful, this method returns a `200 OK` response code and a collection of [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1eb67-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1eb67-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1eb67-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1eb67-132">Request</span></span>
<span data-ttu-id="1eb67-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1eb67-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="1eb67-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1eb67-134">Response</span></span>
<span data-ttu-id="1eb67-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1eb67-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 4033

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVpnConfiguration",
      "id": "bd12424c-424c-bd12-4c42-12bd4c4212bd",
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
      "connectionName": "Connection Name value",
      "connectionType": "pulseSecure",
      "loginGroupOrDomain": "Login Group Or Domain value",
      "role": "Role value",
      "realm": "Realm value",
      "server": {
        "@odata.type": "microsoft.graph.vpnServer",
        "description": "Description value",
        "address": "Address value",
        "isDefaultServer": true
      },
      "identifier": "Identifier value",
      "customData": [
        {
          "@odata.type": "microsoft.graph.keyValue",
          "key": "Key value",
          "value": "Value value"
        }
      ],
      "customKeyValueData": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "enableSplitTunneling": true,
      "authenticationMethod": "usernameAndPassword",
      "enablePerApp": true,
      "safariDomains": [
        "Safari Domains value"
      ],
      "onDemandRules": [
        {
          "@odata.type": "microsoft.graph.vpnOnDemandRule",
          "ssids": [
            "Ssids value"
          ],
          "dnsSearchDomains": [
            "Dns Search Domains value"
          ],
          "probeUrl": "https://example.com/probeUrl/",
          "action": "evaluateConnection",
          "domainAction": "neverConnect",
          "domains": [
            "Domains value"
          ],
          "probeRequiredUrl": "https://example.com/probeRequiredUrl/"
        }
      ],
      "providerType": "appProxy",
      "associatedDomains": [
        "Associated Domains value"
      ],
      "excludedDomains": [
        "Excluded Domains value"
      ],
      "disableOnDemandUserOverride": true,
      "disconnectOnIdle": true,
      "disconnectOnIdleTimerInSeconds": 14,
      "proxyServer": {
        "@odata.type": "microsoft.graph.vpnProxyServer",
        "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
        "address": "Address value",
        "port": 4
      },
      "optInToDeviceIdSharing": true,
      "userDomain": "User Domain value",
      "strictEnforcement": true,
      "cloudName": "Cloud Name value",
      "excludeList": [
        "Exclude List value"
      ],
      "targetedMobileApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value"
    }
  ]
}
```




