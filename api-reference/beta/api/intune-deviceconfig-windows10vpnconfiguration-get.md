---
title: Obter windows10VpnConfiguration
description: Leia as propriedades e as relações do objeto windows10VpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9091db452f0da1081478f824212703eb5fa2969
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146603"
---
# <a name="get-windows10vpnconfiguration"></a><span data-ttu-id="8f032-103">Obter windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="8f032-103">Get windows10VpnConfiguration</span></span>

> <span data-ttu-id="8f032-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8f032-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f032-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8f032-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f032-106">Leia as propriedades e as relações do objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="8f032-106">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f032-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8f032-107">Prerequisites</span></span>
<span data-ttu-id="8f032-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="8f032-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8f032-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8f032-110">Permission type</span></span>|<span data-ttu-id="8f032-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8f032-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f032-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8f032-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8f032-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f032-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="8f032-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8f032-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f032-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f032-115">Not supported.</span></span>|
|<span data-ttu-id="8f032-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8f032-116">Application</span></span>|<span data-ttu-id="8f032-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8f032-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f032-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8f032-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8f032-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8f032-119">Optional query parameters</span></span>
<span data-ttu-id="8f032-120">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8f032-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8f032-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8f032-121">Request headers</span></span>
|<span data-ttu-id="8f032-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8f032-122">Header</span></span>|<span data-ttu-id="8f032-123">Valor</span><span class="sxs-lookup"><span data-stu-id="8f032-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f032-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8f032-124">Authorization</span></span>|<span data-ttu-id="8f032-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8f032-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f032-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8f032-126">Accept</span></span>|<span data-ttu-id="8f032-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8f032-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f032-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8f032-128">Request body</span></span>
<span data-ttu-id="8f032-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8f032-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f032-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f032-130">Response</span></span>
<span data-ttu-id="8f032-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8f032-131">If successful, this method returns a `200 OK` response code and [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f032-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8f032-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f032-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8f032-133">Request</span></span>
<span data-ttu-id="8f032-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8f032-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="8f032-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="8f032-135">Response</span></span>
<span data-ttu-id="8f032-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8f032-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3814

{
  "value": {
    "@odata.type": "#microsoft.graph.windows10VpnConfiguration",
    "id": "c23c9727-9727-c23c-2797-3cc227973cc2",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "connectionName": "Connection Name value",
    "servers": [
      {
        "@odata.type": "microsoft.graph.vpnServer",
        "description": "Description value",
        "address": "Address value",
        "isDefaultServer": true
      }
    ],
    "customXml": "Y3VzdG9tWG1s",
    "profileTarget": "device",
    "connectionType": "f5EdgeClient",
    "enableSplitTunneling": true,
    "enableAlwaysOn": true,
    "enableDeviceTunnel": true,
    "enableDnsRegistration": true,
    "dnsSuffixes": [
      "Dns Suffixes value"
    ],
    "authenticationMethod": "usernameAndPassword",
    "rememberUserCredentials": true,
    "enableConditionalAccess": true,
    "enableSingleSignOnWithAlternateCertificate": true,
    "singleSignOnEku": {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    },
    "singleSignOnIssuerHash": "Single Sign On Issuer Hash value",
    "eapXml": "ZWFwWG1s",
    "proxyServer": {
      "@odata.type": "microsoft.graph.windows10VpnProxyServer",
      "automaticConfigurationScriptUrl": "https://example.com/automaticConfigurationScriptUrl/",
      "address": "Address value",
      "port": 4,
      "bypassProxyServerForLocalAddress": true
    },
    "associatedApps": [
      {
        "@odata.type": "microsoft.graph.windows10AssociatedApps",
        "appType": "universal",
        "identifier": "Identifier value"
      }
    ],
    "onlyAssociatedAppsCanUseConnection": true,
    "windowsInformationProtectionDomain": "Windows Information Protection Domain value",
    "trafficRules": [
      {
        "@odata.type": "microsoft.graph.vpnTrafficRule",
        "name": "Name value",
        "protocols": 9,
        "localPortRanges": [
          {
            "@odata.type": "microsoft.graph.numberRange",
            "lowerNumber": 11,
            "upperNumber": 11
          }
        ],
        "remotePortRanges": [
          {
            "@odata.type": "microsoft.graph.numberRange",
            "lowerNumber": 11,
            "upperNumber": 11
          }
        ],
        "localAddressRanges": [
          {
            "@odata.type": "microsoft.graph.iPv4Range",
            "lowerAddress": "Lower Address value",
            "upperAddress": "Upper Address value"
          }
        ],
        "remoteAddressRanges": [
          {
            "@odata.type": "microsoft.graph.iPv4Range",
            "lowerAddress": "Lower Address value",
            "upperAddress": "Upper Address value"
          }
        ],
        "appId": "App Id value",
        "appType": "desktop",
        "routingPolicyType": "splitTunnel",
        "claims": "Claims value"
      }
    ],
    "routes": [
      {
        "@odata.type": "microsoft.graph.vpnRoute",
        "destinationPrefix": "Destination Prefix value",
        "prefixSize": 10
      }
    ],
    "dnsRules": [
      {
        "@odata.type": "microsoft.graph.vpnDnsRule",
        "name": "Name value",
        "servers": [
          "Servers value"
        ],
        "proxyServerUri": "Proxy Server Uri value",
        "autoTrigger": true,
        "persistent": true
      }
    ],
    "trustedNetworkDomains": [
      "Trusted Network Domains value"
    ]
  }
}
```




