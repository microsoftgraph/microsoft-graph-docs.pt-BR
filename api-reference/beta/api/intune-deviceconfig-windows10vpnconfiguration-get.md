---
title: Obter windows10VpnConfiguration
description: Leia as propriedades e os relacionamentos do objeto windows10VpnConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e19a473e7db98b1272af184698397ed1c368d32d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417011"
---
# <a name="get-windows10vpnconfiguration"></a><span data-ttu-id="dce2a-103">Obter windows10VpnConfiguration</span><span class="sxs-lookup"><span data-stu-id="dce2a-103">Get windows10VpnConfiguration</span></span>

> <span data-ttu-id="dce2a-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="dce2a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="dce2a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dce2a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dce2a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="dce2a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dce2a-107">Leia as propriedades e os relacionamentos do objeto [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="dce2a-107">Read properties and relationships of the [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dce2a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dce2a-108">Prerequisites</span></span>
<span data-ttu-id="dce2a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="dce2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="dce2a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dce2a-111">Permission type</span></span>|<span data-ttu-id="dce2a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dce2a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dce2a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dce2a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dce2a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dce2a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dce2a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dce2a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dce2a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dce2a-116">Not supported.</span></span>|
|<span data-ttu-id="dce2a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dce2a-117">Application</span></span>|<span data-ttu-id="dce2a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dce2a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dce2a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dce2a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dce2a-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="dce2a-120">Optional query parameters</span></span>
<span data-ttu-id="dce2a-121">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="dce2a-121">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dce2a-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dce2a-122">Request headers</span></span>
|<span data-ttu-id="dce2a-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dce2a-123">Header</span></span>|<span data-ttu-id="dce2a-124">Valor</span><span class="sxs-lookup"><span data-stu-id="dce2a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dce2a-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="dce2a-125">Authorization</span></span>|<span data-ttu-id="dce2a-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dce2a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dce2a-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dce2a-127">Accept</span></span>|<span data-ttu-id="dce2a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="dce2a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dce2a-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dce2a-129">Request body</span></span>
<span data-ttu-id="dce2a-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dce2a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dce2a-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="dce2a-131">Response</span></span>
<span data-ttu-id="dce2a-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="dce2a-132">If successful, this method returns a `200 OK` response code and [windows10VpnConfiguration](../resources/intune-deviceconfig-windows10vpnconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dce2a-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dce2a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="dce2a-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dce2a-134">Request</span></span>
<span data-ttu-id="dce2a-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dce2a-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="dce2a-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="dce2a-136">Response</span></span>
<span data-ttu-id="dce2a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dce2a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




