---
title: função managedDeviceEnrollmentFailureDetails
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b28adb643367b9bdc31b08e78bacceae48642422
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43411575"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="b1a57-103">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="b1a57-103">managedDeviceEnrollmentFailureDetails function</span></span>

<span data-ttu-id="b1a57-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1a57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1a57-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1a57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1a57-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1a57-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1a57-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b1a57-107">Prerequisites</span></span>
<span data-ttu-id="b1a57-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1a57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1a57-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1a57-110">Permission type</span></span>|<span data-ttu-id="b1a57-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b1a57-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1a57-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1a57-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b1a57-113">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="b1a57-113">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="b1a57-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1a57-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b1a57-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1a57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1a57-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1a57-116">Not supported.</span></span>|
|<span data-ttu-id="b1a57-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1a57-117">Application</span></span>|<span data-ttu-id="b1a57-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b1a57-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1a57-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1a57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="b1a57-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b1a57-120">Request headers</span></span>
|<span data-ttu-id="b1a57-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b1a57-121">Header</span></span>|<span data-ttu-id="b1a57-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b1a57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1a57-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b1a57-123">Authorization</span></span>|<span data-ttu-id="b1a57-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b1a57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1a57-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b1a57-125">Accept</span></span>|<span data-ttu-id="b1a57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1a57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1a57-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1a57-127">Request body</span></span>
<span data-ttu-id="b1a57-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="b1a57-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="b1a57-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="b1a57-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="b1a57-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1a57-130">Property</span></span>|<span data-ttu-id="b1a57-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1a57-131">Type</span></span>|<span data-ttu-id="b1a57-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1a57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1a57-133">skip</span><span class="sxs-lookup"><span data-stu-id="b1a57-133">skip</span></span>|<span data-ttu-id="b1a57-134">Int32</span><span class="sxs-lookup"><span data-stu-id="b1a57-134">Int32</span></span>|<span data-ttu-id="b1a57-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1a57-135">Not yet documented</span></span>|
|<span data-ttu-id="b1a57-136">top</span><span class="sxs-lookup"><span data-stu-id="b1a57-136">top</span></span>|<span data-ttu-id="b1a57-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b1a57-137">Int32</span></span>|<span data-ttu-id="b1a57-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1a57-138">Not yet documented</span></span>|
|<span data-ttu-id="b1a57-139">filter</span><span class="sxs-lookup"><span data-stu-id="b1a57-139">filter</span></span>|<span data-ttu-id="b1a57-140">String</span><span class="sxs-lookup"><span data-stu-id="b1a57-140">String</span></span>|<span data-ttu-id="b1a57-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1a57-141">Not yet documented</span></span>|
|<span data-ttu-id="b1a57-142">skipToken</span><span class="sxs-lookup"><span data-stu-id="b1a57-142">skipToken</span></span>|<span data-ttu-id="b1a57-143">String</span><span class="sxs-lookup"><span data-stu-id="b1a57-143">String</span></span>|<span data-ttu-id="b1a57-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1a57-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="b1a57-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1a57-145">Response</span></span>
<span data-ttu-id="b1a57-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1a57-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1a57-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1a57-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="b1a57-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b1a57-148">Request</span></span>
<span data-ttu-id="b1a57-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1a57-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="b1a57-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1a57-150">Response</span></span>
<span data-ttu-id="b1a57-151">O objeto de resposta mostrado aqui pode estar truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="b1a57-151">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b1a57-152">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b1a57-152">All of the properties will be returned from an actual call.</span></span>

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







