---
title: ação getConfigurationPolicyNonComplianceReport
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 860b824e2ec6e3b3535733496690a0fe775463cf
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156517"
---
# <a name="getconfigurationpolicynoncompliancereport-action"></a><span data-ttu-id="9130c-103">ação getConfigurationPolicyNonComplianceReport</span><span class="sxs-lookup"><span data-stu-id="9130c-103">getConfigurationPolicyNonComplianceReport action</span></span>

<span data-ttu-id="9130c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9130c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9130c-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9130c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9130c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9130c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9130c-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9130c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9130c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9130c-108">Prerequisites</span></span>
<span data-ttu-id="9130c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9130c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9130c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9130c-111">Permission type</span></span>|<span data-ttu-id="9130c-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9130c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9130c-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9130c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9130c-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9130c-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9130c-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9130c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9130c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9130c-116">Not supported.</span></span>|
|<span data-ttu-id="9130c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9130c-117">Application</span></span>|<span data-ttu-id="9130c-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9130c-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9130c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9130c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getConfigurationPolicyNonComplianceReport
```

## <a name="request-headers"></a><span data-ttu-id="9130c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9130c-120">Request headers</span></span>
|<span data-ttu-id="9130c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9130c-121">Header</span></span>|<span data-ttu-id="9130c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9130c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9130c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9130c-123">Authorization</span></span>|<span data-ttu-id="9130c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9130c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9130c-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9130c-125">Accept</span></span>|<span data-ttu-id="9130c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9130c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9130c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9130c-127">Request body</span></span>
<span data-ttu-id="9130c-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="9130c-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="9130c-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="9130c-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="9130c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9130c-130">Property</span></span>|<span data-ttu-id="9130c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="9130c-131">Type</span></span>|<span data-ttu-id="9130c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="9130c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9130c-133">nome</span><span class="sxs-lookup"><span data-stu-id="9130c-133">name</span></span>|<span data-ttu-id="9130c-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9130c-134">String</span></span>|<span data-ttu-id="9130c-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9130c-135">Not yet documented</span></span>|
|<span data-ttu-id="9130c-136">select</span><span class="sxs-lookup"><span data-stu-id="9130c-136">select</span></span>|<span data-ttu-id="9130c-137">String collection</span><span class="sxs-lookup"><span data-stu-id="9130c-137">String collection</span></span>|<span data-ttu-id="9130c-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9130c-138">Not yet documented</span></span>|
|<span data-ttu-id="9130c-139">search</span><span class="sxs-lookup"><span data-stu-id="9130c-139">search</span></span>|<span data-ttu-id="9130c-140">String</span><span class="sxs-lookup"><span data-stu-id="9130c-140">String</span></span>|<span data-ttu-id="9130c-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9130c-141">Not yet documented</span></span>|
|<span data-ttu-id="9130c-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="9130c-142">groupBy</span></span>|<span data-ttu-id="9130c-143">String collection</span><span class="sxs-lookup"><span data-stu-id="9130c-143">String collection</span></span>|<span data-ttu-id="9130c-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9130c-144">Not yet documented</span></span>|
|<span data-ttu-id="9130c-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="9130c-145">orderBy</span></span>|<span data-ttu-id="9130c-146">String collection</span><span class="sxs-lookup"><span data-stu-id="9130c-146">String collection</span></span>|<span data-ttu-id="9130c-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9130c-147">Not yet documented</span></span>|
|<span data-ttu-id="9130c-148">skip</span><span class="sxs-lookup"><span data-stu-id="9130c-148">skip</span></span>|<span data-ttu-id="9130c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="9130c-149">Int32</span></span>|<span data-ttu-id="9130c-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9130c-150">Not yet documented</span></span>|
|<span data-ttu-id="9130c-151">top</span><span class="sxs-lookup"><span data-stu-id="9130c-151">top</span></span>|<span data-ttu-id="9130c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9130c-152">Int32</span></span>|<span data-ttu-id="9130c-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9130c-153">Not yet documented</span></span>|
|<span data-ttu-id="9130c-154">sessionId</span><span class="sxs-lookup"><span data-stu-id="9130c-154">sessionId</span></span>|<span data-ttu-id="9130c-155">String</span><span class="sxs-lookup"><span data-stu-id="9130c-155">String</span></span>|<span data-ttu-id="9130c-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9130c-156">Not yet documented</span></span>|
|<span data-ttu-id="9130c-157">filter</span><span class="sxs-lookup"><span data-stu-id="9130c-157">filter</span></span>|<span data-ttu-id="9130c-158">String</span><span class="sxs-lookup"><span data-stu-id="9130c-158">String</span></span>|<span data-ttu-id="9130c-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9130c-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9130c-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="9130c-160">Response</span></span>
<span data-ttu-id="9130c-161">Se tiver êxito, essa ação retornará `200 OK` um código de resposta e um Stream no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9130c-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9130c-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9130c-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="9130c-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9130c-163">Request</span></span>
<span data-ttu-id="9130c-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9130c-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getConfigurationPolicyNonComplianceReport

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

### <a name="response"></a><span data-ttu-id="9130c-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="9130c-165">Response</span></span>
<span data-ttu-id="9130c-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9130c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 115

{
  "value": "Z2V0Q29uZmlndXJhdGlvblBvbGljeU5vbkNvbXBsaWFuY2VSZXBvcnQgSW50dW5lIERvYyBTYW1wbGUgLTE2MTk2MDUzMTI="
}
```




