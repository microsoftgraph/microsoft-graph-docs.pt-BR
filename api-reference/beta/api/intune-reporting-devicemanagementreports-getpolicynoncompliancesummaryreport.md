---
title: ação getPolicyNonComplianceSummaryReport
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b449828f9a2e2e7ca3f7dd359504fe2e7a36053e
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178427"
---
# <a name="getpolicynoncompliancesummaryreport-action"></a><span data-ttu-id="23cc3-103">ação getPolicyNonComplianceSummaryReport</span><span class="sxs-lookup"><span data-stu-id="23cc3-103">getPolicyNonComplianceSummaryReport action</span></span>

<span data-ttu-id="23cc3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23cc3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23cc3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="23cc3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23cc3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23cc3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23cc3-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23cc3-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23cc3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="23cc3-108">Prerequisites</span></span>
<span data-ttu-id="23cc3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23cc3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23cc3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="23cc3-111">Permission type</span></span>|<span data-ttu-id="23cc3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="23cc3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23cc3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="23cc3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23cc3-114">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="23cc3-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="23cc3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="23cc3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23cc3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="23cc3-116">Not supported.</span></span>|
|<span data-ttu-id="23cc3-117">Application</span><span class="sxs-lookup"><span data-stu-id="23cc3-117">Application</span></span>|<span data-ttu-id="23cc3-118">DeviceManagementConfiguration. ReadWrite. All, DeviceManagementConfiguration. Read. All, DeviceManagementApps. ReadWrite. All, DeviceManagementApps. Read. All, DeviceManagementManagedDevices. ReadWrite. All, DeviceManagementManagedDevices. Read. All</span><span class="sxs-lookup"><span data-stu-id="23cc3-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="23cc3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="23cc3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getPolicyNonComplianceSummaryReport
```

## <a name="request-headers"></a><span data-ttu-id="23cc3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="23cc3-120">Request headers</span></span>
|<span data-ttu-id="23cc3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="23cc3-121">Header</span></span>|<span data-ttu-id="23cc3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="23cc3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23cc3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="23cc3-123">Authorization</span></span>|<span data-ttu-id="23cc3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="23cc3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23cc3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="23cc3-125">Accept</span></span>|<span data-ttu-id="23cc3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23cc3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23cc3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="23cc3-127">Request body</span></span>
<span data-ttu-id="23cc3-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="23cc3-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="23cc3-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="23cc3-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="23cc3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23cc3-130">Property</span></span>|<span data-ttu-id="23cc3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="23cc3-131">Type</span></span>|<span data-ttu-id="23cc3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="23cc3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23cc3-133">name</span><span class="sxs-lookup"><span data-stu-id="23cc3-133">name</span></span>|<span data-ttu-id="23cc3-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23cc3-134">String</span></span>|<span data-ttu-id="23cc3-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23cc3-135">Not yet documented</span></span>|
|<span data-ttu-id="23cc3-136">select</span><span class="sxs-lookup"><span data-stu-id="23cc3-136">select</span></span>|<span data-ttu-id="23cc3-137">String collection</span><span class="sxs-lookup"><span data-stu-id="23cc3-137">String collection</span></span>|<span data-ttu-id="23cc3-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23cc3-138">Not yet documented</span></span>|
|<span data-ttu-id="23cc3-139">search</span><span class="sxs-lookup"><span data-stu-id="23cc3-139">search</span></span>|<span data-ttu-id="23cc3-140">String</span><span class="sxs-lookup"><span data-stu-id="23cc3-140">String</span></span>|<span data-ttu-id="23cc3-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23cc3-141">Not yet documented</span></span>|
|<span data-ttu-id="23cc3-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="23cc3-142">groupBy</span></span>|<span data-ttu-id="23cc3-143">String collection</span><span class="sxs-lookup"><span data-stu-id="23cc3-143">String collection</span></span>|<span data-ttu-id="23cc3-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23cc3-144">Not yet documented</span></span>|
|<span data-ttu-id="23cc3-145">Classificadoporativado</span><span class="sxs-lookup"><span data-stu-id="23cc3-145">orderBy</span></span>|<span data-ttu-id="23cc3-146">String collection</span><span class="sxs-lookup"><span data-stu-id="23cc3-146">String collection</span></span>|<span data-ttu-id="23cc3-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23cc3-147">Not yet documented</span></span>|
|<span data-ttu-id="23cc3-148">skip</span><span class="sxs-lookup"><span data-stu-id="23cc3-148">skip</span></span>|<span data-ttu-id="23cc3-149">Int32</span><span class="sxs-lookup"><span data-stu-id="23cc3-149">Int32</span></span>|<span data-ttu-id="23cc3-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23cc3-150">Not yet documented</span></span>|
|<span data-ttu-id="23cc3-151">top</span><span class="sxs-lookup"><span data-stu-id="23cc3-151">top</span></span>|<span data-ttu-id="23cc3-152">Int32</span><span class="sxs-lookup"><span data-stu-id="23cc3-152">Int32</span></span>|<span data-ttu-id="23cc3-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23cc3-153">Not yet documented</span></span>|
|<span data-ttu-id="23cc3-154">Identificação_da_sessão</span><span class="sxs-lookup"><span data-stu-id="23cc3-154">sessionId</span></span>|<span data-ttu-id="23cc3-155">String</span><span class="sxs-lookup"><span data-stu-id="23cc3-155">String</span></span>|<span data-ttu-id="23cc3-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23cc3-156">Not yet documented</span></span>|
|<span data-ttu-id="23cc3-157">filter</span><span class="sxs-lookup"><span data-stu-id="23cc3-157">filter</span></span>|<span data-ttu-id="23cc3-158">String</span><span class="sxs-lookup"><span data-stu-id="23cc3-158">String</span></span>|<span data-ttu-id="23cc3-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23cc3-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="23cc3-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="23cc3-160">Response</span></span>
<span data-ttu-id="23cc3-161">Se tiver êxito, esta ação retornará `200 OK` um código de resposta e um fluxo no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="23cc3-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23cc3-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="23cc3-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="23cc3-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="23cc3-163">Request</span></span>
<span data-ttu-id="23cc3-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="23cc3-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getPolicyNonComplianceSummaryReport

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

### <a name="response"></a><span data-ttu-id="23cc3-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="23cc3-165">Response</span></span>
<span data-ttu-id="23cc3-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="23cc3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "value": "Z2V0UG9saWN5Tm9uQ29tcGxpYW5jZVN1bW1hcnlSZXBvcnQgSW50dW5lIERvYyBTYW1wbGUgLTQzMjEwMjAyNg=="
}
```



