---
title: Listar iosikEv2VpnConfigurations
description: Listar propriedades e relações dos objetos iosikEv2VpnConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6917b9b64eee72f7424b187cd825a5e5d94f2555
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50156053"
---
# <a name="list-iosikev2vpnconfigurations"></a><span data-ttu-id="57a40-103">Listar iosikEv2VpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="57a40-103">List iosikEv2VpnConfigurations</span></span>

<span data-ttu-id="57a40-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57a40-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57a40-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57a40-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57a40-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57a40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57a40-107">Listar propriedades e relações dos [objetos iosikEv2VpnConfiguration.](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="57a40-107">List properties and relationships of the [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57a40-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="57a40-108">Prerequisites</span></span>
<span data-ttu-id="57a40-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="57a40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57a40-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="57a40-111">Permission type</span></span>|<span data-ttu-id="57a40-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="57a40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57a40-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="57a40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57a40-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="57a40-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="57a40-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="57a40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57a40-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="57a40-116">Not supported.</span></span>|
|<span data-ttu-id="57a40-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="57a40-117">Application</span></span>|<span data-ttu-id="57a40-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="57a40-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57a40-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="57a40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="57a40-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="57a40-120">Request headers</span></span>
|<span data-ttu-id="57a40-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="57a40-121">Header</span></span>|<span data-ttu-id="57a40-122">Valor</span><span class="sxs-lookup"><span data-stu-id="57a40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57a40-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="57a40-123">Authorization</span></span>|<span data-ttu-id="57a40-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="57a40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57a40-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="57a40-125">Accept</span></span>|<span data-ttu-id="57a40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57a40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57a40-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="57a40-127">Request body</span></span>
<span data-ttu-id="57a40-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="57a40-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="57a40-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="57a40-129">Response</span></span>
<span data-ttu-id="57a40-130">Se bem-sucedido, este método retorna um código de resposta e uma coleção de `200 OK` [objetos iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="57a40-130">If successful, this method returns a `200 OK` response code and a collection of [iosikEv2VpnConfiguration](../resources/intune-deviceconfig-iosikev2vpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57a40-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="57a40-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="57a40-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="57a40-132">Request</span></span>
<span data-ttu-id="57a40-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="57a40-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="57a40-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="57a40-134">Response</span></span>
<span data-ttu-id="57a40-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="57a40-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 6357

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
      "providerType": "appProxy",
      "associatedDomains": [
        "Associated Domains value"
      ],
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
  ]
}
```




