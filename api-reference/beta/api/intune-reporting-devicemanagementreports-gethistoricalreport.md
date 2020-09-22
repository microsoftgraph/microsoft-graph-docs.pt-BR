---
title: ação getHistoricalReport
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 00ed73dcd5364b30250ecf0ff4dbf35d6f975ada
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020045"
---
# <a name="gethistoricalreport-action"></a><span data-ttu-id="10a02-103">ação getHistoricalReport</span><span class="sxs-lookup"><span data-stu-id="10a02-103">getHistoricalReport action</span></span>

<span data-ttu-id="10a02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10a02-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10a02-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="10a02-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10a02-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10a02-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10a02-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="10a02-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10a02-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="10a02-108">Prerequisites</span></span>
<span data-ttu-id="10a02-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10a02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10a02-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="10a02-111">Permission type</span></span>|<span data-ttu-id="10a02-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="10a02-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10a02-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="10a02-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10a02-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="10a02-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="10a02-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="10a02-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10a02-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="10a02-116">Not supported.</span></span>|
|<span data-ttu-id="10a02-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="10a02-117">Application</span></span>|<span data-ttu-id="10a02-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="10a02-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="10a02-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="10a02-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getHistoricalReport
```

## <a name="request-headers"></a><span data-ttu-id="10a02-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="10a02-120">Request headers</span></span>
|<span data-ttu-id="10a02-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="10a02-121">Header</span></span>|<span data-ttu-id="10a02-122">Valor</span><span class="sxs-lookup"><span data-stu-id="10a02-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10a02-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="10a02-123">Authorization</span></span>|<span data-ttu-id="10a02-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10a02-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10a02-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="10a02-125">Accept</span></span>|<span data-ttu-id="10a02-126">application/json</span><span class="sxs-lookup"><span data-stu-id="10a02-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10a02-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="10a02-127">Request body</span></span>
<span data-ttu-id="10a02-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="10a02-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="10a02-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="10a02-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="10a02-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10a02-130">Property</span></span>|<span data-ttu-id="10a02-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="10a02-131">Type</span></span>|<span data-ttu-id="10a02-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="10a02-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10a02-133">nome</span><span class="sxs-lookup"><span data-stu-id="10a02-133">name</span></span>|<span data-ttu-id="10a02-134">String</span><span class="sxs-lookup"><span data-stu-id="10a02-134">String</span></span>|<span data-ttu-id="10a02-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="10a02-135">Not yet documented</span></span>|
|<span data-ttu-id="10a02-136">select</span><span class="sxs-lookup"><span data-stu-id="10a02-136">select</span></span>|<span data-ttu-id="10a02-137">String collection</span><span class="sxs-lookup"><span data-stu-id="10a02-137">String collection</span></span>|<span data-ttu-id="10a02-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="10a02-138">Not yet documented</span></span>|
|<span data-ttu-id="10a02-139">search</span><span class="sxs-lookup"><span data-stu-id="10a02-139">search</span></span>|<span data-ttu-id="10a02-140">String</span><span class="sxs-lookup"><span data-stu-id="10a02-140">String</span></span>|<span data-ttu-id="10a02-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="10a02-141">Not yet documented</span></span>|
|<span data-ttu-id="10a02-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="10a02-142">groupBy</span></span>|<span data-ttu-id="10a02-143">String collection</span><span class="sxs-lookup"><span data-stu-id="10a02-143">String collection</span></span>|<span data-ttu-id="10a02-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="10a02-144">Not yet documented</span></span>|
|<span data-ttu-id="10a02-145">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="10a02-145">orderBy</span></span>|<span data-ttu-id="10a02-146">String collection</span><span class="sxs-lookup"><span data-stu-id="10a02-146">String collection</span></span>|<span data-ttu-id="10a02-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="10a02-147">Not yet documented</span></span>|
|<span data-ttu-id="10a02-148">skip</span><span class="sxs-lookup"><span data-stu-id="10a02-148">skip</span></span>|<span data-ttu-id="10a02-149">Int32</span><span class="sxs-lookup"><span data-stu-id="10a02-149">Int32</span></span>|<span data-ttu-id="10a02-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="10a02-150">Not yet documented</span></span>|
|<span data-ttu-id="10a02-151">top</span><span class="sxs-lookup"><span data-stu-id="10a02-151">top</span></span>|<span data-ttu-id="10a02-152">Int32</span><span class="sxs-lookup"><span data-stu-id="10a02-152">Int32</span></span>|<span data-ttu-id="10a02-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="10a02-153">Not yet documented</span></span>|
|<span data-ttu-id="10a02-154">filter</span><span class="sxs-lookup"><span data-stu-id="10a02-154">filter</span></span>|<span data-ttu-id="10a02-155">String</span><span class="sxs-lookup"><span data-stu-id="10a02-155">String</span></span>|<span data-ttu-id="10a02-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="10a02-156">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="10a02-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="10a02-157">Response</span></span>
<span data-ttu-id="10a02-158">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e um fluxo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="10a02-158">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10a02-159">Exemplo</span><span class="sxs-lookup"><span data-stu-id="10a02-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="10a02-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="10a02-160">Request</span></span>
<span data-ttu-id="10a02-161">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="10a02-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getHistoricalReport

Content-type: application/json
Content-length: 242

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
  "filter": "Filter value"
}
```

### <a name="response"></a><span data-ttu-id="10a02-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="10a02-162">Response</span></span>
<span data-ttu-id="10a02-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="10a02-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 83

{
  "value": "Z2V0SGlzdG9yaWNhbFJlcG9ydCBJbnR1bmUgRG9jIFNhbXBsZSAxNjE5NjA4MTY0"
}
```






