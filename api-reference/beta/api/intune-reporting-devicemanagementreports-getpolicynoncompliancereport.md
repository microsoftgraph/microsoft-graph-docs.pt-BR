---
title: ação getPolicyNonComplianceReport
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d97938d8aefda9b529ee76a0537c57a36d4fa84
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020024"
---
# <a name="getpolicynoncompliancereport-action"></a><span data-ttu-id="79f65-103">ação getPolicyNonComplianceReport</span><span class="sxs-lookup"><span data-stu-id="79f65-103">getPolicyNonComplianceReport action</span></span>

<span data-ttu-id="79f65-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79f65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79f65-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="79f65-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79f65-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79f65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79f65-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="79f65-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79f65-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="79f65-108">Prerequisites</span></span>
<span data-ttu-id="79f65-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="79f65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79f65-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="79f65-111">Permission type</span></span>|<span data-ttu-id="79f65-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="79f65-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79f65-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="79f65-113">Delegated (work or school account)</span></span>|<span data-ttu-id="79f65-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="79f65-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="79f65-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="79f65-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79f65-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="79f65-116">Not supported.</span></span>|
|<span data-ttu-id="79f65-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="79f65-117">Application</span></span>|<span data-ttu-id="79f65-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="79f65-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="79f65-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="79f65-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getPolicyNonComplianceReport
```

## <a name="request-headers"></a><span data-ttu-id="79f65-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="79f65-120">Request headers</span></span>
|<span data-ttu-id="79f65-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="79f65-121">Header</span></span>|<span data-ttu-id="79f65-122">Valor</span><span class="sxs-lookup"><span data-stu-id="79f65-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79f65-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="79f65-123">Authorization</span></span>|<span data-ttu-id="79f65-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="79f65-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79f65-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="79f65-125">Accept</span></span>|<span data-ttu-id="79f65-126">application/json</span><span class="sxs-lookup"><span data-stu-id="79f65-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79f65-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="79f65-127">Request body</span></span>
<span data-ttu-id="79f65-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="79f65-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="79f65-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="79f65-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="79f65-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79f65-130">Property</span></span>|<span data-ttu-id="79f65-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="79f65-131">Type</span></span>|<span data-ttu-id="79f65-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="79f65-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79f65-133">nome</span><span class="sxs-lookup"><span data-stu-id="79f65-133">name</span></span>|<span data-ttu-id="79f65-134">String</span><span class="sxs-lookup"><span data-stu-id="79f65-134">String</span></span>|<span data-ttu-id="79f65-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="79f65-135">Not yet documented</span></span>|
|<span data-ttu-id="79f65-136">select</span><span class="sxs-lookup"><span data-stu-id="79f65-136">select</span></span>|<span data-ttu-id="79f65-137">String collection</span><span class="sxs-lookup"><span data-stu-id="79f65-137">String collection</span></span>|<span data-ttu-id="79f65-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="79f65-138">Not yet documented</span></span>|
|<span data-ttu-id="79f65-139">search</span><span class="sxs-lookup"><span data-stu-id="79f65-139">search</span></span>|<span data-ttu-id="79f65-140">String</span><span class="sxs-lookup"><span data-stu-id="79f65-140">String</span></span>|<span data-ttu-id="79f65-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="79f65-141">Not yet documented</span></span>|
|<span data-ttu-id="79f65-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="79f65-142">groupBy</span></span>|<span data-ttu-id="79f65-143">String collection</span><span class="sxs-lookup"><span data-stu-id="79f65-143">String collection</span></span>|<span data-ttu-id="79f65-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="79f65-144">Not yet documented</span></span>|
|<span data-ttu-id="79f65-145">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="79f65-145">orderBy</span></span>|<span data-ttu-id="79f65-146">String collection</span><span class="sxs-lookup"><span data-stu-id="79f65-146">String collection</span></span>|<span data-ttu-id="79f65-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="79f65-147">Not yet documented</span></span>|
|<span data-ttu-id="79f65-148">skip</span><span class="sxs-lookup"><span data-stu-id="79f65-148">skip</span></span>|<span data-ttu-id="79f65-149">Int32</span><span class="sxs-lookup"><span data-stu-id="79f65-149">Int32</span></span>|<span data-ttu-id="79f65-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="79f65-150">Not yet documented</span></span>|
|<span data-ttu-id="79f65-151">top</span><span class="sxs-lookup"><span data-stu-id="79f65-151">top</span></span>|<span data-ttu-id="79f65-152">Int32</span><span class="sxs-lookup"><span data-stu-id="79f65-152">Int32</span></span>|<span data-ttu-id="79f65-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="79f65-153">Not yet documented</span></span>|
|<span data-ttu-id="79f65-154">Identificação_da_sessão</span><span class="sxs-lookup"><span data-stu-id="79f65-154">sessionId</span></span>|<span data-ttu-id="79f65-155">String</span><span class="sxs-lookup"><span data-stu-id="79f65-155">String</span></span>|<span data-ttu-id="79f65-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="79f65-156">Not yet documented</span></span>|
|<span data-ttu-id="79f65-157">filter</span><span class="sxs-lookup"><span data-stu-id="79f65-157">filter</span></span>|<span data-ttu-id="79f65-158">String</span><span class="sxs-lookup"><span data-stu-id="79f65-158">String</span></span>|<span data-ttu-id="79f65-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="79f65-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="79f65-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="79f65-160">Response</span></span>
<span data-ttu-id="79f65-161">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e um fluxo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="79f65-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79f65-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="79f65-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="79f65-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="79f65-163">Request</span></span>
<span data-ttu-id="79f65-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="79f65-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getPolicyNonComplianceReport

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

### <a name="response"></a><span data-ttu-id="79f65-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="79f65-165">Response</span></span>
<span data-ttu-id="79f65-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="79f65-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "value": "Z2V0UG9saWN5Tm9uQ29tcGxpYW5jZVJlcG9ydCBJbnR1bmUgRG9jIFNhbXBsZSAtNjU2NTI5OTUw"
}
```






