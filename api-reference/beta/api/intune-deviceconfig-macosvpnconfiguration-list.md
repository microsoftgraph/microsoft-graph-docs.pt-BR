---
title: Listar macOSVpnConfigurations
description: Listar Propriedades e relações dos objetos macOSVpnConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f93768906dc3a6c82957620b7ce502f38c5f30d5
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30984650"
---
# <a name="list-macosvpnconfigurations"></a><span data-ttu-id="eb520-103">Listar macOSVpnConfigurations</span><span class="sxs-lookup"><span data-stu-id="eb520-103">List macOSVpnConfigurations</span></span>

> <span data-ttu-id="eb520-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb520-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb520-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb520-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb520-106">Listar Propriedades e relações dos objetos [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="eb520-106">List properties and relationships of the [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eb520-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="eb520-107">Prerequisites</span></span>
<span data-ttu-id="eb520-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb520-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb520-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb520-110">Permission type</span></span>|<span data-ttu-id="eb520-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="eb520-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eb520-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb520-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eb520-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb520-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="eb520-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb520-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eb520-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb520-115">Not supported.</span></span>|
|<span data-ttu-id="eb520-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb520-116">Application</span></span>|<span data-ttu-id="eb520-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb520-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eb520-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb520-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="eb520-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="eb520-119">Request headers</span></span>
|<span data-ttu-id="eb520-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="eb520-120">Header</span></span>|<span data-ttu-id="eb520-121">Valor</span><span class="sxs-lookup"><span data-stu-id="eb520-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eb520-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="eb520-122">Authorization</span></span>|<span data-ttu-id="eb520-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="eb520-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eb520-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="eb520-124">Accept</span></span>|<span data-ttu-id="eb520-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eb520-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eb520-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb520-126">Request body</span></span>
<span data-ttu-id="eb520-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb520-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb520-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb520-128">Response</span></span>
<span data-ttu-id="eb520-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb520-129">If successful, this method returns a `200 OK` response code and a collection of [macOSVpnConfiguration](../resources/intune-deviceconfig-macosvpnconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb520-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb520-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="eb520-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb520-131">Request</span></span>
<span data-ttu-id="eb520-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="eb520-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="eb520-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb520-133">Response</span></span>
<span data-ttu-id="eb520-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb520-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




