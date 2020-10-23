---
title: Obter iosikEv2VpnConfiguration
description: Leia as propriedades e as relações do objeto iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3f32e0ea0a46ec49d8869721f9a73e53018b2399
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48689759"
---
# <a name="get-iosikev2vpnconfiguration"></a><span data-ttu-id="56ad4-103">Obter iosikEv2VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="56ad4-103">Get iosikEv2VpnConfiguration</span></span>

<span data-ttu-id="56ad4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56ad4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56ad4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="56ad4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56ad4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="56ad4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56ad4-107">Leia as propriedades e as relações do objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="56ad4-107">Read properties and relationships of the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="56ad4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="56ad4-108">Prerequisites</span></span>
<span data-ttu-id="56ad4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56ad4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56ad4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="56ad4-111">Permission type</span></span>|<span data-ttu-id="56ad4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="56ad4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56ad4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="56ad4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56ad4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="56ad4-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="56ad4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="56ad4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56ad4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="56ad4-116">Not supported.</span></span>|
|<span data-ttu-id="56ad4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="56ad4-117">Application</span></span>|<span data-ttu-id="56ad4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="56ad4-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="56ad4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="56ad4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56ad4-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="56ad4-120">Optional query parameters</span></span>
<span data-ttu-id="56ad4-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="56ad4-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56ad4-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="56ad4-122">Request headers</span></span>
|<span data-ttu-id="56ad4-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="56ad4-123">Header</span></span>|<span data-ttu-id="56ad4-124">Valor</span><span class="sxs-lookup"><span data-stu-id="56ad4-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56ad4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="56ad4-125">Authorization</span></span>|<span data-ttu-id="56ad4-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="56ad4-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56ad4-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="56ad4-127">Accept</span></span>|<span data-ttu-id="56ad4-128">application/json</span><span class="sxs-lookup"><span data-stu-id="56ad4-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56ad4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="56ad4-129">Request body</span></span>
<span data-ttu-id="56ad4-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="56ad4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56ad4-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="56ad4-131">Response</span></span>
<span data-ttu-id="56ad4-132">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="56ad4-132">If successful, this method returns a `200 OK` response code and [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56ad4-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="56ad4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="56ad4-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="56ad4-134">Request</span></span>
<span data-ttu-id="56ad4-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="56ad4-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="56ad4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="56ad4-136">Response</span></span>
<span data-ttu-id="56ad4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="56ad4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 5943

{
  "value": {
    "@odata.type": "#microsoft.graph.iosikEv2VpnConfiguration",
    "id": "b87b0327-0327-b87b-2703-7bb827037bb8",
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
    "excludedDomains": [
      "Excluded Domains value"
    ],
    "disableOnDemandUserOverride": true,
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
    "microsoftTunnelSiteId": "Microsoft Tunnel Site Id value",
    "childSecurityAssociationParameters": {
      "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
      "securityEncryptionAlgorithm": "des",
      "securityIntegrityAlgorithm": "sha1_96",
      "securityDiffieHellmanGroup": 10,
      "lifetimeInMinutes": 1
    },
    "clientAuthenticationType": "deviceAuthentication",
    "deadPeerDetectionRate": "none",
    "disableMobilityAndMultihoming": true,
    "disableRedirect": true,
    "enableCertificateRevocationCheck": true,
    "enableEAP": true,
    "enablePerfectForwardSecrecy": true,
    "enableUseInternalSubnetAttributes": true,
    "localIdentifier": "empty",
    "remoteIdentifier": "Remote Identifier value",
    "securityAssociationParameters": {
      "@odata.type": "microsoft.graph.iosVpnSecurityAssociationParameters",
      "securityEncryptionAlgorithm": "des",
      "securityIntegrityAlgorithm": "sha1_96",
      "securityDiffieHellmanGroup": 10,
      "lifetimeInMinutes": 1
    },
    "serverCertificateCommonName": "Server Certificate Common Name value",
    "serverCertificateIssuerCommonName": "Server Certificate Issuer Common Name value",
    "serverCertificateType": "ecdsa256",
    "sharedSecret": "Shared Secret value",
    "tlsMaximumVersion": "Tls Maximum Version value",
    "tlsMinimumVersion": "Tls Minimum Version value",
    "allowDefaultSecurityAssociationParameters": true,
    "allowDefaultChildSecurityAssociationParameters": true,
    "alwaysOnConfiguration": {
      "@odata.type": "microsoft.graph.appleVpnAlwaysOnConfiguration",
      "tunnelConfiguration": "cellular",
      "userToggleEnabled": true,
      "voicemailExceptionAction": "allowTrafficOutside",
      "airPrintExceptionAction": "allowTrafficOutside",
      "cellularExceptionAction": "allowTrafficOutside",
      "allowAllCaptiveNetworkPlugins": true,
      "allowedCaptiveNetworkPlugins": {
        "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins",
        "allowedBundleIdentifiers": [
          "Allowed Bundle Identifiers value"
        ]
      },
      "allowCaptiveWebSheet": true,
      "natKeepAliveIntervalInSeconds": 13,
      "natKeepAliveOffloadEnable": true
    },
    "enableAlwaysOnConfiguration": true,
    "mtuSizeInBytes": 14
  }
}
```





