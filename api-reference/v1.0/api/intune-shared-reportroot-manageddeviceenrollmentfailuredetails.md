---
title: Função managedDeviceEnrollmentFailureDetails
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1539992ad475c2339a33aae809bc477d5da4e772
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732222"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="197ed-103">Função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="197ed-103">managedDeviceEnrollmentFailureDetails function</span></span>

<span data-ttu-id="197ed-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="197ed-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="197ed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="197ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="197ed-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="197ed-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="197ed-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="197ed-107">Prerequisites</span></span>
<span data-ttu-id="197ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="197ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="197ed-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="197ed-110">Permission type</span></span>|<span data-ttu-id="197ed-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="197ed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="197ed-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="197ed-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="197ed-113">&nbsp;&nbsp;Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="197ed-113">&nbsp; &nbsp; Troubleshooting</span></span> | <span data-ttu-id="197ed-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="197ed-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="197ed-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="197ed-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="197ed-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="197ed-116">Not supported.</span></span>|
|<span data-ttu-id="197ed-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="197ed-117">Application</span></span>|<span data-ttu-id="197ed-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="197ed-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="197ed-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="197ed-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="197ed-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="197ed-120">Request headers</span></span>
|<span data-ttu-id="197ed-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="197ed-121">Header</span></span>|<span data-ttu-id="197ed-122">Valor</span><span class="sxs-lookup"><span data-stu-id="197ed-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="197ed-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="197ed-123">Authorization</span></span>|<span data-ttu-id="197ed-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="197ed-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="197ed-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="197ed-125">Accept</span></span>|<span data-ttu-id="197ed-126">application/json</span><span class="sxs-lookup"><span data-stu-id="197ed-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="197ed-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="197ed-127">Request body</span></span>
<span data-ttu-id="197ed-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="197ed-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="197ed-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="197ed-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="197ed-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="197ed-130">Property</span></span>|<span data-ttu-id="197ed-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="197ed-131">Type</span></span>|<span data-ttu-id="197ed-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="197ed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="197ed-133">skip</span><span class="sxs-lookup"><span data-stu-id="197ed-133">skip</span></span>|<span data-ttu-id="197ed-134">Int32</span><span class="sxs-lookup"><span data-stu-id="197ed-134">Int32</span></span>|<span data-ttu-id="197ed-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="197ed-135">Not yet documented</span></span>|
|<span data-ttu-id="197ed-136">top</span><span class="sxs-lookup"><span data-stu-id="197ed-136">top</span></span>|<span data-ttu-id="197ed-137">Int32</span><span class="sxs-lookup"><span data-stu-id="197ed-137">Int32</span></span>|<span data-ttu-id="197ed-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="197ed-138">Not yet documented</span></span>|
|<span data-ttu-id="197ed-139">filter</span><span class="sxs-lookup"><span data-stu-id="197ed-139">filter</span></span>|<span data-ttu-id="197ed-140">String</span><span class="sxs-lookup"><span data-stu-id="197ed-140">String</span></span>|<span data-ttu-id="197ed-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="197ed-141">Not yet documented</span></span>|
|<span data-ttu-id="197ed-142">skipToken</span><span class="sxs-lookup"><span data-stu-id="197ed-142">skipToken</span></span>|<span data-ttu-id="197ed-143">String</span><span class="sxs-lookup"><span data-stu-id="197ed-143">String</span></span>|<span data-ttu-id="197ed-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="197ed-144">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="197ed-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="197ed-145">Response</span></span>
<span data-ttu-id="197ed-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="197ed-146">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="197ed-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="197ed-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="197ed-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="197ed-148">Request</span></span>
<span data-ttu-id="197ed-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="197ed-149">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="197ed-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="197ed-150">Response</span></span>
<span data-ttu-id="197ed-151">O objeto de resposta mostrado aqui pode ser truncado para brevidade.</span><span class="sxs-lookup"><span data-stu-id="197ed-151">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="197ed-152">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="197ed-152">All of the properties will be returned from an actual call.</span></span>

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










