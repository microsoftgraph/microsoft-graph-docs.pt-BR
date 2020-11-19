---
title: Criar microsoftTunnelServer
description: Criar um novo objeto microsoftTunnelServer.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 146de9c8b03d2934ad6507b5adf2aecc3d778d75
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301401"
---
# <a name="create-microsofttunnelserver"></a><span data-ttu-id="0e52f-103">Criar microsoftTunnelServer</span><span class="sxs-lookup"><span data-stu-id="0e52f-103">Create microsoftTunnelServer</span></span>

<span data-ttu-id="0e52f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e52f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e52f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e52f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e52f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e52f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e52f-107">Criar um novo objeto [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) .</span><span class="sxs-lookup"><span data-stu-id="0e52f-107">Create a new [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0e52f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0e52f-108">Prerequisites</span></span>
<span data-ttu-id="0e52f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0e52f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e52f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0e52f-111">Permission type</span></span>|<span data-ttu-id="0e52f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0e52f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e52f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0e52f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e52f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e52f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0e52f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0e52f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e52f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0e52f-116">Not supported.</span></span>|
|<span data-ttu-id="0e52f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e52f-117">Application</span></span>|<span data-ttu-id="0e52f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e52f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e52f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0e52f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers
```

## <a name="request-headers"></a><span data-ttu-id="0e52f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0e52f-120">Request headers</span></span>
|<span data-ttu-id="0e52f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0e52f-121">Header</span></span>|<span data-ttu-id="0e52f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0e52f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e52f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0e52f-123">Authorization</span></span>|<span data-ttu-id="0e52f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0e52f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e52f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="0e52f-125">Accept</span></span>|<span data-ttu-id="0e52f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e52f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e52f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0e52f-127">Request body</span></span>
<span data-ttu-id="0e52f-128">No corpo da solicitação, forneça uma representação JSON do objeto microsoftTunnelServer.</span><span class="sxs-lookup"><span data-stu-id="0e52f-128">In the request body, supply a JSON representation for the microsoftTunnelServer object.</span></span>

<span data-ttu-id="0e52f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar microsoftTunnelServer.</span><span class="sxs-lookup"><span data-stu-id="0e52f-129">The following table shows the properties that are required when you create the microsoftTunnelServer.</span></span>

|<span data-ttu-id="0e52f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e52f-130">Property</span></span>|<span data-ttu-id="0e52f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e52f-131">Type</span></span>|<span data-ttu-id="0e52f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e52f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e52f-133">id</span><span class="sxs-lookup"><span data-stu-id="0e52f-133">id</span></span>|<span data-ttu-id="0e52f-134">String</span><span class="sxs-lookup"><span data-stu-id="0e52f-134">String</span></span>|<span data-ttu-id="0e52f-135">A ID do MicrosoftTunnelServer</span><span class="sxs-lookup"><span data-stu-id="0e52f-135">The MicrosoftTunnelServer's Id</span></span>|
|<span data-ttu-id="0e52f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0e52f-136">displayName</span></span>|<span data-ttu-id="0e52f-137">String</span><span class="sxs-lookup"><span data-stu-id="0e52f-137">String</span></span>|<span data-ttu-id="0e52f-138">O nome de exibição do MicrosoftTunnelServer</span><span class="sxs-lookup"><span data-stu-id="0e52f-138">The MicrosoftTunnelServer's display name</span></span>|
|<span data-ttu-id="0e52f-139">tunnelServerHealthStatus</span><span class="sxs-lookup"><span data-stu-id="0e52f-139">tunnelServerHealthStatus</span></span>|[<span data-ttu-id="0e52f-140">microsoftTunnelServerHealthStatus</span><span class="sxs-lookup"><span data-stu-id="0e52f-140">microsoftTunnelServerHealthStatus</span></span>](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|<span data-ttu-id="0e52f-141">O status de integridade do MicrosoftTunnelServer.</span><span class="sxs-lookup"><span data-stu-id="0e52f-141">The MicrosoftTunnelServer's health status.</span></span> <span data-ttu-id="0e52f-142">Os valores possíveis são: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.</span><span class="sxs-lookup"><span data-stu-id="0e52f-142">Possible values are: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.</span></span>|
|<span data-ttu-id="0e52f-143">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="0e52f-143">lastCheckinDateTime</span></span>|<span data-ttu-id="0e52f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e52f-144">DateTimeOffset</span></span>|<span data-ttu-id="0e52f-145">Quando o MicrosoftTunnelServer último check-in</span><span class="sxs-lookup"><span data-stu-id="0e52f-145">When the MicrosoftTunnelServer last checked in</span></span>|



## <a name="response"></a><span data-ttu-id="0e52f-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e52f-146">Response</span></span>
<span data-ttu-id="0e52f-147">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0e52f-147">If successful, this method returns a `201 Created` response code and a [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e52f-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0e52f-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="0e52f-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0e52f-149">Request</span></span>
<span data-ttu-id="0e52f-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0e52f-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers
Content-type: application/json
Content-length: 208

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "displayName": "Display Name value",
  "tunnelServerHealthStatus": "healthy",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
}
```

### <a name="response"></a><span data-ttu-id="0e52f-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="0e52f-151">Response</span></span>
<span data-ttu-id="0e52f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0e52f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 257

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "id": "b5cf0aee-0aee-b5cf-ee0a-cfb5ee0acfb5",
  "displayName": "Display Name value",
  "tunnelServerHealthStatus": "healthy",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
}
```




