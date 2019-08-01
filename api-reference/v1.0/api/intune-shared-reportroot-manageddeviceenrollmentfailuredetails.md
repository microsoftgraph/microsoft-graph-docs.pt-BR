---
title: função managedDeviceEnrollmentFailureDetails
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: da38aa1fb497bc5fb1225f2435ed2bd9c4e4b3c3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025845"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="e3c18-103">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="e3c18-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="e3c18-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e3c18-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3c18-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e3c18-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3c18-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e3c18-106">Prerequisites</span></span>
<span data-ttu-id="e3c18-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3c18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3c18-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3c18-109">Permission type</span></span>|<span data-ttu-id="e3c18-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e3c18-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3c18-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3c18-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e3c18-112">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="e3c18-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="e3c18-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3c18-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e3c18-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3c18-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3c18-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3c18-115">Not supported.</span></span>|
|<span data-ttu-id="e3c18-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3c18-116">Application</span></span>|<span data-ttu-id="e3c18-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3c18-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3c18-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3c18-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="e3c18-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3c18-119">Request headers</span></span>
|<span data-ttu-id="e3c18-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e3c18-120">Header</span></span>|<span data-ttu-id="e3c18-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e3c18-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3c18-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3c18-122">Authorization</span></span>|<span data-ttu-id="e3c18-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e3c18-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3c18-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e3c18-124">Accept</span></span>|<span data-ttu-id="e3c18-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e3c18-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3c18-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3c18-126">Request body</span></span>
<span data-ttu-id="e3c18-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="e3c18-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e3c18-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="e3c18-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e3c18-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3c18-129">Property</span></span>|<span data-ttu-id="e3c18-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3c18-130">Type</span></span>|<span data-ttu-id="e3c18-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3c18-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3c18-132">skip</span><span class="sxs-lookup"><span data-stu-id="e3c18-132">skip</span></span>|<span data-ttu-id="e3c18-133">Int32</span><span class="sxs-lookup"><span data-stu-id="e3c18-133">Int32</span></span>|<span data-ttu-id="e3c18-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e3c18-134">Not yet documented</span></span>|
|<span data-ttu-id="e3c18-135">top</span><span class="sxs-lookup"><span data-stu-id="e3c18-135">top</span></span>|<span data-ttu-id="e3c18-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e3c18-136">Int32</span></span>|<span data-ttu-id="e3c18-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e3c18-137">Not yet documented</span></span>|
|<span data-ttu-id="e3c18-138">filter</span><span class="sxs-lookup"><span data-stu-id="e3c18-138">filter</span></span>|<span data-ttu-id="e3c18-139">String</span><span class="sxs-lookup"><span data-stu-id="e3c18-139">String</span></span>|<span data-ttu-id="e3c18-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e3c18-140">Not yet documented</span></span>|
|<span data-ttu-id="e3c18-141">skipToken</span><span class="sxs-lookup"><span data-stu-id="e3c18-141">skipToken</span></span>|<span data-ttu-id="e3c18-142">String</span><span class="sxs-lookup"><span data-stu-id="e3c18-142">String</span></span>|<span data-ttu-id="e3c18-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e3c18-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e3c18-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3c18-144">Response</span></span>
<span data-ttu-id="e3c18-145">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3c18-145">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3c18-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3c18-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3c18-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3c18-147">Request</span></span>
<span data-ttu-id="e3c18-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3c18-148">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e3c18-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3c18-149">Response</span></span>
<span data-ttu-id="e3c18-150">O objeto de resposta mostrado aqui pode estar truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="e3c18-150">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e3c18-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3c18-151">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 123

{
  "value": {
    "@odata.type": "microsoft.graph.report",
    "content": "<Unknown Primitive Type Edm.Stream>"
  }
}
```




