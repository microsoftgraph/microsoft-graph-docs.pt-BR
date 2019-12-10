---
title: ação getDeviceNonComplianceReport
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 69d9aac21c491736429b8a8bae1ede36381f891d
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940296"
---
# <a name="getdevicenoncompliancereport-action"></a><span data-ttu-id="86905-103">ação getDeviceNonComplianceReport</span><span class="sxs-lookup"><span data-stu-id="86905-103">getDeviceNonComplianceReport action</span></span>

> <span data-ttu-id="86905-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="86905-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86905-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86905-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86905-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="86905-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86905-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86905-107">Prerequisites</span></span>
<span data-ttu-id="86905-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86905-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86905-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86905-110">Permission type</span></span>|<span data-ttu-id="86905-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="86905-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86905-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86905-112">Delegated (work or school account)</span></span>|<span data-ttu-id="86905-113">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="86905-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="86905-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86905-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86905-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86905-115">Not supported.</span></span>|
|<span data-ttu-id="86905-116">Application</span><span class="sxs-lookup"><span data-stu-id="86905-116">Application</span></span>|<span data-ttu-id="86905-117">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="86905-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86905-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86905-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getDeviceNonComplianceReport
```

## <a name="request-headers"></a><span data-ttu-id="86905-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86905-119">Request headers</span></span>
|<span data-ttu-id="86905-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86905-120">Header</span></span>|<span data-ttu-id="86905-121">Valor</span><span class="sxs-lookup"><span data-stu-id="86905-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86905-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="86905-122">Authorization</span></span>|<span data-ttu-id="86905-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86905-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86905-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="86905-124">Accept</span></span>|<span data-ttu-id="86905-125">application/json</span><span class="sxs-lookup"><span data-stu-id="86905-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86905-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86905-126">Request body</span></span>
<span data-ttu-id="86905-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="86905-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="86905-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="86905-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="86905-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86905-129">Property</span></span>|<span data-ttu-id="86905-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="86905-130">Type</span></span>|<span data-ttu-id="86905-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="86905-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86905-132">name</span><span class="sxs-lookup"><span data-stu-id="86905-132">name</span></span>|<span data-ttu-id="86905-133">String</span><span class="sxs-lookup"><span data-stu-id="86905-133">String</span></span>|<span data-ttu-id="86905-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="86905-134">Not yet documented</span></span>|
|<span data-ttu-id="86905-135">select</span><span class="sxs-lookup"><span data-stu-id="86905-135">select</span></span>|<span data-ttu-id="86905-136">String collection</span><span class="sxs-lookup"><span data-stu-id="86905-136">String collection</span></span>|<span data-ttu-id="86905-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="86905-137">Not yet documented</span></span>|
|<span data-ttu-id="86905-138">search</span><span class="sxs-lookup"><span data-stu-id="86905-138">search</span></span>|<span data-ttu-id="86905-139">String</span><span class="sxs-lookup"><span data-stu-id="86905-139">String</span></span>|<span data-ttu-id="86905-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="86905-140">Not yet documented</span></span>|
|<span data-ttu-id="86905-141">groupBy</span><span class="sxs-lookup"><span data-stu-id="86905-141">groupBy</span></span>|<span data-ttu-id="86905-142">String collection</span><span class="sxs-lookup"><span data-stu-id="86905-142">String collection</span></span>|<span data-ttu-id="86905-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="86905-143">Not yet documented</span></span>|
|<span data-ttu-id="86905-144">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="86905-144">orderBy</span></span>|<span data-ttu-id="86905-145">String collection</span><span class="sxs-lookup"><span data-stu-id="86905-145">String collection</span></span>|<span data-ttu-id="86905-146">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="86905-146">Not yet documented</span></span>|
|<span data-ttu-id="86905-147">skip</span><span class="sxs-lookup"><span data-stu-id="86905-147">skip</span></span>|<span data-ttu-id="86905-148">Int32</span><span class="sxs-lookup"><span data-stu-id="86905-148">Int32</span></span>|<span data-ttu-id="86905-149">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="86905-149">Not yet documented</span></span>|
|<span data-ttu-id="86905-150">top</span><span class="sxs-lookup"><span data-stu-id="86905-150">top</span></span>|<span data-ttu-id="86905-151">Int32</span><span class="sxs-lookup"><span data-stu-id="86905-151">Int32</span></span>|<span data-ttu-id="86905-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="86905-152">Not yet documented</span></span>|
|<span data-ttu-id="86905-153">Identificação_da_sessão</span><span class="sxs-lookup"><span data-stu-id="86905-153">sessionId</span></span>|<span data-ttu-id="86905-154">String</span><span class="sxs-lookup"><span data-stu-id="86905-154">String</span></span>|<span data-ttu-id="86905-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="86905-155">Not yet documented</span></span>|
|<span data-ttu-id="86905-156">filter</span><span class="sxs-lookup"><span data-stu-id="86905-156">filter</span></span>|<span data-ttu-id="86905-157">String</span><span class="sxs-lookup"><span data-stu-id="86905-157">String</span></span>|<span data-ttu-id="86905-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="86905-158">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="86905-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="86905-159">Response</span></span>
<span data-ttu-id="86905-160">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e um fluxo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86905-160">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86905-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86905-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="86905-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86905-162">Request</span></span>
<span data-ttu-id="86905-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86905-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="86905-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="86905-164">Response</span></span>
<span data-ttu-id="86905-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86905-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 54

{
  "value": "<Unknown Primitive Type Edm.Stream>"
}
```





