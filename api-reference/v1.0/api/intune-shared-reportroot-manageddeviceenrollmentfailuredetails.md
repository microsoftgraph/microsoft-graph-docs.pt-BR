---
title: função managedDeviceEnrollmentFailureDetails
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fd16afe8aafaefe84f385d13a9a56e823b689130
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37361368"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="84ba5-103">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="84ba5-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="84ba5-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84ba5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84ba5-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="84ba5-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84ba5-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="84ba5-106">Prerequisites</span></span>
<span data-ttu-id="84ba5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84ba5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84ba5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="84ba5-109">Permission type</span></span>|<span data-ttu-id="84ba5-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="84ba5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84ba5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="84ba5-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="84ba5-112">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="84ba5-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="84ba5-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84ba5-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="84ba5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="84ba5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84ba5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84ba5-115">Not supported.</span></span>|
|<span data-ttu-id="84ba5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="84ba5-116">Application</span></span>|<span data-ttu-id="84ba5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="84ba5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84ba5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="84ba5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="84ba5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="84ba5-119">Request headers</span></span>
|<span data-ttu-id="84ba5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="84ba5-120">Header</span></span>|<span data-ttu-id="84ba5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="84ba5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84ba5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="84ba5-122">Authorization</span></span>|<span data-ttu-id="84ba5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="84ba5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84ba5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="84ba5-124">Accept</span></span>|<span data-ttu-id="84ba5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84ba5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84ba5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="84ba5-126">Request body</span></span>
<span data-ttu-id="84ba5-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="84ba5-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="84ba5-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="84ba5-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="84ba5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84ba5-129">Property</span></span>|<span data-ttu-id="84ba5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="84ba5-130">Type</span></span>|<span data-ttu-id="84ba5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="84ba5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84ba5-132">skip</span><span class="sxs-lookup"><span data-stu-id="84ba5-132">skip</span></span>|<span data-ttu-id="84ba5-133">Int32</span><span class="sxs-lookup"><span data-stu-id="84ba5-133">Int32</span></span>|<span data-ttu-id="84ba5-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="84ba5-134">Not yet documented</span></span>|
|<span data-ttu-id="84ba5-135">top</span><span class="sxs-lookup"><span data-stu-id="84ba5-135">top</span></span>|<span data-ttu-id="84ba5-136">Int32</span><span class="sxs-lookup"><span data-stu-id="84ba5-136">Int32</span></span>|<span data-ttu-id="84ba5-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="84ba5-137">Not yet documented</span></span>|
|<span data-ttu-id="84ba5-138">filter</span><span class="sxs-lookup"><span data-stu-id="84ba5-138">filter</span></span>|<span data-ttu-id="84ba5-139">String</span><span class="sxs-lookup"><span data-stu-id="84ba5-139">String</span></span>|<span data-ttu-id="84ba5-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="84ba5-140">Not yet documented</span></span>|
|<span data-ttu-id="84ba5-141">skipToken</span><span class="sxs-lookup"><span data-stu-id="84ba5-141">skipToken</span></span>|<span data-ttu-id="84ba5-142">String</span><span class="sxs-lookup"><span data-stu-id="84ba5-142">String</span></span>|<span data-ttu-id="84ba5-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="84ba5-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="84ba5-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="84ba5-144">Response</span></span>
<span data-ttu-id="84ba5-145">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="84ba5-145">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84ba5-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="84ba5-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="84ba5-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="84ba5-147">Request</span></span>
<span data-ttu-id="84ba5-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="84ba5-148">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="84ba5-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="84ba5-149">Response</span></span>
<span data-ttu-id="84ba5-150">O objeto de resposta mostrado aqui pode estar truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="84ba5-150">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="84ba5-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="84ba5-151">All of the properties will be returned from an actual call.</span></span>

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





