---
title: função managedDeviceEnrollmentFailureDetails
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 90415987d5708015cd639d4e2d7dd9d1866264c4
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939589"
---
# <a name="manageddeviceenrollmentfailuredetails-function"></a><span data-ttu-id="e8119-103">função managedDeviceEnrollmentFailureDetails</span><span class="sxs-lookup"><span data-stu-id="e8119-103">managedDeviceEnrollmentFailureDetails function</span></span>

> <span data-ttu-id="e8119-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e8119-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e8119-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e8119-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8119-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8119-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8119-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e8119-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e8119-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8119-108">Prerequisites</span></span>
<span data-ttu-id="e8119-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8119-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8119-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8119-111">Permission type</span></span>|<span data-ttu-id="e8119-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e8119-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8119-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8119-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e8119-114">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="e8119-114">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="e8119-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8119-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e8119-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8119-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8119-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8119-117">Not supported.</span></span>|
|<span data-ttu-id="e8119-118">Application</span><span class="sxs-lookup"><span data-stu-id="e8119-118">Application</span></span>||
| <span data-ttu-id="e8119-119">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="e8119-119">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="e8119-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8119-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8119-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8119-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentFailureDetails
```

## <a name="request-headers"></a><span data-ttu-id="e8119-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8119-122">Request headers</span></span>
|<span data-ttu-id="e8119-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8119-123">Header</span></span>|<span data-ttu-id="e8119-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e8119-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8119-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8119-125">Authorization</span></span>|<span data-ttu-id="e8119-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8119-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8119-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e8119-127">Accept</span></span>|<span data-ttu-id="e8119-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e8119-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8119-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8119-129">Request body</span></span>
<span data-ttu-id="e8119-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="e8119-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e8119-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8119-131">Property</span></span>|<span data-ttu-id="e8119-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8119-132">Type</span></span>|<span data-ttu-id="e8119-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8119-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8119-134">filter</span><span class="sxs-lookup"><span data-stu-id="e8119-134">filter</span></span>|<span data-ttu-id="e8119-135">String</span><span class="sxs-lookup"><span data-stu-id="e8119-135">String</span></span>|<span data-ttu-id="e8119-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e8119-136">Not yet documented</span></span>|
|<span data-ttu-id="e8119-137">skipToken</span><span class="sxs-lookup"><span data-stu-id="e8119-137">skipToken</span></span>|<span data-ttu-id="e8119-138">String</span><span class="sxs-lookup"><span data-stu-id="e8119-138">String</span></span>|<span data-ttu-id="e8119-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e8119-139">Not yet documented</span></span>|
|<span data-ttu-id="e8119-140">skip</span><span class="sxs-lookup"><span data-stu-id="e8119-140">skip</span></span>|<span data-ttu-id="e8119-141">Int32</span><span class="sxs-lookup"><span data-stu-id="e8119-141">Int32</span></span>|<span data-ttu-id="e8119-142">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e8119-142">Not yet documented</span></span>|
|<span data-ttu-id="e8119-143">top</span><span class="sxs-lookup"><span data-stu-id="e8119-143">top</span></span>|<span data-ttu-id="e8119-144">Int32</span><span class="sxs-lookup"><span data-stu-id="e8119-144">Int32</span></span>|<span data-ttu-id="e8119-145">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e8119-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e8119-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8119-146">Response</span></span>
<span data-ttu-id="e8119-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e8119-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8119-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8119-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="e8119-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8119-149">Request</span></span>
<span data-ttu-id="e8119-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8119-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentFailureDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e8119-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8119-151">Response</span></span>
<span data-ttu-id="e8119-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8119-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











