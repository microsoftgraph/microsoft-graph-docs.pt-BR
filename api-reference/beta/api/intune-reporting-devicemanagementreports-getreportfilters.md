---
title: ação getReportFilters
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 57b0f0095ae5b85fce3fad3c72957df51175d313
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791332"
---
# <a name="getreportfilters-action"></a><span data-ttu-id="b6174-103">ação getReportFilters</span><span class="sxs-lookup"><span data-stu-id="b6174-103">getReportFilters action</span></span>

<span data-ttu-id="b6174-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6174-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6174-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b6174-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6174-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b6174-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6174-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6174-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6174-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6174-108">Prerequisites</span></span>
<span data-ttu-id="b6174-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6174-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6174-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6174-111">Permission type</span></span>|<span data-ttu-id="b6174-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6174-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6174-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6174-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6174-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="b6174-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b6174-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6174-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6174-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6174-116">Not supported.</span></span>|
|<span data-ttu-id="b6174-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6174-117">Application</span></span>|<span data-ttu-id="b6174-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="b6174-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6174-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6174-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getReportFilters
```

## <a name="request-headers"></a><span data-ttu-id="b6174-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6174-120">Request headers</span></span>
|<span data-ttu-id="b6174-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6174-121">Header</span></span>|<span data-ttu-id="b6174-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b6174-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6174-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6174-123">Authorization</span></span>|<span data-ttu-id="b6174-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6174-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6174-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b6174-125">Accept</span></span>|<span data-ttu-id="b6174-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6174-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6174-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6174-127">Request body</span></span>
<span data-ttu-id="b6174-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b6174-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b6174-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b6174-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b6174-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6174-130">Property</span></span>|<span data-ttu-id="b6174-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6174-131">Type</span></span>|<span data-ttu-id="b6174-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6174-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6174-133">nome</span><span class="sxs-lookup"><span data-stu-id="b6174-133">name</span></span>|<span data-ttu-id="b6174-134">String</span><span class="sxs-lookup"><span data-stu-id="b6174-134">String</span></span>|<span data-ttu-id="b6174-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6174-135">Not yet documented</span></span>|
|<span data-ttu-id="b6174-136">select</span><span class="sxs-lookup"><span data-stu-id="b6174-136">select</span></span>|<span data-ttu-id="b6174-137">String collection</span><span class="sxs-lookup"><span data-stu-id="b6174-137">String collection</span></span>|<span data-ttu-id="b6174-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6174-138">Not yet documented</span></span>|
|<span data-ttu-id="b6174-139">search</span><span class="sxs-lookup"><span data-stu-id="b6174-139">search</span></span>|<span data-ttu-id="b6174-140">String</span><span class="sxs-lookup"><span data-stu-id="b6174-140">String</span></span>|<span data-ttu-id="b6174-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6174-141">Not yet documented</span></span>|
|<span data-ttu-id="b6174-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="b6174-142">groupBy</span></span>|<span data-ttu-id="b6174-143">String collection</span><span class="sxs-lookup"><span data-stu-id="b6174-143">String collection</span></span>|<span data-ttu-id="b6174-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6174-144">Not yet documented</span></span>|
|<span data-ttu-id="b6174-145">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="b6174-145">orderBy</span></span>|<span data-ttu-id="b6174-146">String collection</span><span class="sxs-lookup"><span data-stu-id="b6174-146">String collection</span></span>|<span data-ttu-id="b6174-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6174-147">Not yet documented</span></span>|
|<span data-ttu-id="b6174-148">skip</span><span class="sxs-lookup"><span data-stu-id="b6174-148">skip</span></span>|<span data-ttu-id="b6174-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b6174-149">Int32</span></span>|<span data-ttu-id="b6174-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6174-150">Not yet documented</span></span>|
|<span data-ttu-id="b6174-151">top</span><span class="sxs-lookup"><span data-stu-id="b6174-151">top</span></span>|<span data-ttu-id="b6174-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b6174-152">Int32</span></span>|<span data-ttu-id="b6174-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6174-153">Not yet documented</span></span>|
|<span data-ttu-id="b6174-154">Identificação_da_sessão</span><span class="sxs-lookup"><span data-stu-id="b6174-154">sessionId</span></span>|<span data-ttu-id="b6174-155">String</span><span class="sxs-lookup"><span data-stu-id="b6174-155">String</span></span>|<span data-ttu-id="b6174-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6174-156">Not yet documented</span></span>|
|<span data-ttu-id="b6174-157">filter</span><span class="sxs-lookup"><span data-stu-id="b6174-157">filter</span></span>|<span data-ttu-id="b6174-158">String</span><span class="sxs-lookup"><span data-stu-id="b6174-158">String</span></span>|<span data-ttu-id="b6174-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b6174-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b6174-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6174-160">Response</span></span>
<span data-ttu-id="b6174-161">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e um fluxo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6174-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6174-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6174-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6174-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6174-163">Request</span></span>
<span data-ttu-id="b6174-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6174-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getReportFilters

Content-type: application/json
Content-length: 278

{
  "name": "Name value",
  "select": [
    "Select value"
  ],
  "search": "Search value",
  "groupBy": [
    "Group By value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "skip": 4,
  "top": 3,
  "sessionId": "Session Id value",
  "filter": "Filter value"
}
```

### <a name="response"></a><span data-ttu-id="b6174-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6174-165">Response</span></span>
<span data-ttu-id="b6174-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6174-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": "Z2V0UmVwb3J0RmlsdGVycyBJbnR1bmUgRG9jIFNhbXBsZSAxMzYxOTI0Mjkx"
}
```



