---
title: função managedDeviceEnrollmentFailureDetails
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c234181bb70ca0df11cff01b67eb7d6fa60e27ca
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32576794"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="710ad-103">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="710ad-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="710ad-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="710ad-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="710ad-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="710ad-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="710ad-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="710ad-106">Prerequisites</span></span>
<span data-ttu-id="710ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="710ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="710ad-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="710ad-109">Permission type</span></span>|<span data-ttu-id="710ad-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="710ad-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="710ad-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="710ad-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="710ad-112">&nbsp;&nbsp; Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="710ad-112">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="710ad-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="710ad-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="710ad-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="710ad-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="710ad-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="710ad-115">Not supported.</span></span>|
|<span data-ttu-id="710ad-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="710ad-116">Application</span></span>|<span data-ttu-id="710ad-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="710ad-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="710ad-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="710ad-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="710ad-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="710ad-119">Request headers</span></span>
|<span data-ttu-id="710ad-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="710ad-120">Header</span></span>|<span data-ttu-id="710ad-121">Valor</span><span class="sxs-lookup"><span data-stu-id="710ad-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="710ad-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="710ad-122">Authorization</span></span>|<span data-ttu-id="710ad-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="710ad-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="710ad-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="710ad-124">Accept</span></span>|<span data-ttu-id="710ad-125">application/json</span><span class="sxs-lookup"><span data-stu-id="710ad-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="710ad-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="710ad-126">Request body</span></span>
<span data-ttu-id="710ad-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="710ad-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="710ad-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="710ad-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="710ad-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="710ad-129">Property</span></span>|<span data-ttu-id="710ad-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="710ad-130">Type</span></span>|<span data-ttu-id="710ad-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="710ad-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="710ad-132">skip</span><span class="sxs-lookup"><span data-stu-id="710ad-132">skip</span></span>|<span data-ttu-id="710ad-133">Int32</span><span class="sxs-lookup"><span data-stu-id="710ad-133">Int32</span></span>|<span data-ttu-id="710ad-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="710ad-134">Not yet documented</span></span>|
|<span data-ttu-id="710ad-135">top</span><span class="sxs-lookup"><span data-stu-id="710ad-135">top</span></span>|<span data-ttu-id="710ad-136">Int32</span><span class="sxs-lookup"><span data-stu-id="710ad-136">Int32</span></span>|<span data-ttu-id="710ad-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="710ad-137">Not yet documented</span></span>|
|<span data-ttu-id="710ad-138">filtro</span><span class="sxs-lookup"><span data-stu-id="710ad-138">filter</span></span>|<span data-ttu-id="710ad-139">String</span><span class="sxs-lookup"><span data-stu-id="710ad-139">String</span></span>|<span data-ttu-id="710ad-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="710ad-140">Not yet documented</span></span>|
|<span data-ttu-id="710ad-141">skipToken</span><span class="sxs-lookup"><span data-stu-id="710ad-141">skipToken</span></span>|<span data-ttu-id="710ad-142">String</span><span class="sxs-lookup"><span data-stu-id="710ad-142">String</span></span>|<span data-ttu-id="710ad-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="710ad-143">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="710ad-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="710ad-144">Response</span></span>
<span data-ttu-id="710ad-145">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="710ad-145">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="710ad-146">Exemplo</span><span class="sxs-lookup"><span data-stu-id="710ad-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="710ad-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="710ad-147">Request</span></span>
<span data-ttu-id="710ad-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="710ad-148">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="710ad-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="710ad-149">Response</span></span>
<span data-ttu-id="710ad-150">O objeto de resposta mostrado aqui pode estar truncado por brevidade.</span><span class="sxs-lookup"><span data-stu-id="710ad-150">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="710ad-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="710ad-151">All of the properties will be returned from an actual call.</span></span>

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




