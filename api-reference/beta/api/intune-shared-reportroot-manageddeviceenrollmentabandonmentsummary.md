---
title: função managedDeviceEnrollmentAbandonmentSummary
description: Metadados para o relatório de Resumo de abandono de registro
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7792bd9aef146b3b12b005510e2a955d072c802f
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37195829"
---
# <a name="manageddeviceenrollmentabandonmentsummary-function"></a><span data-ttu-id="c3074-103">função managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="c3074-103">managedDeviceEnrollmentAbandonmentSummary function</span></span>

> <span data-ttu-id="c3074-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c3074-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c3074-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c3074-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c3074-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c3074-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3074-107">Metadados para o relatório de Resumo de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="c3074-107">Metadata for Enrollment abandonment summary report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c3074-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c3074-108">Prerequisites</span></span>
<span data-ttu-id="c3074-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3074-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3074-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3074-111">Permission type</span></span>|<span data-ttu-id="c3074-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c3074-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3074-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3074-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="c3074-114">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="c3074-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="c3074-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3074-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="c3074-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3074-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3074-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3074-117">Not supported.</span></span>|
|<span data-ttu-id="c3074-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3074-118">Application</span></span>||
| <span data-ttu-id="c3074-119">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="c3074-119">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="c3074-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="c3074-120">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3074-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3074-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentSummary
```

## <a name="request-headers"></a><span data-ttu-id="c3074-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c3074-122">Request headers</span></span>
|<span data-ttu-id="c3074-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c3074-123">Header</span></span>|<span data-ttu-id="c3074-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c3074-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3074-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c3074-125">Authorization</span></span>|<span data-ttu-id="c3074-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c3074-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3074-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c3074-127">Accept</span></span>|<span data-ttu-id="c3074-128">application/json</span><span class="sxs-lookup"><span data-stu-id="c3074-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3074-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3074-129">Request body</span></span>
<span data-ttu-id="c3074-130">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="c3074-130">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="c3074-131">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="c3074-131">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="c3074-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3074-132">Property</span></span>|<span data-ttu-id="c3074-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3074-133">Type</span></span>|<span data-ttu-id="c3074-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3074-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3074-135">skip</span><span class="sxs-lookup"><span data-stu-id="c3074-135">skip</span></span>|<span data-ttu-id="c3074-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c3074-136">Int32</span></span>|<span data-ttu-id="c3074-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c3074-137">Not yet documented</span></span>|
|<span data-ttu-id="c3074-138">top</span><span class="sxs-lookup"><span data-stu-id="c3074-138">top</span></span>|<span data-ttu-id="c3074-139">Int32</span><span class="sxs-lookup"><span data-stu-id="c3074-139">Int32</span></span>|<span data-ttu-id="c3074-140">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c3074-140">Not yet documented</span></span>|
|<span data-ttu-id="c3074-141">filter</span><span class="sxs-lookup"><span data-stu-id="c3074-141">filter</span></span>|<span data-ttu-id="c3074-142">String</span><span class="sxs-lookup"><span data-stu-id="c3074-142">String</span></span>|<span data-ttu-id="c3074-143">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c3074-143">Not yet documented</span></span>|
|<span data-ttu-id="c3074-144">skipToken</span><span class="sxs-lookup"><span data-stu-id="c3074-144">skipToken</span></span>|<span data-ttu-id="c3074-145">String</span><span class="sxs-lookup"><span data-stu-id="c3074-145">String</span></span>|<span data-ttu-id="c3074-146">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c3074-146">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c3074-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3074-147">Response</span></span>
<span data-ttu-id="c3074-148">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c3074-148">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3074-149">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c3074-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="c3074-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c3074-150">Request</span></span>
<span data-ttu-id="c3074-151">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c3074-151">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentSummary(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="c3074-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3074-152">Response</span></span>
<span data-ttu-id="c3074-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c3074-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









