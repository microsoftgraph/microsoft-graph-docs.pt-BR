---
title: ação getSettingNonComplianceReport
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 13b0f4485cfc752895f17cdd7ed58e203367b1d1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040459"
---
# <a name="getsettingnoncompliancereport-action"></a><span data-ttu-id="3b230-103">ação getSettingNonComplianceReport</span><span class="sxs-lookup"><span data-stu-id="3b230-103">getSettingNonComplianceReport action</span></span>

<span data-ttu-id="3b230-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b230-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b230-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b230-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b230-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b230-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b230-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3b230-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b230-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b230-108">Prerequisites</span></span>
<span data-ttu-id="3b230-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3b230-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b230-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b230-111">Permission type</span></span>|<span data-ttu-id="3b230-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b230-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b230-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b230-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3b230-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="3b230-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="3b230-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b230-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b230-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b230-116">Not supported.</span></span>|
|<span data-ttu-id="3b230-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b230-117">Application</span></span>|<span data-ttu-id="3b230-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="3b230-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b230-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b230-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getSettingNonComplianceReport
```

## <a name="request-headers"></a><span data-ttu-id="3b230-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b230-120">Request headers</span></span>
|<span data-ttu-id="3b230-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b230-121">Header</span></span>|<span data-ttu-id="3b230-122">Valor</span><span class="sxs-lookup"><span data-stu-id="3b230-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b230-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b230-123">Authorization</span></span>|<span data-ttu-id="3b230-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b230-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b230-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b230-125">Accept</span></span>|<span data-ttu-id="3b230-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3b230-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b230-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b230-127">Request body</span></span>
<span data-ttu-id="3b230-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3b230-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3b230-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3b230-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3b230-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b230-130">Property</span></span>|<span data-ttu-id="3b230-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b230-131">Type</span></span>|<span data-ttu-id="3b230-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b230-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b230-133">nome</span><span class="sxs-lookup"><span data-stu-id="3b230-133">name</span></span>|<span data-ttu-id="3b230-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b230-134">String</span></span>|<span data-ttu-id="3b230-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3b230-135">Not yet documented</span></span>|
|<span data-ttu-id="3b230-136">select</span><span class="sxs-lookup"><span data-stu-id="3b230-136">select</span></span>|<span data-ttu-id="3b230-137">String collection</span><span class="sxs-lookup"><span data-stu-id="3b230-137">String collection</span></span>|<span data-ttu-id="3b230-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3b230-138">Not yet documented</span></span>|
|<span data-ttu-id="3b230-139">search</span><span class="sxs-lookup"><span data-stu-id="3b230-139">search</span></span>|<span data-ttu-id="3b230-140">String</span><span class="sxs-lookup"><span data-stu-id="3b230-140">String</span></span>|<span data-ttu-id="3b230-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3b230-141">Not yet documented</span></span>|
|<span data-ttu-id="3b230-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="3b230-142">groupBy</span></span>|<span data-ttu-id="3b230-143">String collection</span><span class="sxs-lookup"><span data-stu-id="3b230-143">String collection</span></span>|<span data-ttu-id="3b230-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3b230-144">Not yet documented</span></span>|
|<span data-ttu-id="3b230-145">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="3b230-145">orderBy</span></span>|<span data-ttu-id="3b230-146">String collection</span><span class="sxs-lookup"><span data-stu-id="3b230-146">String collection</span></span>|<span data-ttu-id="3b230-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3b230-147">Not yet documented</span></span>|
|<span data-ttu-id="3b230-148">skip</span><span class="sxs-lookup"><span data-stu-id="3b230-148">skip</span></span>|<span data-ttu-id="3b230-149">Int32</span><span class="sxs-lookup"><span data-stu-id="3b230-149">Int32</span></span>|<span data-ttu-id="3b230-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3b230-150">Not yet documented</span></span>|
|<span data-ttu-id="3b230-151">top</span><span class="sxs-lookup"><span data-stu-id="3b230-151">top</span></span>|<span data-ttu-id="3b230-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3b230-152">Int32</span></span>|<span data-ttu-id="3b230-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3b230-153">Not yet documented</span></span>|
|<span data-ttu-id="3b230-154">Identificação_da_sessão</span><span class="sxs-lookup"><span data-stu-id="3b230-154">sessionId</span></span>|<span data-ttu-id="3b230-155">String</span><span class="sxs-lookup"><span data-stu-id="3b230-155">String</span></span>|<span data-ttu-id="3b230-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3b230-156">Not yet documented</span></span>|
|<span data-ttu-id="3b230-157">filter</span><span class="sxs-lookup"><span data-stu-id="3b230-157">filter</span></span>|<span data-ttu-id="3b230-158">String</span><span class="sxs-lookup"><span data-stu-id="3b230-158">String</span></span>|<span data-ttu-id="3b230-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3b230-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="3b230-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b230-160">Response</span></span>
<span data-ttu-id="3b230-161">Se tiver êxito, esta ação retornará um `200 OK` código de resposta e um fluxo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b230-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b230-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b230-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b230-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b230-163">Request</span></span>
<span data-ttu-id="3b230-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b230-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getSettingNonComplianceReport

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

### <a name="response"></a><span data-ttu-id="3b230-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b230-165">Response</span></span>
<span data-ttu-id="3b230-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b230-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 99

{
  "value": "Z2V0U2V0dGluZ05vbkNvbXBsaWFuY2VSZXBvcnQgSW50dW5lIERvYyBTYW1wbGUgMTEwMDk1MTE2MA=="
}
```






