---
title: Atualizar o microsoftTunnelServer
description: Atualize as propriedades de um objeto microsoftTunnelServer.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8e878a43325dcad36f615f8eefc41e74f6a85fd3
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51864855"
---
# <a name="update-microsofttunnelserver"></a><span data-ttu-id="07df7-103">Atualizar o microsoftTunnelServer</span><span class="sxs-lookup"><span data-stu-id="07df7-103">Update microsoftTunnelServer</span></span>

<span data-ttu-id="07df7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07df7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07df7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="07df7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07df7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07df7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07df7-107">Atualize as propriedades de um [objeto microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)</span><span class="sxs-lookup"><span data-stu-id="07df7-107">Update the properties of a [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07df7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="07df7-108">Prerequisites</span></span>
<span data-ttu-id="07df7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="07df7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07df7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="07df7-111">Permission type</span></span>|<span data-ttu-id="07df7-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="07df7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07df7-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="07df7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="07df7-114">DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07df7-114">DeviceManagementConfiguration.ReadWrite.All, MicrosoftTunnelGateway.Read.All, MicrosoftTunnelGateway.ReadWrite.All</span></span>|
|<span data-ttu-id="07df7-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="07df7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07df7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="07df7-116">Not supported.</span></span>|
|<span data-ttu-id="07df7-117">Application</span><span class="sxs-lookup"><span data-stu-id="07df7-117">Application</span></span>|<span data-ttu-id="07df7-118">MicrosoftTunnelGateway.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07df7-118">MicrosoftTunnelGateway.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07df7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="07df7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers/{microsoftTunnelServerId}
```

## <a name="request-headers"></a><span data-ttu-id="07df7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="07df7-120">Request headers</span></span>
|<span data-ttu-id="07df7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="07df7-121">Header</span></span>|<span data-ttu-id="07df7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="07df7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07df7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="07df7-123">Authorization</span></span>|<span data-ttu-id="07df7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07df7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07df7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="07df7-125">Accept</span></span>|<span data-ttu-id="07df7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="07df7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07df7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="07df7-127">Request body</span></span>
<span data-ttu-id="07df7-128">No corpo da solicitação, fornece uma representação JSON para o [objeto microsoftTunnelServer.](../resources/intune-mstunnel-microsofttunnelserver.md)</span><span class="sxs-lookup"><span data-stu-id="07df7-128">In the request body, supply a JSON representation for the [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object.</span></span>

<span data-ttu-id="07df7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md).</span><span class="sxs-lookup"><span data-stu-id="07df7-129">The following table shows the properties that are required when you create the [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md).</span></span>

|<span data-ttu-id="07df7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07df7-130">Property</span></span>|<span data-ttu-id="07df7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="07df7-131">Type</span></span>|<span data-ttu-id="07df7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="07df7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07df7-133">id</span><span class="sxs-lookup"><span data-stu-id="07df7-133">id</span></span>|<span data-ttu-id="07df7-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07df7-134">String</span></span>|<span data-ttu-id="07df7-135">Id do MicrosoftTunnelServer</span><span class="sxs-lookup"><span data-stu-id="07df7-135">The MicrosoftTunnelServer's Id</span></span>|
|<span data-ttu-id="07df7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="07df7-136">displayName</span></span>|<span data-ttu-id="07df7-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="07df7-137">String</span></span>|<span data-ttu-id="07df7-138">O nome de exibição do MicrosoftTunnelServer</span><span class="sxs-lookup"><span data-stu-id="07df7-138">The MicrosoftTunnelServer's display name</span></span>|
|<span data-ttu-id="07df7-139">tunnelServerHealthStatus</span><span class="sxs-lookup"><span data-stu-id="07df7-139">tunnelServerHealthStatus</span></span>|[<span data-ttu-id="07df7-140">microsoftTunnelServerHealthStatus</span><span class="sxs-lookup"><span data-stu-id="07df7-140">microsoftTunnelServerHealthStatus</span></span>](../resources/intune-mstunnel-microsofttunnelserverhealthstatus.md)|<span data-ttu-id="07df7-141">O status de saúde do MicrosoftTunnelServer.</span><span class="sxs-lookup"><span data-stu-id="07df7-141">The MicrosoftTunnelServer's health status.</span></span> <span data-ttu-id="07df7-142">Os valores possíveis são: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.</span><span class="sxs-lookup"><span data-stu-id="07df7-142">Possible values are: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.</span></span>|
|<span data-ttu-id="07df7-143">lastCheckinDateTime</span><span class="sxs-lookup"><span data-stu-id="07df7-143">lastCheckinDateTime</span></span>|<span data-ttu-id="07df7-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07df7-144">DateTimeOffset</span></span>|<span data-ttu-id="07df7-145">Quando o MicrosoftTunnelServer entrou pela última vez</span><span class="sxs-lookup"><span data-stu-id="07df7-145">When the MicrosoftTunnelServer last checked in</span></span>|



## <a name="response"></a><span data-ttu-id="07df7-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="07df7-146">Response</span></span>
<span data-ttu-id="07df7-147">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="07df7-147">If successful, this method returns a `200 OK` response code and an updated [microsoftTunnelServer](../resources/intune-mstunnel-microsofttunnelserver.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07df7-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="07df7-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="07df7-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="07df7-149">Request</span></span>
<span data-ttu-id="07df7-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="07df7-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers/{microsoftTunnelServerId}
Content-type: application/json
Content-length: 208

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "displayName": "Display Name value",
  "tunnelServerHealthStatus": "healthy",
  "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
}
```

### <a name="response"></a><span data-ttu-id="07df7-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="07df7-151">Response</span></span>
<span data-ttu-id="07df7-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="07df7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




