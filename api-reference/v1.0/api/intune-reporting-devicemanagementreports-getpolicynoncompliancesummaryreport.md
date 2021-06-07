---
title: ação getPolicyNonComplianceSummaryReport
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 57f42660be5aa664ad58069473a38c194c58ea5f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757446"
---
# <a name="getpolicynoncompliancesummaryreport-action"></a><span data-ttu-id="ebdfd-103">ação getPolicyNonComplianceSummaryReport</span><span class="sxs-lookup"><span data-stu-id="ebdfd-103">getPolicyNonComplianceSummaryReport action</span></span>

<span data-ttu-id="ebdfd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ebdfd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ebdfd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ebdfd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ebdfd-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ebdfd-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ebdfd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ebdfd-107">Prerequisites</span></span>
<span data-ttu-id="ebdfd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ebdfd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ebdfd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ebdfd-110">Permission type</span></span>|<span data-ttu-id="ebdfd-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ebdfd-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebdfd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ebdfd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ebdfd-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebdfd-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ebdfd-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ebdfd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebdfd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ebdfd-115">Not supported.</span></span>|
|<span data-ttu-id="ebdfd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ebdfd-116">Application</span></span>|<span data-ttu-id="ebdfd-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebdfd-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebdfd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ebdfd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getPolicyNonComplianceSummaryReport
```

## <a name="request-headers"></a><span data-ttu-id="ebdfd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ebdfd-119">Request headers</span></span>
|<span data-ttu-id="ebdfd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ebdfd-120">Header</span></span>|<span data-ttu-id="ebdfd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ebdfd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebdfd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ebdfd-122">Authorization</span></span>|<span data-ttu-id="ebdfd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ebdfd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebdfd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ebdfd-124">Accept</span></span>|<span data-ttu-id="ebdfd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ebdfd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebdfd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ebdfd-126">Request body</span></span>
<span data-ttu-id="ebdfd-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="ebdfd-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ebdfd-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="ebdfd-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ebdfd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ebdfd-129">Property</span></span>|<span data-ttu-id="ebdfd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ebdfd-130">Type</span></span>|<span data-ttu-id="ebdfd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ebdfd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebdfd-132">nome</span><span class="sxs-lookup"><span data-stu-id="ebdfd-132">name</span></span>|<span data-ttu-id="ebdfd-133">String</span><span class="sxs-lookup"><span data-stu-id="ebdfd-133">String</span></span>|<span data-ttu-id="ebdfd-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ebdfd-134">Not yet documented</span></span>|
|<span data-ttu-id="ebdfd-135">select</span><span class="sxs-lookup"><span data-stu-id="ebdfd-135">select</span></span>|<span data-ttu-id="ebdfd-136">String collection</span><span class="sxs-lookup"><span data-stu-id="ebdfd-136">String collection</span></span>|<span data-ttu-id="ebdfd-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ebdfd-137">Not yet documented</span></span>|
|<span data-ttu-id="ebdfd-138">search</span><span class="sxs-lookup"><span data-stu-id="ebdfd-138">search</span></span>|<span data-ttu-id="ebdfd-139">String</span><span class="sxs-lookup"><span data-stu-id="ebdfd-139">String</span></span>|<span data-ttu-id="ebdfd-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ebdfd-140">Not yet documented</span></span>|
|<span data-ttu-id="ebdfd-141">groupBy</span><span class="sxs-lookup"><span data-stu-id="ebdfd-141">groupBy</span></span>|<span data-ttu-id="ebdfd-142">String collection</span><span class="sxs-lookup"><span data-stu-id="ebdfd-142">String collection</span></span>|<span data-ttu-id="ebdfd-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ebdfd-143">Not yet documented</span></span>|
|<span data-ttu-id="ebdfd-144">orderBy</span><span class="sxs-lookup"><span data-stu-id="ebdfd-144">orderBy</span></span>|<span data-ttu-id="ebdfd-145">String collection</span><span class="sxs-lookup"><span data-stu-id="ebdfd-145">String collection</span></span>|<span data-ttu-id="ebdfd-146">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ebdfd-146">Not yet documented</span></span>|
|<span data-ttu-id="ebdfd-147">skip</span><span class="sxs-lookup"><span data-stu-id="ebdfd-147">skip</span></span>|<span data-ttu-id="ebdfd-148">Int32</span><span class="sxs-lookup"><span data-stu-id="ebdfd-148">Int32</span></span>|<span data-ttu-id="ebdfd-149">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ebdfd-149">Not yet documented</span></span>|
|<span data-ttu-id="ebdfd-150">top</span><span class="sxs-lookup"><span data-stu-id="ebdfd-150">top</span></span>|<span data-ttu-id="ebdfd-151">Int32</span><span class="sxs-lookup"><span data-stu-id="ebdfd-151">Int32</span></span>|<span data-ttu-id="ebdfd-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ebdfd-152">Not yet documented</span></span>|
|<span data-ttu-id="ebdfd-153">sessionId</span><span class="sxs-lookup"><span data-stu-id="ebdfd-153">sessionId</span></span>|<span data-ttu-id="ebdfd-154">String</span><span class="sxs-lookup"><span data-stu-id="ebdfd-154">String</span></span>|<span data-ttu-id="ebdfd-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ebdfd-155">Not yet documented</span></span>|
|<span data-ttu-id="ebdfd-156">filter</span><span class="sxs-lookup"><span data-stu-id="ebdfd-156">filter</span></span>|<span data-ttu-id="ebdfd-157">String</span><span class="sxs-lookup"><span data-stu-id="ebdfd-157">String</span></span>|<span data-ttu-id="ebdfd-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ebdfd-158">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ebdfd-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebdfd-159">Response</span></span>
<span data-ttu-id="ebdfd-160">Se tiver êxito, essa ação retornará `200 OK` um código de resposta e um Stream no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ebdfd-160">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebdfd-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ebdfd-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="ebdfd-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ebdfd-162">Request</span></span>
<span data-ttu-id="ebdfd-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ebdfd-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/reports/getPolicyNonComplianceSummaryReport

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

### <a name="response"></a><span data-ttu-id="ebdfd-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="ebdfd-164">Response</span></span>
<span data-ttu-id="ebdfd-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ebdfd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "value": "Z2V0UG9saWN5Tm9uQ29tcGxpYW5jZVN1bW1hcnlSZXBvcnQgSW50dW5lIERvYyBTYW1wbGUgLTQzMjEwMjAyNg=="
}
```




