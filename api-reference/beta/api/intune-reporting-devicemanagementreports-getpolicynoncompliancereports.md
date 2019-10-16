---
title: ação getPolicyNoncomplianceReports
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 31e516228060df44fe45005801c490667d0e299e
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537209"
---
# <a name="getpolicynoncompliancereports-action"></a><span data-ttu-id="3125f-103">ação getPolicyNoncomplianceReports</span><span class="sxs-lookup"><span data-stu-id="3125f-103">getPolicyNoncomplianceReports action</span></span>

> <span data-ttu-id="3125f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3125f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3125f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3125f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3125f-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3125f-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3125f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3125f-107">Prerequisites</span></span>
<span data-ttu-id="3125f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3125f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3125f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3125f-110">Permission type</span></span>|<span data-ttu-id="3125f-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3125f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3125f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3125f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3125f-113">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="3125f-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3125f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3125f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3125f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3125f-115">Not supported.</span></span>|
|<span data-ttu-id="3125f-116">Application</span><span class="sxs-lookup"><span data-stu-id="3125f-116">Application</span></span>|<span data-ttu-id="3125f-117">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="3125f-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3125f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3125f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getPolicyNoncomplianceReports
```

## <a name="request-headers"></a><span data-ttu-id="3125f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3125f-119">Request headers</span></span>
|<span data-ttu-id="3125f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3125f-120">Header</span></span>|<span data-ttu-id="3125f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3125f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3125f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3125f-122">Authorization</span></span>|<span data-ttu-id="3125f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3125f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3125f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3125f-124">Accept</span></span>|<span data-ttu-id="3125f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3125f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3125f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3125f-126">Request body</span></span>
<span data-ttu-id="3125f-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3125f-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3125f-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3125f-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3125f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3125f-129">Property</span></span>|<span data-ttu-id="3125f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3125f-130">Type</span></span>|<span data-ttu-id="3125f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3125f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3125f-132">name</span><span class="sxs-lookup"><span data-stu-id="3125f-132">name</span></span>|<span data-ttu-id="3125f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3125f-133">String</span></span>|<span data-ttu-id="3125f-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3125f-134">Not yet documented</span></span>|
|<span data-ttu-id="3125f-135">select</span><span class="sxs-lookup"><span data-stu-id="3125f-135">select</span></span>|<span data-ttu-id="3125f-136">String collection</span><span class="sxs-lookup"><span data-stu-id="3125f-136">String collection</span></span>|<span data-ttu-id="3125f-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3125f-137">Not yet documented</span></span>|
|<span data-ttu-id="3125f-138">search</span><span class="sxs-lookup"><span data-stu-id="3125f-138">search</span></span>|<span data-ttu-id="3125f-139">String</span><span class="sxs-lookup"><span data-stu-id="3125f-139">String</span></span>|<span data-ttu-id="3125f-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3125f-140">Not yet documented</span></span>|
|<span data-ttu-id="3125f-141">groupBy</span><span class="sxs-lookup"><span data-stu-id="3125f-141">groupBy</span></span>|<span data-ttu-id="3125f-142">String collection</span><span class="sxs-lookup"><span data-stu-id="3125f-142">String collection</span></span>|<span data-ttu-id="3125f-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3125f-143">Not yet documented</span></span>|
|<span data-ttu-id="3125f-144">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="3125f-144">orderBy</span></span>|<span data-ttu-id="3125f-145">String collection</span><span class="sxs-lookup"><span data-stu-id="3125f-145">String collection</span></span>|<span data-ttu-id="3125f-146">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3125f-146">Not yet documented</span></span>|
|<span data-ttu-id="3125f-147">skip</span><span class="sxs-lookup"><span data-stu-id="3125f-147">skip</span></span>|<span data-ttu-id="3125f-148">Int32</span><span class="sxs-lookup"><span data-stu-id="3125f-148">Int32</span></span>|<span data-ttu-id="3125f-149">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3125f-149">Not yet documented</span></span>|
|<span data-ttu-id="3125f-150">top</span><span class="sxs-lookup"><span data-stu-id="3125f-150">top</span></span>|<span data-ttu-id="3125f-151">Int32</span><span class="sxs-lookup"><span data-stu-id="3125f-151">Int32</span></span>|<span data-ttu-id="3125f-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3125f-152">Not yet documented</span></span>|
|<span data-ttu-id="3125f-153">Identificação_da_sessão</span><span class="sxs-lookup"><span data-stu-id="3125f-153">sessionId</span></span>|<span data-ttu-id="3125f-154">String</span><span class="sxs-lookup"><span data-stu-id="3125f-154">String</span></span>|<span data-ttu-id="3125f-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3125f-155">Not yet documented</span></span>|
|<span data-ttu-id="3125f-156">filter</span><span class="sxs-lookup"><span data-stu-id="3125f-156">filter</span></span>|<span data-ttu-id="3125f-157">String</span><span class="sxs-lookup"><span data-stu-id="3125f-157">String</span></span>|<span data-ttu-id="3125f-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3125f-158">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3125f-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="3125f-159">Response</span></span>
<span data-ttu-id="3125f-160">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e um fluxo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3125f-160">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3125f-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3125f-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="3125f-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3125f-162">Request</span></span>
<span data-ttu-id="3125f-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3125f-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getPolicyNoncomplianceReports

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

### <a name="response"></a><span data-ttu-id="3125f-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="3125f-164">Response</span></span>
<span data-ttu-id="3125f-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3125f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 54

{
  "value": "<Unknown Primitive Type Edm.Stream>"
}
```






