---
title: Listar microsoftTunnelServers
description: Listar Propriedades e relações dos objetos microsoftTunnelServer.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 84dee839a77f3d3125506dcc68ba88f43c0ced6c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301397"
---
# <a name="list-microsofttunnelservers"></a><span data-ttu-id="75bcf-103">Listar microsoftTunnelServers</span><span class="sxs-lookup"><span data-stu-id="75bcf-103">List microsoftTunnelServers</span></span>

<span data-ttu-id="75bcf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75bcf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75bcf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="75bcf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75bcf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75bcf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75bcf-107">Listar Propriedades e relações dos objetos [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) .</span><span class="sxs-lookup"><span data-stu-id="75bcf-107">List properties and relationships of the [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="75bcf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="75bcf-108">Prerequisites</span></span>
<span data-ttu-id="75bcf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="75bcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="75bcf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="75bcf-111">Permission type</span></span>|<span data-ttu-id="75bcf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="75bcf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="75bcf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="75bcf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="75bcf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="75bcf-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="75bcf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="75bcf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="75bcf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="75bcf-116">Not supported.</span></span>|
|<span data-ttu-id="75bcf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="75bcf-117">Application</span></span>|<span data-ttu-id="75bcf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="75bcf-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="75bcf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="75bcf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers
```

## <a name="request-headers"></a><span data-ttu-id="75bcf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="75bcf-120">Request headers</span></span>
|<span data-ttu-id="75bcf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="75bcf-121">Header</span></span>|<span data-ttu-id="75bcf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="75bcf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="75bcf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="75bcf-123">Authorization</span></span>|<span data-ttu-id="75bcf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="75bcf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="75bcf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="75bcf-125">Accept</span></span>|<span data-ttu-id="75bcf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="75bcf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="75bcf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="75bcf-127">Request body</span></span>
<span data-ttu-id="75bcf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="75bcf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="75bcf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="75bcf-129">Response</span></span>
<span data-ttu-id="75bcf-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="75bcf-130">If successful, this method returns a `200 OK` response code and a collection of [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="75bcf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="75bcf-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="75bcf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="75bcf-132">Request</span></span>
<span data-ttu-id="75bcf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="75bcf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers
```

### <a name="response"></a><span data-ttu-id="75bcf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="75bcf-134">Response</span></span>
<span data-ttu-id="75bcf-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="75bcf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.microsoftTunnelServer",
      "id": "b5cf0aee-0aee-b5cf-ee0a-cfb5ee0acfb5",
      "displayName": "Display Name value",
      "tunnelServerHealthStatus": "healthy",
      "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
    }
  ]
}
```




