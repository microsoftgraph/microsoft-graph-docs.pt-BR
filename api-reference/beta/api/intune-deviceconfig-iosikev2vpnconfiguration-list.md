---
title: Listar iosikEv2VpnConfigurations
description: Listar Propriedades e relações dos objetos iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dfdfe22363140d5567af531c411262205a789230
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123103"
---
# <a name="list-iosikev2vpnconfigurations"></a><span data-ttu-id="5cb5e-103">Listar iosikEv2VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="5cb5e-103">List iosikEv2VpnConfigurations</span></span>

<span data-ttu-id="5cb5e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cb5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5cb5e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5cb5e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cb5e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5cb5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cb5e-107">Listar Propriedades e relações dos objetos [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5cb5e-107">List properties and relationships of the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5cb5e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5cb5e-108">Prerequisites</span></span>
<span data-ttu-id="5cb5e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5cb5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cb5e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5cb5e-111">Permission type</span></span>|<span data-ttu-id="5cb5e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5cb5e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cb5e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5cb5e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5cb5e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5cb5e-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5cb5e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5cb5e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cb5e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5cb5e-116">Not supported.</span></span>|
|<span data-ttu-id="5cb5e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5cb5e-117">Application</span></span>|<span data-ttu-id="5cb5e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5cb5e-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cb5e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5cb5e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5cb5e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5cb5e-120">Request headers</span></span>
|<span data-ttu-id="5cb5e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5cb5e-121">Header</span></span>|<span data-ttu-id="5cb5e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5cb5e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cb5e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5cb5e-123">Authorization</span></span>|<span data-ttu-id="5cb5e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5cb5e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cb5e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5cb5e-125">Accept</span></span>|<span data-ttu-id="5cb5e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5cb5e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cb5e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5cb5e-127">Request body</span></span>
<span data-ttu-id="5cb5e-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="5cb5e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5cb5e-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cb5e-129">Response</span></span>
<span data-ttu-id="5cb5e-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5cb5e-130">If successful, this method returns a `200 OK` response code and a collection of [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cb5e-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5cb5e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cb5e-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5cb5e-132">Request</span></span>
<span data-ttu-id="5cb5e-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5cb5e-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="5cb5e-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="5cb5e-134">Response</span></span>
<span data-ttu-id="5cb5e-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5cb5e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 6070

{
  "value": [
    {
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
      "proxyServer": {
        "@odata.type": "microsoft.graph.vpnProxyServer",
        "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
        "address": "Address value",
        "port": 4
      },
      "optInToDeviceIdSharing": true,
      "providerType": "appProxy",
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
      "enableAlwaysOnConfiguration": true
    }
  ]
}
```



