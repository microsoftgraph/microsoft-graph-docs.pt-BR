---
title: função managedDeviceEnrollmentFailureDetails
description: Ainda não documentado
ms.openlocfilehash: c5e68453cb1655e4018156ac207b60e4145e571a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006478"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="98c66-103">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="98c66-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="98c66-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="98c66-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="98c66-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="98c66-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="98c66-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="98c66-106">Prerequisites</span></span>
<span data-ttu-id="98c66-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98c66-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98c66-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98c66-109">Permission type</span></span>|<span data-ttu-id="98c66-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="98c66-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98c66-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98c66-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="98c66-112">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="98c66-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="98c66-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98c66-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="98c66-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98c66-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98c66-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98c66-115">Not supported.</span></span>|
|<span data-ttu-id="98c66-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98c66-116">Application</span></span>|<span data-ttu-id="98c66-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98c66-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="98c66-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98c66-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="98c66-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98c66-119">Request headers</span></span>
|<span data-ttu-id="98c66-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98c66-120">Header</span></span>|<span data-ttu-id="98c66-121">Valor</span><span class="sxs-lookup"><span data-stu-id="98c66-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98c66-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="98c66-122">Authorization</span></span>|<span data-ttu-id="98c66-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98c66-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98c66-124">Accept</span><span class="sxs-lookup"><span data-stu-id="98c66-124">Accept</span></span>|<span data-ttu-id="98c66-125">application/json</span><span class="sxs-lookup"><span data-stu-id="98c66-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98c66-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98c66-126">Request body</span></span>
<span data-ttu-id="98c66-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="98c66-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="98c66-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="98c66-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="98c66-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98c66-129">Property</span></span>|<span data-ttu-id="98c66-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="98c66-130">Type</span></span>|<span data-ttu-id="98c66-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="98c66-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98c66-132">skip</span><span class="sxs-lookup"><span data-stu-id="98c66-132">skip</span></span>|<span data-ttu-id="98c66-133">Int32</span><span class="sxs-lookup"><span data-stu-id="98c66-133">Int32</span></span>|<span data-ttu-id="98c66-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="98c66-134">Not yet documented</span></span>|
|<span data-ttu-id="98c66-135">top</span><span class="sxs-lookup"><span data-stu-id="98c66-135">top</span></span>|<span data-ttu-id="98c66-136">Int32</span><span class="sxs-lookup"><span data-stu-id="98c66-136">Int32</span></span>|<span data-ttu-id="98c66-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="98c66-137">Not yet documented</span></span>|
|<span data-ttu-id="98c66-138">filter</span><span class="sxs-lookup"><span data-stu-id="98c66-138">filter</span></span>|<span data-ttu-id="98c66-139">String</span><span class="sxs-lookup"><span data-stu-id="98c66-139">String</span></span>|<span data-ttu-id="98c66-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="98c66-140">Not yet documented</span></span>|
|<span data-ttu-id="98c66-141">skipToken</span><span class="sxs-lookup"><span data-stu-id="98c66-141">skipToken</span></span>|<span data-ttu-id="98c66-142">String</span><span class="sxs-lookup"><span data-stu-id="98c66-142">String</span></span>|<span data-ttu-id="98c66-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="98c66-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="98c66-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="98c66-144">Response</span></span>
<span data-ttu-id="98c66-145">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98c66-145">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98c66-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98c66-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="98c66-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98c66-147">Request</span></span>
<span data-ttu-id="98c66-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98c66-148">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="98c66-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="98c66-149">Response</span></span>
<span data-ttu-id="98c66-150">No objeto response mostrado aqui pode estar truncado para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="98c66-150">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="98c66-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98c66-151">All of the properties will be returned from an actual call.</span></span>

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




