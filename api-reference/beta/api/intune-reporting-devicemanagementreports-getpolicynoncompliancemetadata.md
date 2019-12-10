---
title: ação getPolicyNonComplianceMetadata
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 70427a9d4601330f1c00ab7fe6371af5bd37a05b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39940282"
---
# <a name="getpolicynoncompliancemetadata-action"></a><span data-ttu-id="22256-103">ação getPolicyNonComplianceMetadata</span><span class="sxs-lookup"><span data-stu-id="22256-103">getPolicyNonComplianceMetadata action</span></span>

> <span data-ttu-id="22256-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="22256-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22256-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="22256-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22256-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="22256-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22256-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="22256-107">Prerequisites</span></span>
<span data-ttu-id="22256-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="22256-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22256-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="22256-110">Permission type</span></span>|<span data-ttu-id="22256-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="22256-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22256-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="22256-112">Delegated (work or school account)</span></span>|<span data-ttu-id="22256-113">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="22256-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="22256-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="22256-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22256-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="22256-115">Not supported.</span></span>|
|<span data-ttu-id="22256-116">Application</span><span class="sxs-lookup"><span data-stu-id="22256-116">Application</span></span>|<span data-ttu-id="22256-117">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="22256-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="22256-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="22256-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getPolicyNonComplianceMetadata
```

## <a name="request-headers"></a><span data-ttu-id="22256-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="22256-119">Request headers</span></span>
|<span data-ttu-id="22256-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="22256-120">Header</span></span>|<span data-ttu-id="22256-121">Valor</span><span class="sxs-lookup"><span data-stu-id="22256-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22256-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="22256-122">Authorization</span></span>|<span data-ttu-id="22256-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="22256-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22256-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="22256-124">Accept</span></span>|<span data-ttu-id="22256-125">application/json</span><span class="sxs-lookup"><span data-stu-id="22256-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22256-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="22256-126">Request body</span></span>
<span data-ttu-id="22256-127">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="22256-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="22256-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="22256-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="22256-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22256-129">Property</span></span>|<span data-ttu-id="22256-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="22256-130">Type</span></span>|<span data-ttu-id="22256-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="22256-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22256-132">name</span><span class="sxs-lookup"><span data-stu-id="22256-132">name</span></span>|<span data-ttu-id="22256-133">String</span><span class="sxs-lookup"><span data-stu-id="22256-133">String</span></span>|<span data-ttu-id="22256-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="22256-134">Not yet documented</span></span>|
|<span data-ttu-id="22256-135">select</span><span class="sxs-lookup"><span data-stu-id="22256-135">select</span></span>|<span data-ttu-id="22256-136">String collection</span><span class="sxs-lookup"><span data-stu-id="22256-136">String collection</span></span>|<span data-ttu-id="22256-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="22256-137">Not yet documented</span></span>|
|<span data-ttu-id="22256-138">search</span><span class="sxs-lookup"><span data-stu-id="22256-138">search</span></span>|<span data-ttu-id="22256-139">String</span><span class="sxs-lookup"><span data-stu-id="22256-139">String</span></span>|<span data-ttu-id="22256-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="22256-140">Not yet documented</span></span>|
|<span data-ttu-id="22256-141">groupBy</span><span class="sxs-lookup"><span data-stu-id="22256-141">groupBy</span></span>|<span data-ttu-id="22256-142">String collection</span><span class="sxs-lookup"><span data-stu-id="22256-142">String collection</span></span>|<span data-ttu-id="22256-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="22256-143">Not yet documented</span></span>|
|<span data-ttu-id="22256-144">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="22256-144">orderBy</span></span>|<span data-ttu-id="22256-145">String collection</span><span class="sxs-lookup"><span data-stu-id="22256-145">String collection</span></span>|<span data-ttu-id="22256-146">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="22256-146">Not yet documented</span></span>|
|<span data-ttu-id="22256-147">skip</span><span class="sxs-lookup"><span data-stu-id="22256-147">skip</span></span>|<span data-ttu-id="22256-148">Int32</span><span class="sxs-lookup"><span data-stu-id="22256-148">Int32</span></span>|<span data-ttu-id="22256-149">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="22256-149">Not yet documented</span></span>|
|<span data-ttu-id="22256-150">top</span><span class="sxs-lookup"><span data-stu-id="22256-150">top</span></span>|<span data-ttu-id="22256-151">Int32</span><span class="sxs-lookup"><span data-stu-id="22256-151">Int32</span></span>|<span data-ttu-id="22256-152">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="22256-152">Not yet documented</span></span>|
|<span data-ttu-id="22256-153">Identificação_da_sessão</span><span class="sxs-lookup"><span data-stu-id="22256-153">sessionId</span></span>|<span data-ttu-id="22256-154">String</span><span class="sxs-lookup"><span data-stu-id="22256-154">String</span></span>|<span data-ttu-id="22256-155">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="22256-155">Not yet documented</span></span>|
|<span data-ttu-id="22256-156">filter</span><span class="sxs-lookup"><span data-stu-id="22256-156">filter</span></span>|<span data-ttu-id="22256-157">String</span><span class="sxs-lookup"><span data-stu-id="22256-157">String</span></span>|<span data-ttu-id="22256-158">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="22256-158">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="22256-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="22256-159">Response</span></span>
<span data-ttu-id="22256-160">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e um fluxo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="22256-160">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22256-161">Exemplo</span><span class="sxs-lookup"><span data-stu-id="22256-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="22256-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="22256-162">Request</span></span>
<span data-ttu-id="22256-163">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="22256-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getPolicyNonComplianceMetadata

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

### <a name="response"></a><span data-ttu-id="22256-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="22256-164">Response</span></span>
<span data-ttu-id="22256-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="22256-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 54

{
  "value": "<Unknown Primitive Type Edm.Stream>"
}
```





