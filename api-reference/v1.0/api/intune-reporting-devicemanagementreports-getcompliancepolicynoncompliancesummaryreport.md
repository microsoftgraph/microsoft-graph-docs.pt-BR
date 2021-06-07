---
title: ação getCompliancePolicyNonComplianceSummaryReport
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 2aa7b2b4493947c29a2161218f1b3fd7f10ca8d8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748886"
---
# <a name="getcompliancepolicynoncompliancesummaryreport-action"></a><span data-ttu-id="2fe95-103">ação getCompliancePolicyNonComplianceSummaryReport</span><span class="sxs-lookup"><span data-stu-id="2fe95-103">getCompliancePolicyNonComplianceSummaryReport action</span></span>

<span data-ttu-id="2fe95-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fe95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2fe95-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2fe95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fe95-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2fe95-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2fe95-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2fe95-107">Prerequisites</span></span>
<span data-ttu-id="2fe95-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2fe95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fe95-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2fe95-110">Permission type</span></span>|<span data-ttu-id="2fe95-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2fe95-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fe95-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2fe95-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2fe95-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fe95-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2fe95-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2fe95-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fe95-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2fe95-115">Not supported.</span></span>|
|<span data-ttu-id="2fe95-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2fe95-116">Application</span></span>|<span data-ttu-id="2fe95-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fe95-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fe95-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2fe95-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getCompliancePolicyNonComplianceSummaryReport
```

## <a name="request-headers"></a><span data-ttu-id="2fe95-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2fe95-119">Request headers</span></span>
|<span data-ttu-id="2fe95-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2fe95-120">Header</span></span>|<span data-ttu-id="2fe95-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2fe95-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fe95-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2fe95-122">Authorization</span></span>|<span data-ttu-id="2fe95-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2fe95-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fe95-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2fe95-124">Accept</span></span>|<span data-ttu-id="2fe95-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2fe95-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fe95-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2fe95-126">Request body</span></span>
<span data-ttu-id="2fe95-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="2fe95-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2fe95-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="2fe95-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2fe95-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fe95-129">Property</span></span>|<span data-ttu-id="2fe95-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fe95-130">Type</span></span>|<span data-ttu-id="2fe95-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fe95-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fe95-132">nome</span><span class="sxs-lookup"><span data-stu-id="2fe95-132">name</span></span>|<span data-ttu-id="2fe95-133">String</span><span class="sxs-lookup"><span data-stu-id="2fe95-133">String</span></span>|<span data-ttu-id="2fe95-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2fe95-134">Not yet documented</span></span>|
|<span data-ttu-id="2fe95-135">select</span><span class="sxs-lookup"><span data-stu-id="2fe95-135">select</span></span>|<span data-ttu-id="2fe95-136">String collection</span><span class="sxs-lookup"><span data-stu-id="2fe95-136">String collection</span></span>|<span data-ttu-id="2fe95-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2fe95-137">Not yet documented</span></span>|
|<span data-ttu-id="2fe95-138">search</span><span class="sxs-lookup"><span data-stu-id="2fe95-138">search</span></span>|<span data-ttu-id="2fe95-139">String</span><span class="sxs-lookup"><span data-stu-id="2fe95-139">String</span></span>|<span data-ttu-id="2fe95-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2fe95-140">Not yet documented</span></span>|
|<span data-ttu-id="2fe95-141">groupBy</span><span class="sxs-lookup"><span data-stu-id="2fe95-141">groupBy</span></span>|<span data-ttu-id="2fe95-142">String collection</span><span class="sxs-lookup"><span data-stu-id="2fe95-142">String collection</span></span>|<span data-ttu-id="2fe95-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2fe95-143">Not yet documented</span></span>|
|<span data-ttu-id="2fe95-144">orderBy</span><span class="sxs-lookup"><span data-stu-id="2fe95-144">orderBy</span></span>|<span data-ttu-id="2fe95-145">String collection</span><span class="sxs-lookup"><span data-stu-id="2fe95-145">String collection</span></span>|<span data-ttu-id="2fe95-146">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2fe95-146">Not yet documented</span></span>|
|<span data-ttu-id="2fe95-147">skip</span><span class="sxs-lookup"><span data-stu-id="2fe95-147">skip</span></span>|<span data-ttu-id="2fe95-148">Int32</span><span class="sxs-lookup"><span data-stu-id="2fe95-148">Int32</span></span>|<span data-ttu-id="2fe95-149">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2fe95-149">Not yet documented</span></span>|
|<span data-ttu-id="2fe95-150">top</span><span class="sxs-lookup"><span data-stu-id="2fe95-150">top</span></span>|<span data-ttu-id="2fe95-151">Int32</span><span class="sxs-lookup"><span data-stu-id="2fe95-151">Int32</span></span>|<span data-ttu-id="2fe95-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2fe95-152">Not yet documented</span></span>|
|<span data-ttu-id="2fe95-153">sessionId</span><span class="sxs-lookup"><span data-stu-id="2fe95-153">sessionId</span></span>|<span data-ttu-id="2fe95-154">String</span><span class="sxs-lookup"><span data-stu-id="2fe95-154">String</span></span>|<span data-ttu-id="2fe95-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2fe95-155">Not yet documented</span></span>|
|<span data-ttu-id="2fe95-156">filter</span><span class="sxs-lookup"><span data-stu-id="2fe95-156">filter</span></span>|<span data-ttu-id="2fe95-157">String</span><span class="sxs-lookup"><span data-stu-id="2fe95-157">String</span></span>|<span data-ttu-id="2fe95-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2fe95-158">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2fe95-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fe95-159">Response</span></span>
<span data-ttu-id="2fe95-160">Se tiver êxito, essa ação retornará `200 OK` um código de resposta e um Stream no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2fe95-160">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fe95-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2fe95-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="2fe95-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2fe95-162">Request</span></span>
<span data-ttu-id="2fe95-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2fe95-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/reports/getCompliancePolicyNonComplianceSummaryReport

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

### <a name="response"></a><span data-ttu-id="2fe95-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="2fe95-164">Response</span></span>
<span data-ttu-id="2fe95-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2fe95-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 119

{
  "value": "Z2V0Q29tcGxpYW5jZVBvbGljeU5vbkNvbXBsaWFuY2VTdW1tYXJ5UmVwb3J0IEludHVuZSBEb2MgU2FtcGxlIDg4MTYwMDMxNQ=="
}
```




