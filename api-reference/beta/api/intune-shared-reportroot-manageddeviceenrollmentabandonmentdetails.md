---
title: função managedDeviceEnrollmentAbandonmentDetails
description: Metadados para o relatório de detalhes de abandono de inscrição
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8e2031657c3aff7d09d126b6eff01beaf34813a0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939907"
---
# <a name="manageddeviceenrollmentabandonmentdetails-function"></a><span data-ttu-id="94f0d-103">função managedDeviceEnrollmentAbandonmentDetails</span><span class="sxs-lookup"><span data-stu-id="94f0d-103">managedDeviceEnrollmentAbandonmentDetails function</span></span>

> <span data-ttu-id="94f0d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="94f0d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94f0d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="94f0d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94f0d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="94f0d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94f0d-107">Metadados para o relatório de detalhes de abandono de inscrição</span><span class="sxs-lookup"><span data-stu-id="94f0d-107">Metadata for Enrollment abandonment details report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="94f0d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="94f0d-108">Prerequisites</span></span>
<span data-ttu-id="94f0d-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94f0d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94f0d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94f0d-111">Permission type</span></span>|<span data-ttu-id="94f0d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="94f0d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94f0d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94f0d-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="94f0d-114">&nbsp;&nbsp; **Frequentes**</span><span class="sxs-lookup"><span data-stu-id="94f0d-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="94f0d-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="94f0d-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="94f0d-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94f0d-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94f0d-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94f0d-117">Not supported.</span></span>|
|<span data-ttu-id="94f0d-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94f0d-118">Application</span></span>|<span data-ttu-id="94f0d-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94f0d-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94f0d-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94f0d-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentDetails
```

## <a name="request-headers"></a><span data-ttu-id="94f0d-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94f0d-121">Request headers</span></span>
|<span data-ttu-id="94f0d-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94f0d-122">Header</span></span>|<span data-ttu-id="94f0d-123">Valor</span><span class="sxs-lookup"><span data-stu-id="94f0d-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94f0d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="94f0d-124">Authorization</span></span>|<span data-ttu-id="94f0d-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94f0d-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94f0d-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="94f0d-126">Accept</span></span>|<span data-ttu-id="94f0d-127">application/json</span><span class="sxs-lookup"><span data-stu-id="94f0d-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94f0d-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94f0d-128">Request body</span></span>
<span data-ttu-id="94f0d-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="94f0d-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="94f0d-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="94f0d-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="94f0d-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94f0d-131">Property</span></span>|<span data-ttu-id="94f0d-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="94f0d-132">Type</span></span>|<span data-ttu-id="94f0d-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="94f0d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94f0d-134">skip</span><span class="sxs-lookup"><span data-stu-id="94f0d-134">skip</span></span>|<span data-ttu-id="94f0d-135">Int32</span><span class="sxs-lookup"><span data-stu-id="94f0d-135">Int32</span></span>|<span data-ttu-id="94f0d-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="94f0d-136">Not yet documented</span></span>|
|<span data-ttu-id="94f0d-137">top</span><span class="sxs-lookup"><span data-stu-id="94f0d-137">top</span></span>|<span data-ttu-id="94f0d-138">Int32</span><span class="sxs-lookup"><span data-stu-id="94f0d-138">Int32</span></span>|<span data-ttu-id="94f0d-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="94f0d-139">Not yet documented</span></span>|
|<span data-ttu-id="94f0d-140">filter</span><span class="sxs-lookup"><span data-stu-id="94f0d-140">filter</span></span>|<span data-ttu-id="94f0d-141">String</span><span class="sxs-lookup"><span data-stu-id="94f0d-141">String</span></span>|<span data-ttu-id="94f0d-142">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="94f0d-142">Not yet documented</span></span>|
|<span data-ttu-id="94f0d-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="94f0d-143">skipToken</span></span>|<span data-ttu-id="94f0d-144">String</span><span class="sxs-lookup"><span data-stu-id="94f0d-144">String</span></span>|<span data-ttu-id="94f0d-145">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="94f0d-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="94f0d-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="94f0d-146">Response</span></span>
<span data-ttu-id="94f0d-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94f0d-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94f0d-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94f0d-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="94f0d-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94f0d-149">Request</span></span>
<span data-ttu-id="94f0d-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94f0d-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentDetails(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="94f0d-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="94f0d-151">Response</span></span>
<span data-ttu-id="94f0d-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94f0d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





