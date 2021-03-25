---
title: Atualizar microsoftTunnelServerLogCollectionResponse
description: Atualize as propriedades de um objeto microsoftTunnelServerLogCollectionResponse.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df112324b5ad51cd8a3d0bb6893e8789f24449fe
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51152968"
---
# <a name="update-microsofttunnelserverlogcollectionresponse"></a><span data-ttu-id="e20e4-103">Atualizar microsoftTunnelServerLogCollectionResponse</span><span class="sxs-lookup"><span data-stu-id="e20e4-103">Update microsoftTunnelServerLogCollectionResponse</span></span>

<span data-ttu-id="e20e4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e20e4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e20e4-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e20e4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e20e4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e20e4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e20e4-107">Atualize as propriedades de um [objeto microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)</span><span class="sxs-lookup"><span data-stu-id="e20e4-107">Update the properties of a [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e20e4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e20e4-108">Prerequisites</span></span>
<span data-ttu-id="e20e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e20e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e20e4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e20e4-111">Permission type</span></span>|<span data-ttu-id="e20e4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e20e4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e20e4-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e20e4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e20e4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e20e4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e20e4-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e20e4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e20e4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e20e4-116">Not supported.</span></span>|
|<span data-ttu-id="e20e4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e20e4-117">Application</span></span>|<span data-ttu-id="e20e4-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e20e4-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e20e4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e20e4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/microsoftTunnelServerLogCollectionResponses/{microsoftTunnelServerLogCollectionResponseId}
```

## <a name="request-headers"></a><span data-ttu-id="e20e4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e20e4-120">Request headers</span></span>
|<span data-ttu-id="e20e4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e20e4-121">Header</span></span>|<span data-ttu-id="e20e4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e20e4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e20e4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e20e4-123">Authorization</span></span>|<span data-ttu-id="e20e4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e20e4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e20e4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e20e4-125">Accept</span></span>|<span data-ttu-id="e20e4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e20e4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e20e4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e20e4-127">Request body</span></span>
<span data-ttu-id="e20e4-128">No corpo da solicitação, fornece uma representação JSON para o [objeto microsoftTunnelServerLogCollectionResponse.](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md)</span><span class="sxs-lookup"><span data-stu-id="e20e4-128">In the request body, supply a JSON representation for the [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) object.</span></span>

<span data-ttu-id="e20e4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md).</span><span class="sxs-lookup"><span data-stu-id="e20e4-129">The following table shows the properties that are required when you create the [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md).</span></span>

|<span data-ttu-id="e20e4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e20e4-130">Property</span></span>|<span data-ttu-id="e20e4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e20e4-131">Type</span></span>|<span data-ttu-id="e20e4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e20e4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e20e4-133">id</span><span class="sxs-lookup"><span data-stu-id="e20e4-133">id</span></span>|<span data-ttu-id="e20e4-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e20e4-134">String</span></span>|<span data-ttu-id="e20e4-135">A ID exclusiva da entidade</span><span class="sxs-lookup"><span data-stu-id="e20e4-135">The unique ID of the entity</span></span>|
|<span data-ttu-id="e20e4-136">status</span><span class="sxs-lookup"><span data-stu-id="e20e4-136">status</span></span>|[<span data-ttu-id="e20e4-137">microsoftTunnelLogCollectionStatus</span><span class="sxs-lookup"><span data-stu-id="e20e4-137">microsoftTunnelLogCollectionStatus</span></span>](../resources/intune-mstunnel-microsofttunnellogcollectionstatus.md)|<span data-ttu-id="e20e4-138">O status do conjunto de log.</span><span class="sxs-lookup"><span data-stu-id="e20e4-138">The status of log collection.</span></span> <span data-ttu-id="e20e4-139">Os valores possíveis são: `pending`, `completed`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="e20e4-139">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="e20e4-140">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e20e4-140">startDateTime</span></span>|<span data-ttu-id="e20e4-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e20e4-141">DateTimeOffset</span></span>|<span data-ttu-id="e20e4-142">A hora de início dos logs coletados</span><span class="sxs-lookup"><span data-stu-id="e20e4-142">The start time of the logs collected</span></span> |
|<span data-ttu-id="e20e4-143">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e20e4-143">endDateTime</span></span>|<span data-ttu-id="e20e4-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e20e4-144">DateTimeOffset</span></span>|<span data-ttu-id="e20e4-145">A hora de término dos logs coletados</span><span class="sxs-lookup"><span data-stu-id="e20e4-145">The end time of the logs collected</span></span>|
|<span data-ttu-id="e20e4-146">sizeInBytes</span><span class="sxs-lookup"><span data-stu-id="e20e4-146">sizeInBytes</span></span>|<span data-ttu-id="e20e4-147">Int64</span><span class="sxs-lookup"><span data-stu-id="e20e4-147">Int64</span></span>|<span data-ttu-id="e20e4-148">O tamanho dos logs em bytes</span><span class="sxs-lookup"><span data-stu-id="e20e4-148">The size of the logs in bytes</span></span>|



## <a name="response"></a><span data-ttu-id="e20e4-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="e20e4-149">Response</span></span>
<span data-ttu-id="e20e4-150">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e20e4-150">If successful, this method returns a `200 OK` response code and an updated [microsoftTunnelServerLogCollectionResponse](../resources/intune-mstunnel-microsofttunnelserverlogcollectionresponse.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e20e4-151">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e20e4-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="e20e4-152">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e20e4-152">Request</span></span>
<span data-ttu-id="e20e4-153">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e20e4-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelServerLogCollectionResponses/{microsoftTunnelServerLogCollectionResponseId}
Content-type: application/json
Content-length: 244

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServerLogCollectionResponse",
  "status": "completed",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
  "sizeInBytes": 11
}
```

### <a name="response"></a><span data-ttu-id="e20e4-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="e20e4-154">Response</span></span>
<span data-ttu-id="e20e4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e20e4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 293

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServerLogCollectionResponse",
  "id": "05dcc2e9-c2e9-05dc-e9c2-dc05e9c2dc05",
  "status": "completed",
  "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
  "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
  "sizeInBytes": 11
}
```




