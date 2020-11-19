---
title: Listar microsoftTunnelConfigurations
description: Listar Propriedades e relações dos objetos microsoftTunnelConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ab1de746c6b289083ceb7256cc8382df36a0f7d2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241224"
---
# <a name="list-microsofttunnelconfigurations"></a><span data-ttu-id="77fdf-103">Listar microsoftTunnelConfigurations</span><span class="sxs-lookup"><span data-stu-id="77fdf-103">List microsoftTunnelConfigurations</span></span>

<span data-ttu-id="77fdf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77fdf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77fdf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="77fdf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77fdf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="77fdf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77fdf-107">Listar Propriedades e relações dos objetos [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="77fdf-107">List properties and relationships of the [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77fdf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="77fdf-108">Prerequisites</span></span>
<span data-ttu-id="77fdf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77fdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77fdf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77fdf-111">Permission type</span></span>|<span data-ttu-id="77fdf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="77fdf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77fdf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77fdf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77fdf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="77fdf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="77fdf-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77fdf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77fdf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77fdf-116">Not supported.</span></span>|
|<span data-ttu-id="77fdf-117">Application</span><span class="sxs-lookup"><span data-stu-id="77fdf-117">Application</span></span>|<span data-ttu-id="77fdf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="77fdf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="77fdf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77fdf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="77fdf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77fdf-120">Request headers</span></span>
|<span data-ttu-id="77fdf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77fdf-121">Header</span></span>|<span data-ttu-id="77fdf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="77fdf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77fdf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="77fdf-123">Authorization</span></span>|<span data-ttu-id="77fdf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77fdf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77fdf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="77fdf-125">Accept</span></span>|<span data-ttu-id="77fdf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77fdf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77fdf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77fdf-127">Request body</span></span>
<span data-ttu-id="77fdf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="77fdf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77fdf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="77fdf-129">Response</span></span>
<span data-ttu-id="77fdf-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77fdf-130">If successful, this method returns a `200 OK` response code and a collection of [microsoftTunnelConfiguration](../resources/intune-mstunnel-microsofttunnelconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77fdf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77fdf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="77fdf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77fdf-132">Request</span></span>
<span data-ttu-id="77fdf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77fdf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelConfigurations
```

### <a name="response"></a><span data-ttu-id="77fdf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="77fdf-134">Response</span></span>
<span data-ttu-id="77fdf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77fdf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 950

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
      "id": "b8bdb469-b469-b8bd-69b4-bdb869b4bdb8",
      "displayName": "Display Name value",
      "description": "Description value",
      "network": "Network value",
      "dnsServers": [
        "Dns Servers value"
      ],
      "defaultDomainSuffix": "Default Domain Suffix value",
      "routesInclude": [
        "Routes Include value"
      ],
      "routesExclude": [
        "Routes Exclude value"
      ],
      "splitDNS": [
        "Split DNS value"
      ],
      "listenPort": 10,
      "advancedSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ],
      "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




