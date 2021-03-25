---
title: Ação getSettingNonComplianceReport
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d5e9ce6697677328bf168049546e35e585cb1a21
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156398"
---
# <a name="getsettingnoncompliancereport-action"></a><span data-ttu-id="92bb9-103">Ação getSettingNonComplianceReport</span><span class="sxs-lookup"><span data-stu-id="92bb9-103">getSettingNonComplianceReport action</span></span>

<span data-ttu-id="92bb9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92bb9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92bb9-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92bb9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92bb9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92bb9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92bb9-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="92bb9-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92bb9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92bb9-108">Prerequisites</span></span>
<span data-ttu-id="92bb9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92bb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92bb9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92bb9-111">Permission type</span></span>|<span data-ttu-id="92bb9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="92bb9-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92bb9-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92bb9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92bb9-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92bb9-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="92bb9-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92bb9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92bb9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92bb9-116">Not supported.</span></span>|
|<span data-ttu-id="92bb9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92bb9-117">Application</span></span>|<span data-ttu-id="92bb9-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="92bb9-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92bb9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92bb9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/reports/getSettingNonComplianceReport
```

## <a name="request-headers"></a><span data-ttu-id="92bb9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92bb9-120">Request headers</span></span>
|<span data-ttu-id="92bb9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92bb9-121">Header</span></span>|<span data-ttu-id="92bb9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="92bb9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92bb9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="92bb9-123">Authorization</span></span>|<span data-ttu-id="92bb9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92bb9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92bb9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92bb9-125">Accept</span></span>|<span data-ttu-id="92bb9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92bb9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92bb9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92bb9-127">Request body</span></span>
<span data-ttu-id="92bb9-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="92bb9-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="92bb9-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="92bb9-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="92bb9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92bb9-130">Property</span></span>|<span data-ttu-id="92bb9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="92bb9-131">Type</span></span>|<span data-ttu-id="92bb9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="92bb9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92bb9-133">nome</span><span class="sxs-lookup"><span data-stu-id="92bb9-133">name</span></span>|<span data-ttu-id="92bb9-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="92bb9-134">String</span></span>|<span data-ttu-id="92bb9-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="92bb9-135">Not yet documented</span></span>|
|<span data-ttu-id="92bb9-136">select</span><span class="sxs-lookup"><span data-stu-id="92bb9-136">select</span></span>|<span data-ttu-id="92bb9-137">String collection</span><span class="sxs-lookup"><span data-stu-id="92bb9-137">String collection</span></span>|<span data-ttu-id="92bb9-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="92bb9-138">Not yet documented</span></span>|
|<span data-ttu-id="92bb9-139">search</span><span class="sxs-lookup"><span data-stu-id="92bb9-139">search</span></span>|<span data-ttu-id="92bb9-140">String</span><span class="sxs-lookup"><span data-stu-id="92bb9-140">String</span></span>|<span data-ttu-id="92bb9-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="92bb9-141">Not yet documented</span></span>|
|<span data-ttu-id="92bb9-142">groupBy</span><span class="sxs-lookup"><span data-stu-id="92bb9-142">groupBy</span></span>|<span data-ttu-id="92bb9-143">String collection</span><span class="sxs-lookup"><span data-stu-id="92bb9-143">String collection</span></span>|<span data-ttu-id="92bb9-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="92bb9-144">Not yet documented</span></span>|
|<span data-ttu-id="92bb9-145">orderBy</span><span class="sxs-lookup"><span data-stu-id="92bb9-145">orderBy</span></span>|<span data-ttu-id="92bb9-146">String collection</span><span class="sxs-lookup"><span data-stu-id="92bb9-146">String collection</span></span>|<span data-ttu-id="92bb9-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="92bb9-147">Not yet documented</span></span>|
|<span data-ttu-id="92bb9-148">skip</span><span class="sxs-lookup"><span data-stu-id="92bb9-148">skip</span></span>|<span data-ttu-id="92bb9-149">Int32</span><span class="sxs-lookup"><span data-stu-id="92bb9-149">Int32</span></span>|<span data-ttu-id="92bb9-150">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="92bb9-150">Not yet documented</span></span>|
|<span data-ttu-id="92bb9-151">top</span><span class="sxs-lookup"><span data-stu-id="92bb9-151">top</span></span>|<span data-ttu-id="92bb9-152">Int32</span><span class="sxs-lookup"><span data-stu-id="92bb9-152">Int32</span></span>|<span data-ttu-id="92bb9-153">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="92bb9-153">Not yet documented</span></span>|
|<span data-ttu-id="92bb9-154">sessionId</span><span class="sxs-lookup"><span data-stu-id="92bb9-154">sessionId</span></span>|<span data-ttu-id="92bb9-155">String</span><span class="sxs-lookup"><span data-stu-id="92bb9-155">String</span></span>|<span data-ttu-id="92bb9-156">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="92bb9-156">Not yet documented</span></span>|
|<span data-ttu-id="92bb9-157">filter</span><span class="sxs-lookup"><span data-stu-id="92bb9-157">filter</span></span>|<span data-ttu-id="92bb9-158">String</span><span class="sxs-lookup"><span data-stu-id="92bb9-158">String</span></span>|<span data-ttu-id="92bb9-159">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="92bb9-159">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="92bb9-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="92bb9-160">Response</span></span>
<span data-ttu-id="92bb9-161">Se tiver êxito, essa ação retornará `200 OK` um código de resposta e um Stream no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92bb9-161">If successful, this action returns a `200 OK` response code and a Stream in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92bb9-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92bb9-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="92bb9-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92bb9-163">Request</span></span>
<span data-ttu-id="92bb9-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92bb9-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="92bb9-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="92bb9-165">Response</span></span>
<span data-ttu-id="92bb9-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92bb9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 99

{
  "value": "Z2V0U2V0dGluZ05vbkNvbXBsaWFuY2VSZXBvcnQgSW50dW5lIERvYyBTYW1wbGUgMTEwMDk1MTE2MA=="
}
```




