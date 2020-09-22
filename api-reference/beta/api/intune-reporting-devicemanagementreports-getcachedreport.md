---
title: ação getCachedReport
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 12972799b6bf1ac22379fef60ce2476215ea69a9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47980481"
---
# <a name="getcachedreport-action"></a><span data-ttu-id="29b8f-103">ação getCachedReport</span><span class="sxs-lookup"><span data-stu-id="29b8f-103">getCachedReport action</span></span>

<span data-ttu-id="29b8f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29b8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29b8f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="29b8f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29b8f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29b8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29b8f-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="29b8f-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29b8f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29b8f-108">Prerequisites</span></span>
<span data-ttu-id="29b8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29b8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29b8f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="29b8f-111">Permission type</span></span>|<span data-ttu-id="29b8f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="29b8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29b8f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="29b8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29b8f-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="29b8f-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="29b8f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="29b8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29b8f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="29b8f-116">Not supported.</span></span>|
|<span data-ttu-id="29b8f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="29b8f-117">Application</span></span>|<span data-ttu-id="29b8f-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="29b8f-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29b8f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29b8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getCachedReport
```

## <a name="request-headers"></a><span data-ttu-id="29b8f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29b8f-120">Request headers</span></span>
|<span data-ttu-id="29b8f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="29b8f-121">Header</span></span>|<span data-ttu-id="29b8f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="29b8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29b8f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="29b8f-123">Authorization</span></span>|<span data-ttu-id="29b8f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29b8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29b8f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="29b8f-125">Accept</span></span>|<span data-ttu-id="29b8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29b8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29b8f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29b8f-127">Request body</span></span>
<span data-ttu-id="29b8f-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="29b8f-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="29b8f-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="29b8f-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="29b8f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="29b8f-130">Property</span></span>|<span data-ttu-id="29b8f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="29b8f-131">Type</span></span>|<span data-ttu-id="29b8f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="29b8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29b8f-133">id</span><span class="sxs-lookup"><span data-stu-id="29b8f-133">id</span></span>|<span data-ttu-id="29b8f-134">String</span><span class="sxs-lookup"><span data-stu-id="29b8f-134">String</span></span>|<span data-ttu-id="29b8f-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="29b8f-135">Not yet documented</span></span>|
|<span data-ttu-id="29b8f-136">select</span><span class="sxs-lookup"><span data-stu-id="29b8f-136">select</span></span>|<span data-ttu-id="29b8f-137">String collection</span><span class="sxs-lookup"><span data-stu-id="29b8f-137">String collection</span></span>|<span data-ttu-id="29b8f-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="29b8f-138">Not yet documented</span></span>|
|<span data-ttu-id="29b8f-139">search</span><span class="sxs-lookup"><span data-stu-id="29b8f-139">search</span></span>|<span data-ttu-id="29b8f-140">String</span><span class="sxs-lookup"><span data-stu-id="29b8f-140">String</span></span>|<span data-ttu-id="29b8f-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="29b8f-141">Not yet documented</span></span>|
|<span data-ttu-id="29b8f-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="29b8f-142">groupBy</span></span>|<span data-ttu-id="29b8f-143">String collection</span><span class="sxs-lookup"><span data-stu-id="29b8f-143">String collection</span></span>|<span data-ttu-id="29b8f-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="29b8f-144">Not yet documented</span></span>|
|<span data-ttu-id="29b8f-145">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="29b8f-145">orderBy</span></span>|<span data-ttu-id="29b8f-146">String collection</span><span class="sxs-lookup"><span data-stu-id="29b8f-146">String collection</span></span>|<span data-ttu-id="29b8f-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="29b8f-147">Not yet documented</span></span>|
|<span data-ttu-id="29b8f-148">skip</span><span class="sxs-lookup"><span data-stu-id="29b8f-148">skip</span></span>|<span data-ttu-id="29b8f-149">Int32</span><span class="sxs-lookup"><span data-stu-id="29b8f-149">Int32</span></span>|<span data-ttu-id="29b8f-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="29b8f-150">Not yet documented</span></span>|
|<span data-ttu-id="29b8f-151">top</span><span class="sxs-lookup"><span data-stu-id="29b8f-151">top</span></span>|<span data-ttu-id="29b8f-152">Int32</span><span class="sxs-lookup"><span data-stu-id="29b8f-152">Int32</span></span>|<span data-ttu-id="29b8f-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="29b8f-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="29b8f-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="29b8f-154">Response</span></span>
<span data-ttu-id="29b8f-155">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e um fluxo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29b8f-155">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29b8f-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29b8f-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="29b8f-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29b8f-157">Request</span></span>
<span data-ttu-id="29b8f-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29b8f-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getCachedReport

Content-type: application/json
Content-length: 209

{
  "id": "Id value",
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
  "top": 3
}
```

### <a name="response"></a><span data-ttu-id="29b8f-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="29b8f-159">Response</span></span>
<span data-ttu-id="29b8f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="29b8f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": "Z2V0Q2FjaGVkUmVwb3J0IEludHVuZSBEb2MgU2FtcGxlIDc5MjIxODQ3OA=="
}
```






