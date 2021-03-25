---
title: ação getCompliancePolicyNonComplianceReport
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 94c47247034342d91f98e3ec6c6d141d34af4bfd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156566"
---
# <a name="getcompliancepolicynoncompliancereport-action"></a><span data-ttu-id="44d53-103">ação getCompliancePolicyNonComplianceReport</span><span class="sxs-lookup"><span data-stu-id="44d53-103">getCompliancePolicyNonComplianceReport action</span></span>

<span data-ttu-id="44d53-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="44d53-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44d53-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="44d53-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44d53-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="44d53-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44d53-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="44d53-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="44d53-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="44d53-108">Prerequisites</span></span>
<span data-ttu-id="44d53-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="44d53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="44d53-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44d53-111">Permission type</span></span>|<span data-ttu-id="44d53-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="44d53-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="44d53-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44d53-113">Delegated (work or school account)</span></span>|<span data-ttu-id="44d53-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44d53-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="44d53-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44d53-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="44d53-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44d53-116">Not supported.</span></span>|
|<span data-ttu-id="44d53-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44d53-117">Application</span></span>|<span data-ttu-id="44d53-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="44d53-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="44d53-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44d53-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getCompliancePolicyNonComplianceReport
```

## <a name="request-headers"></a><span data-ttu-id="44d53-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44d53-120">Request headers</span></span>
|<span data-ttu-id="44d53-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="44d53-121">Header</span></span>|<span data-ttu-id="44d53-122">Valor</span><span class="sxs-lookup"><span data-stu-id="44d53-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="44d53-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="44d53-123">Authorization</span></span>|<span data-ttu-id="44d53-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44d53-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="44d53-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="44d53-125">Accept</span></span>|<span data-ttu-id="44d53-126">application/json</span><span class="sxs-lookup"><span data-stu-id="44d53-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="44d53-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44d53-127">Request body</span></span>
<span data-ttu-id="44d53-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="44d53-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="44d53-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="44d53-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="44d53-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="44d53-130">Property</span></span>|<span data-ttu-id="44d53-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="44d53-131">Type</span></span>|<span data-ttu-id="44d53-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="44d53-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44d53-133">nome</span><span class="sxs-lookup"><span data-stu-id="44d53-133">name</span></span>|<span data-ttu-id="44d53-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="44d53-134">String</span></span>|<span data-ttu-id="44d53-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="44d53-135">Not yet documented</span></span>|
|<span data-ttu-id="44d53-136">select</span><span class="sxs-lookup"><span data-stu-id="44d53-136">select</span></span>|<span data-ttu-id="44d53-137">String collection</span><span class="sxs-lookup"><span data-stu-id="44d53-137">String collection</span></span>|<span data-ttu-id="44d53-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="44d53-138">Not yet documented</span></span>|
|<span data-ttu-id="44d53-139">search</span><span class="sxs-lookup"><span data-stu-id="44d53-139">search</span></span>|<span data-ttu-id="44d53-140">String</span><span class="sxs-lookup"><span data-stu-id="44d53-140">String</span></span>|<span data-ttu-id="44d53-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="44d53-141">Not yet documented</span></span>|
|<span data-ttu-id="44d53-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="44d53-142">groupBy</span></span>|<span data-ttu-id="44d53-143">String collection</span><span class="sxs-lookup"><span data-stu-id="44d53-143">String collection</span></span>|<span data-ttu-id="44d53-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="44d53-144">Not yet documented</span></span>|
|<span data-ttu-id="44d53-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="44d53-145">orderBy</span></span>|<span data-ttu-id="44d53-146">String collection</span><span class="sxs-lookup"><span data-stu-id="44d53-146">String collection</span></span>|<span data-ttu-id="44d53-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="44d53-147">Not yet documented</span></span>|
|<span data-ttu-id="44d53-148">skip</span><span class="sxs-lookup"><span data-stu-id="44d53-148">skip</span></span>|<span data-ttu-id="44d53-149">Int32</span><span class="sxs-lookup"><span data-stu-id="44d53-149">Int32</span></span>|<span data-ttu-id="44d53-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="44d53-150">Not yet documented</span></span>|
|<span data-ttu-id="44d53-151">top</span><span class="sxs-lookup"><span data-stu-id="44d53-151">top</span></span>|<span data-ttu-id="44d53-152">Int32</span><span class="sxs-lookup"><span data-stu-id="44d53-152">Int32</span></span>|<span data-ttu-id="44d53-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="44d53-153">Not yet documented</span></span>|
|<span data-ttu-id="44d53-154">sessionId</span><span class="sxs-lookup"><span data-stu-id="44d53-154">sessionId</span></span>|<span data-ttu-id="44d53-155">String</span><span class="sxs-lookup"><span data-stu-id="44d53-155">String</span></span>|<span data-ttu-id="44d53-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="44d53-156">Not yet documented</span></span>|
|<span data-ttu-id="44d53-157">filter</span><span class="sxs-lookup"><span data-stu-id="44d53-157">filter</span></span>|<span data-ttu-id="44d53-158">String</span><span class="sxs-lookup"><span data-stu-id="44d53-158">String</span></span>|<span data-ttu-id="44d53-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="44d53-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="44d53-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="44d53-160">Response</span></span>
<span data-ttu-id="44d53-161">Se tiver êxito, essa ação retornará `200 OK` um código de resposta e um Stream no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44d53-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44d53-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44d53-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="44d53-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44d53-163">Request</span></span>
<span data-ttu-id="44d53-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44d53-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getCompliancePolicyNonComplianceReport

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

### <a name="response"></a><span data-ttu-id="44d53-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="44d53-165">Response</span></span>
<span data-ttu-id="44d53-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="44d53-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 111

{
  "value": "Z2V0Q29tcGxpYW5jZVBvbGljeU5vbkNvbXBsaWFuY2VSZXBvcnQgSW50dW5lIERvYyBTYW1wbGUgMTA0ODU4MDU5OQ=="
}
```




