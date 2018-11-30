---
title: Lista iosVpnConfigurations
description: Lista as propriedades e os relacionamentos dos objetos iosVpnConfiguration.
ms.openlocfilehash: dba55598a3ce7b01b871a5d8605a1cf18891ebdf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033027"
---
# <a name="list-iosvpnconfigurations"></a><span data-ttu-id="1f45d-103">Lista iosVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="1f45d-103">List iosVpnConfigurations</span></span>

> <span data-ttu-id="1f45d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1f45d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f45d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1f45d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f45d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1f45d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f45d-107">Lista as propriedades e os relacionamentos dos objetos [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1f45d-107">List properties and relationships of the [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1f45d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1f45d-108">Prerequisites</span></span>
<span data-ttu-id="1f45d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1f45d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f45d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1f45d-111">Permission type</span></span>|<span data-ttu-id="1f45d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1f45d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f45d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1f45d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f45d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1f45d-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1f45d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1f45d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f45d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f45d-116">Not supported.</span></span>|
|<span data-ttu-id="1f45d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f45d-117">Application</span></span>|<span data-ttu-id="1f45d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1f45d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f45d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1f45d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1f45d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1f45d-120">Request headers</span></span>
|<span data-ttu-id="1f45d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1f45d-121">Header</span></span>|<span data-ttu-id="1f45d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="1f45d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f45d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f45d-123">Authorization</span></span>|<span data-ttu-id="1f45d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1f45d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f45d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1f45d-125">Accept</span></span>|<span data-ttu-id="1f45d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f45d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f45d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1f45d-127">Request body</span></span>
<span data-ttu-id="1f45d-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1f45d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1f45d-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f45d-129">Response</span></span>
<span data-ttu-id="1f45d-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1f45d-130">If successful, this method returns a `200 OK` response code and a collection of [iosVpnConfiguration](../resources/intune-deviceconfig-iosvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f45d-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1f45d-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1f45d-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1f45d-132">Request</span></span>
<span data-ttu-id="1f45d-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1f45d-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="1f45d-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1f45d-134">Response</span></span>
<span data-ttu-id="1f45d-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1f45d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2547

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
      ]
    }
  ]
}
```





