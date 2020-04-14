---
title: ação getCachedReport
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d3dfd7497f8e0cd530d24c23760fccba459c6b02
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454378"
---
# <a name="getcachedreport-action"></a><span data-ttu-id="b539c-103">ação getCachedReport</span><span class="sxs-lookup"><span data-stu-id="b539c-103">getCachedReport action</span></span>

<span data-ttu-id="b539c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b539c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b539c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b539c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b539c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b539c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b539c-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b539c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b539c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b539c-108">Prerequisites</span></span>
<span data-ttu-id="b539c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b539c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b539c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b539c-111">Permission type</span></span>|<span data-ttu-id="b539c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b539c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b539c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b539c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b539c-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="b539c-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b539c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b539c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b539c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b539c-116">Not supported.</span></span>|
|<span data-ttu-id="b539c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b539c-117">Application</span></span>|<span data-ttu-id="b539c-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="b539c-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b539c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b539c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getCachedReport
```

## <a name="request-headers"></a><span data-ttu-id="b539c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b539c-120">Request headers</span></span>
|<span data-ttu-id="b539c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b539c-121">Header</span></span>|<span data-ttu-id="b539c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b539c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b539c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b539c-123">Authorization</span></span>|<span data-ttu-id="b539c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b539c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b539c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b539c-125">Accept</span></span>|<span data-ttu-id="b539c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b539c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b539c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b539c-127">Request body</span></span>
<span data-ttu-id="b539c-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="b539c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="b539c-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="b539c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="b539c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b539c-130">Property</span></span>|<span data-ttu-id="b539c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b539c-131">Type</span></span>|<span data-ttu-id="b539c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b539c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b539c-133">id</span><span class="sxs-lookup"><span data-stu-id="b539c-133">id</span></span>|<span data-ttu-id="b539c-134">String</span><span class="sxs-lookup"><span data-stu-id="b539c-134">String</span></span>|<span data-ttu-id="b539c-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b539c-135">Not yet documented</span></span>|
|<span data-ttu-id="b539c-136">select</span><span class="sxs-lookup"><span data-stu-id="b539c-136">select</span></span>|<span data-ttu-id="b539c-137">String collection</span><span class="sxs-lookup"><span data-stu-id="b539c-137">String collection</span></span>|<span data-ttu-id="b539c-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b539c-138">Not yet documented</span></span>|
|<span data-ttu-id="b539c-139">search</span><span class="sxs-lookup"><span data-stu-id="b539c-139">search</span></span>|<span data-ttu-id="b539c-140">String</span><span class="sxs-lookup"><span data-stu-id="b539c-140">String</span></span>|<span data-ttu-id="b539c-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b539c-141">Not yet documented</span></span>|
|<span data-ttu-id="b539c-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="b539c-142">groupBy</span></span>|<span data-ttu-id="b539c-143">String collection</span><span class="sxs-lookup"><span data-stu-id="b539c-143">String collection</span></span>|<span data-ttu-id="b539c-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b539c-144">Not yet documented</span></span>|
|<span data-ttu-id="b539c-145">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="b539c-145">orderBy</span></span>|<span data-ttu-id="b539c-146">String collection</span><span class="sxs-lookup"><span data-stu-id="b539c-146">String collection</span></span>|<span data-ttu-id="b539c-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b539c-147">Not yet documented</span></span>|
|<span data-ttu-id="b539c-148">skip</span><span class="sxs-lookup"><span data-stu-id="b539c-148">skip</span></span>|<span data-ttu-id="b539c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="b539c-149">Int32</span></span>|<span data-ttu-id="b539c-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b539c-150">Not yet documented</span></span>|
|<span data-ttu-id="b539c-151">top</span><span class="sxs-lookup"><span data-stu-id="b539c-151">top</span></span>|<span data-ttu-id="b539c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="b539c-152">Int32</span></span>|<span data-ttu-id="b539c-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b539c-153">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b539c-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="b539c-154">Response</span></span>
<span data-ttu-id="b539c-155">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e um fluxo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b539c-155">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b539c-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b539c-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="b539c-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b539c-157">Request</span></span>
<span data-ttu-id="b539c-158">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b539c-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b539c-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="b539c-159">Response</span></span>
<span data-ttu-id="b539c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b539c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 54

{
  "value": "<Unknown Primitive Type Edm.Stream>"
}
```



