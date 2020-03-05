---
title: ação getDeviceNonComplianceReport
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eb91658d5dc924d2be0e1bf4543957f49de68103
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42459161"
---
# <a name="getdevicenoncompliancereport-action"></a><span data-ttu-id="12a40-103">ação getDeviceNonComplianceReport</span><span class="sxs-lookup"><span data-stu-id="12a40-103">getDeviceNonComplianceReport action</span></span>

<span data-ttu-id="12a40-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="12a40-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="12a40-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="12a40-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="12a40-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="12a40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12a40-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="12a40-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="12a40-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="12a40-108">Prerequisites</span></span>
<span data-ttu-id="12a40-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="12a40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="12a40-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="12a40-111">Permission type</span></span>|<span data-ttu-id="12a40-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="12a40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="12a40-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="12a40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="12a40-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="12a40-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="12a40-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="12a40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="12a40-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="12a40-116">Not supported.</span></span>|
|<span data-ttu-id="12a40-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="12a40-117">Application</span></span>|<span data-ttu-id="12a40-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="12a40-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="12a40-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="12a40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getDeviceNonComplianceReport
```

## <a name="request-headers"></a><span data-ttu-id="12a40-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="12a40-120">Request headers</span></span>
|<span data-ttu-id="12a40-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="12a40-121">Header</span></span>|<span data-ttu-id="12a40-122">Valor</span><span class="sxs-lookup"><span data-stu-id="12a40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="12a40-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="12a40-123">Authorization</span></span>|<span data-ttu-id="12a40-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="12a40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="12a40-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="12a40-125">Accept</span></span>|<span data-ttu-id="12a40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="12a40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="12a40-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="12a40-127">Request body</span></span>
<span data-ttu-id="12a40-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="12a40-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="12a40-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="12a40-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="12a40-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="12a40-130">Property</span></span>|<span data-ttu-id="12a40-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="12a40-131">Type</span></span>|<span data-ttu-id="12a40-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="12a40-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12a40-133">nome</span><span class="sxs-lookup"><span data-stu-id="12a40-133">name</span></span>|<span data-ttu-id="12a40-134">String</span><span class="sxs-lookup"><span data-stu-id="12a40-134">String</span></span>|<span data-ttu-id="12a40-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="12a40-135">Not yet documented</span></span>|
|<span data-ttu-id="12a40-136">select</span><span class="sxs-lookup"><span data-stu-id="12a40-136">select</span></span>|<span data-ttu-id="12a40-137">String collection</span><span class="sxs-lookup"><span data-stu-id="12a40-137">String collection</span></span>|<span data-ttu-id="12a40-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="12a40-138">Not yet documented</span></span>|
|<span data-ttu-id="12a40-139">search</span><span class="sxs-lookup"><span data-stu-id="12a40-139">search</span></span>|<span data-ttu-id="12a40-140">String</span><span class="sxs-lookup"><span data-stu-id="12a40-140">String</span></span>|<span data-ttu-id="12a40-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="12a40-141">Not yet documented</span></span>|
|<span data-ttu-id="12a40-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="12a40-142">groupBy</span></span>|<span data-ttu-id="12a40-143">String collection</span><span class="sxs-lookup"><span data-stu-id="12a40-143">String collection</span></span>|<span data-ttu-id="12a40-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="12a40-144">Not yet documented</span></span>|
|<span data-ttu-id="12a40-145">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="12a40-145">orderBy</span></span>|<span data-ttu-id="12a40-146">String collection</span><span class="sxs-lookup"><span data-stu-id="12a40-146">String collection</span></span>|<span data-ttu-id="12a40-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="12a40-147">Not yet documented</span></span>|
|<span data-ttu-id="12a40-148">skip</span><span class="sxs-lookup"><span data-stu-id="12a40-148">skip</span></span>|<span data-ttu-id="12a40-149">Int32</span><span class="sxs-lookup"><span data-stu-id="12a40-149">Int32</span></span>|<span data-ttu-id="12a40-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="12a40-150">Not yet documented</span></span>|
|<span data-ttu-id="12a40-151">top</span><span class="sxs-lookup"><span data-stu-id="12a40-151">top</span></span>|<span data-ttu-id="12a40-152">Int32</span><span class="sxs-lookup"><span data-stu-id="12a40-152">Int32</span></span>|<span data-ttu-id="12a40-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="12a40-153">Not yet documented</span></span>|
|<span data-ttu-id="12a40-154">Identificação_da_sessão</span><span class="sxs-lookup"><span data-stu-id="12a40-154">sessionId</span></span>|<span data-ttu-id="12a40-155">String</span><span class="sxs-lookup"><span data-stu-id="12a40-155">String</span></span>|<span data-ttu-id="12a40-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="12a40-156">Not yet documented</span></span>|
|<span data-ttu-id="12a40-157">filter</span><span class="sxs-lookup"><span data-stu-id="12a40-157">filter</span></span>|<span data-ttu-id="12a40-158">String</span><span class="sxs-lookup"><span data-stu-id="12a40-158">String</span></span>|<span data-ttu-id="12a40-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="12a40-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="12a40-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="12a40-160">Response</span></span>
<span data-ttu-id="12a40-161">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e um fluxo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="12a40-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="12a40-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="12a40-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="12a40-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="12a40-163">Request</span></span>
<span data-ttu-id="12a40-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="12a40-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getDeviceNonComplianceReport

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

### <a name="response"></a><span data-ttu-id="12a40-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="12a40-165">Response</span></span>
<span data-ttu-id="12a40-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="12a40-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 54

{
  "value": "<Unknown Primitive Type Edm.Stream>"
}
```





