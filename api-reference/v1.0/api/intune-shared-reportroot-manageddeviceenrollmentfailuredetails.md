---
title: função managedDeviceEnrollmentFailureDetails
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1539992ad475c2339a33aae809bc477d5da4e772
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089137"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="89aa9-103">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="89aa9-103">managedDeviceEnrollmentFailureDetails function</span></span>

<span data-ttu-id="89aa9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89aa9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89aa9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="89aa9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89aa9-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89aa9-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="89aa9-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="89aa9-107">Prerequisites</span></span>
<span data-ttu-id="89aa9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="89aa9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89aa9-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="89aa9-110">Permission type</span></span>|<span data-ttu-id="89aa9-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="89aa9-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="89aa9-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="89aa9-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="89aa9-113">&nbsp;&nbsp;Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="89aa9-113">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="89aa9-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89aa9-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="89aa9-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="89aa9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="89aa9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89aa9-116">Not supported.</span></span>|
|<span data-ttu-id="89aa9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="89aa9-117">Application</span></span>|<span data-ttu-id="89aa9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="89aa9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="89aa9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="89aa9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="89aa9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="89aa9-120">Request headers</span></span>
|<span data-ttu-id="89aa9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="89aa9-121">Header</span></span>|<span data-ttu-id="89aa9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="89aa9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="89aa9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="89aa9-123">Authorization</span></span>|<span data-ttu-id="89aa9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="89aa9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="89aa9-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="89aa9-125">Accept</span></span>|<span data-ttu-id="89aa9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="89aa9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="89aa9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="89aa9-127">Request body</span></span>
<span data-ttu-id="89aa9-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="89aa9-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="89aa9-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="89aa9-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="89aa9-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="89aa9-130">Property</span></span>|<span data-ttu-id="89aa9-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="89aa9-131">Type</span></span>|<span data-ttu-id="89aa9-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="89aa9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89aa9-133">skip</span><span class="sxs-lookup"><span data-stu-id="89aa9-133">skip</span></span>|<span data-ttu-id="89aa9-134">Int32</span><span class="sxs-lookup"><span data-stu-id="89aa9-134">Int32</span></span>|<span data-ttu-id="89aa9-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89aa9-135">Not yet documented</span></span>|
|<span data-ttu-id="89aa9-136">top</span><span class="sxs-lookup"><span data-stu-id="89aa9-136">top</span></span>|<span data-ttu-id="89aa9-137">Int32</span><span class="sxs-lookup"><span data-stu-id="89aa9-137">Int32</span></span>|<span data-ttu-id="89aa9-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89aa9-138">Not yet documented</span></span>|
|<span data-ttu-id="89aa9-139">filter</span><span class="sxs-lookup"><span data-stu-id="89aa9-139">filter</span></span>|<span data-ttu-id="89aa9-140">String</span><span class="sxs-lookup"><span data-stu-id="89aa9-140">String</span></span>|<span data-ttu-id="89aa9-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89aa9-141">Not yet documented</span></span>|
|<span data-ttu-id="89aa9-142">skipToken</span><span class="sxs-lookup"><span data-stu-id="89aa9-142">skipToken</span></span>|<span data-ttu-id="89aa9-143">String</span><span class="sxs-lookup"><span data-stu-id="89aa9-143">String</span></span>|<span data-ttu-id="89aa9-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="89aa9-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="89aa9-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="89aa9-145">Response</span></span>
<span data-ttu-id="89aa9-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="89aa9-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89aa9-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="89aa9-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="89aa9-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="89aa9-148">Request</span></span>
<span data-ttu-id="89aa9-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="89aa9-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="89aa9-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="89aa9-150">Response</span></span>
<span data-ttu-id="89aa9-151">O objeto de resposta mostrado aqui pode estar truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="89aa9-151">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="89aa9-152">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="89aa9-152">All of the properties will be returned from an actual call.</span></span>

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










