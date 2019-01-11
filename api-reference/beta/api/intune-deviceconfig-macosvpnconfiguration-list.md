---
title: Lista macOSVpnConfigurations
description: Lista as propriedades e os relacionamentos dos objetos macOSVpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8d091ffce914fb257f21ae4afde18803a5ea0b6e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858244"
---
# <a name="list-macosvpnconfigurations"></a><span data-ttu-id="ecada-103">Lista macOSVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="ecada-103">List macOSVpnConfigurations</span></span>

> <span data-ttu-id="ecada-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ecada-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecada-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ecada-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ecada-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ecada-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ecada-107">Lista as propriedades e os relacionamentos dos objetos [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="ecada-107">List properties and relationships of the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ecada-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ecada-108">Prerequisites</span></span>
<span data-ttu-id="ecada-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ecada-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecada-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ecada-111">Permission type</span></span>|<span data-ttu-id="ecada-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ecada-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecada-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ecada-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ecada-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ecada-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ecada-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ecada-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecada-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecada-116">Not supported.</span></span>|
|<span data-ttu-id="ecada-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ecada-117">Application</span></span>|<span data-ttu-id="ecada-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ecada-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecada-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ecada-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ecada-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ecada-120">Request headers</span></span>
|<span data-ttu-id="ecada-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ecada-121">Header</span></span>|<span data-ttu-id="ecada-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ecada-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecada-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ecada-123">Authorization</span></span>|<span data-ttu-id="ecada-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ecada-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecada-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ecada-125">Accept</span></span>|<span data-ttu-id="ecada-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ecada-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecada-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ecada-127">Request body</span></span>
<span data-ttu-id="ecada-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ecada-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecada-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecada-129">Response</span></span>
<span data-ttu-id="ecada-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ecada-130">If successful, this method returns a `200 OK` response code and a collection of [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecada-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ecada-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ecada-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ecada-132">Request</span></span>
<span data-ttu-id="ecada-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ecada-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="ecada-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ecada-134">Response</span></span>
<span data-ttu-id="ecada-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ecada-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2334

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSVpnConfiguration",
      "id": "8ce00178-0178-8ce0-7801-e08c7801e08c",
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
      "optInToDeviceIdSharing": true
    }
  ]
}
```





