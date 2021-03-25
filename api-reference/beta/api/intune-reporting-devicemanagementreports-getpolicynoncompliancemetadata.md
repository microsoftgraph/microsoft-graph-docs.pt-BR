---
title: ação getPolicyNonComplianceMetadata
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0a4b97e410f7c0a303f290b5c970ce05dd32b2b5
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156468"
---
# <a name="getpolicynoncompliancemetadata-action"></a><span data-ttu-id="485a4-103">ação getPolicyNonComplianceMetadata</span><span class="sxs-lookup"><span data-stu-id="485a4-103">getPolicyNonComplianceMetadata action</span></span>

<span data-ttu-id="485a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="485a4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="485a4-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="485a4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="485a4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="485a4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="485a4-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="485a4-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="485a4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="485a4-108">Prerequisites</span></span>
<span data-ttu-id="485a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="485a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="485a4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="485a4-111">Permission type</span></span>|<span data-ttu-id="485a4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="485a4-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="485a4-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="485a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="485a4-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="485a4-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="485a4-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="485a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="485a4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="485a4-116">Not supported.</span></span>|
|<span data-ttu-id="485a4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="485a4-117">Application</span></span>|<span data-ttu-id="485a4-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="485a4-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="485a4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="485a4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getPolicyNonComplianceMetadata
```

## <a name="request-headers"></a><span data-ttu-id="485a4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="485a4-120">Request headers</span></span>
|<span data-ttu-id="485a4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="485a4-121">Header</span></span>|<span data-ttu-id="485a4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="485a4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="485a4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="485a4-123">Authorization</span></span>|<span data-ttu-id="485a4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="485a4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="485a4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="485a4-125">Accept</span></span>|<span data-ttu-id="485a4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="485a4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="485a4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="485a4-127">Request body</span></span>
<span data-ttu-id="485a4-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="485a4-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="485a4-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="485a4-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="485a4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="485a4-130">Property</span></span>|<span data-ttu-id="485a4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="485a4-131">Type</span></span>|<span data-ttu-id="485a4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="485a4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="485a4-133">nome</span><span class="sxs-lookup"><span data-stu-id="485a4-133">name</span></span>|<span data-ttu-id="485a4-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="485a4-134">String</span></span>|<span data-ttu-id="485a4-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="485a4-135">Not yet documented</span></span>|
|<span data-ttu-id="485a4-136">select</span><span class="sxs-lookup"><span data-stu-id="485a4-136">select</span></span>|<span data-ttu-id="485a4-137">String collection</span><span class="sxs-lookup"><span data-stu-id="485a4-137">String collection</span></span>|<span data-ttu-id="485a4-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="485a4-138">Not yet documented</span></span>|
|<span data-ttu-id="485a4-139">search</span><span class="sxs-lookup"><span data-stu-id="485a4-139">search</span></span>|<span data-ttu-id="485a4-140">String</span><span class="sxs-lookup"><span data-stu-id="485a4-140">String</span></span>|<span data-ttu-id="485a4-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="485a4-141">Not yet documented</span></span>|
|<span data-ttu-id="485a4-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="485a4-142">groupBy</span></span>|<span data-ttu-id="485a4-143">String collection</span><span class="sxs-lookup"><span data-stu-id="485a4-143">String collection</span></span>|<span data-ttu-id="485a4-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="485a4-144">Not yet documented</span></span>|
|<span data-ttu-id="485a4-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="485a4-145">orderBy</span></span>|<span data-ttu-id="485a4-146">String collection</span><span class="sxs-lookup"><span data-stu-id="485a4-146">String collection</span></span>|<span data-ttu-id="485a4-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="485a4-147">Not yet documented</span></span>|
|<span data-ttu-id="485a4-148">skip</span><span class="sxs-lookup"><span data-stu-id="485a4-148">skip</span></span>|<span data-ttu-id="485a4-149">Int32</span><span class="sxs-lookup"><span data-stu-id="485a4-149">Int32</span></span>|<span data-ttu-id="485a4-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="485a4-150">Not yet documented</span></span>|
|<span data-ttu-id="485a4-151">top</span><span class="sxs-lookup"><span data-stu-id="485a4-151">top</span></span>|<span data-ttu-id="485a4-152">Int32</span><span class="sxs-lookup"><span data-stu-id="485a4-152">Int32</span></span>|<span data-ttu-id="485a4-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="485a4-153">Not yet documented</span></span>|
|<span data-ttu-id="485a4-154">sessionId</span><span class="sxs-lookup"><span data-stu-id="485a4-154">sessionId</span></span>|<span data-ttu-id="485a4-155">String</span><span class="sxs-lookup"><span data-stu-id="485a4-155">String</span></span>|<span data-ttu-id="485a4-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="485a4-156">Not yet documented</span></span>|
|<span data-ttu-id="485a4-157">filter</span><span class="sxs-lookup"><span data-stu-id="485a4-157">filter</span></span>|<span data-ttu-id="485a4-158">String</span><span class="sxs-lookup"><span data-stu-id="485a4-158">String</span></span>|<span data-ttu-id="485a4-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="485a4-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="485a4-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="485a4-160">Response</span></span>
<span data-ttu-id="485a4-161">Se tiver êxito, essa ação retornará `200 OK` um código de resposta e um Stream no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="485a4-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="485a4-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="485a4-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="485a4-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="485a4-163">Request</span></span>
<span data-ttu-id="485a4-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="485a4-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="485a4-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="485a4-165">Response</span></span>
<span data-ttu-id="485a4-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="485a4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 99

{
  "value": "Z2V0UG9saWN5Tm9uQ29tcGxpYW5jZU1ldGFkYXRhIEludHVuZSBEb2MgU2FtcGxlIC0xNzM5NTg5Nzc5"
}
```




