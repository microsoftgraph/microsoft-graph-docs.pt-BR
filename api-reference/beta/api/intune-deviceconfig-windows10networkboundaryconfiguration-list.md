---
title: Listar windows10NetworkBoundaryConfigurations
description: Listar Propriedades e relações dos objetos windows10NetworkBoundaryConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 37edd55ac6a299f304d51b8e4d37746b3e1ebf8c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47972459"
---
# <a name="list-windows10networkboundaryconfigurations"></a><span data-ttu-id="96d0f-103">Listar windows10NetworkBoundaryConfigurations</span><span class="sxs-lookup"><span data-stu-id="96d0f-103">List windows10NetworkBoundaryConfigurations</span></span>

<span data-ttu-id="96d0f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96d0f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96d0f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="96d0f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96d0f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96d0f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96d0f-107">Listar Propriedades e relações dos objetos [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="96d0f-107">List properties and relationships of the [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96d0f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="96d0f-108">Prerequisites</span></span>
<span data-ttu-id="96d0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96d0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96d0f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96d0f-111">Permission type</span></span>|<span data-ttu-id="96d0f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="96d0f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96d0f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96d0f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96d0f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="96d0f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="96d0f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96d0f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96d0f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96d0f-116">Not supported.</span></span>|
|<span data-ttu-id="96d0f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96d0f-117">Application</span></span>|<span data-ttu-id="96d0f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="96d0f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96d0f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96d0f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="96d0f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="96d0f-120">Request headers</span></span>
|<span data-ttu-id="96d0f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="96d0f-121">Header</span></span>|<span data-ttu-id="96d0f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="96d0f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96d0f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="96d0f-123">Authorization</span></span>|<span data-ttu-id="96d0f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="96d0f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96d0f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="96d0f-125">Accept</span></span>|<span data-ttu-id="96d0f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96d0f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96d0f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96d0f-127">Request body</span></span>
<span data-ttu-id="96d0f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="96d0f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96d0f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="96d0f-129">Response</span></span>
<span data-ttu-id="96d0f-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="96d0f-130">If successful, this method returns a `200 OK` response code and a collection of [windows10NetworkBoundaryConfiguration](../resources/intune-deviceconfig-windows10networkboundaryconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96d0f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="96d0f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="96d0f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="96d0f-132">Request</span></span>
<span data-ttu-id="96d0f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="96d0f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="96d0f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="96d0f-134">Response</span></span>
<span data-ttu-id="96d0f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="96d0f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2368

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10NetworkBoundaryConfiguration",
      "id": "afbc9e01-9e01-afbc-019e-bcaf019ebcaf",
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
      "windowsNetworkIsolationPolicy": {
        "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy",
        "enterpriseNetworkDomainNames": [
          "Enterprise Network Domain Names value"
        ],
        "enterpriseCloudResources": [
          {
            "@odata.type": "microsoft.graph.proxiedDomain",
            "ipAddressOrFQDN": "Ip Address Or FQDN value",
            "proxy": "Proxy value"
          }
        ],
        "enterpriseIPRanges": [
          {
            "@odata.type": "microsoft.graph.ipRange"
          }
        ],
        "enterpriseInternalProxyServers": [
          "Enterprise Internal Proxy Servers value"
        ],
        "enterpriseIPRangesAreAuthoritative": true,
        "enterpriseProxyServers": [
          "Enterprise Proxy Servers value"
        ],
        "enterpriseProxyServersAreAuthoritative": true,
        "neutralDomainResources": [
          "Neutral Domain Resources value"
        ]
      }
    }
  ]
}
```






