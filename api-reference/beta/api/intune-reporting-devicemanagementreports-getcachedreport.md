---
title: ação getCachedReport
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bf2b229601bb7126b7e29f9036f032a4d28b88e4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459145"
---
# <a name="getcachedreport-action"></a><span data-ttu-id="d2447-103">ação getCachedReport</span><span class="sxs-lookup"><span data-stu-id="d2447-103">getCachedReport action</span></span>

<span data-ttu-id="d2447-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d2447-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2447-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d2447-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2447-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2447-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2447-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d2447-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2447-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d2447-108">Prerequisites</span></span>
<span data-ttu-id="d2447-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d2447-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2447-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d2447-111">Permission type</span></span>|<span data-ttu-id="d2447-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d2447-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2447-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d2447-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d2447-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="d2447-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="d2447-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d2447-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2447-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d2447-116">Not supported.</span></span>|
|<span data-ttu-id="d2447-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d2447-117">Application</span></span>|<span data-ttu-id="d2447-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="d2447-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2447-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d2447-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getCachedReport
```

## <a name="request-headers"></a><span data-ttu-id="d2447-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d2447-120">Request headers</span></span>
|<span data-ttu-id="d2447-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d2447-121">Header</span></span>|<span data-ttu-id="d2447-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d2447-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2447-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d2447-123">Authorization</span></span>|<span data-ttu-id="d2447-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d2447-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2447-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d2447-125">Accept</span></span>|<span data-ttu-id="d2447-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2447-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2447-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d2447-127">Request body</span></span>
<span data-ttu-id="d2447-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d2447-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d2447-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d2447-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d2447-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2447-130">Property</span></span>|<span data-ttu-id="d2447-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2447-131">Type</span></span>|<span data-ttu-id="d2447-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2447-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2447-133">id</span><span class="sxs-lookup"><span data-stu-id="d2447-133">id</span></span>|<span data-ttu-id="d2447-134">String</span><span class="sxs-lookup"><span data-stu-id="d2447-134">String</span></span>|<span data-ttu-id="d2447-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d2447-135">Not yet documented</span></span>|
|<span data-ttu-id="d2447-136">select</span><span class="sxs-lookup"><span data-stu-id="d2447-136">select</span></span>|<span data-ttu-id="d2447-137">String collection</span><span class="sxs-lookup"><span data-stu-id="d2447-137">String collection</span></span>|<span data-ttu-id="d2447-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d2447-138">Not yet documented</span></span>|
|<span data-ttu-id="d2447-139">search</span><span class="sxs-lookup"><span data-stu-id="d2447-139">search</span></span>|<span data-ttu-id="d2447-140">String</span><span class="sxs-lookup"><span data-stu-id="d2447-140">String</span></span>|<span data-ttu-id="d2447-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d2447-141">Not yet documented</span></span>|
|<span data-ttu-id="d2447-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="d2447-142">groupBy</span></span>|<span data-ttu-id="d2447-143">String collection</span><span class="sxs-lookup"><span data-stu-id="d2447-143">String collection</span></span>|<span data-ttu-id="d2447-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d2447-144">Not yet documented</span></span>|
|<span data-ttu-id="d2447-145">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="d2447-145">orderBy</span></span>|<span data-ttu-id="d2447-146">String collection</span><span class="sxs-lookup"><span data-stu-id="d2447-146">String collection</span></span>|<span data-ttu-id="d2447-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d2447-147">Not yet documented</span></span>|
|<span data-ttu-id="d2447-148">skip</span><span class="sxs-lookup"><span data-stu-id="d2447-148">skip</span></span>|<span data-ttu-id="d2447-149">Int32</span><span class="sxs-lookup"><span data-stu-id="d2447-149">Int32</span></span>|<span data-ttu-id="d2447-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d2447-150">Not yet documented</span></span>|
|<span data-ttu-id="d2447-151">top</span><span class="sxs-lookup"><span data-stu-id="d2447-151">top</span></span>|<span data-ttu-id="d2447-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d2447-152">Int32</span></span>|<span data-ttu-id="d2447-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d2447-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d2447-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2447-154">Response</span></span>
<span data-ttu-id="d2447-155">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e um fluxo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d2447-155">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2447-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d2447-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2447-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d2447-157">Request</span></span>
<span data-ttu-id="d2447-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d2447-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d2447-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="d2447-159">Response</span></span>
<span data-ttu-id="d2447-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d2447-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 54

{
  "value": "<Unknown Primitive Type Edm.Stream>"
}
```





