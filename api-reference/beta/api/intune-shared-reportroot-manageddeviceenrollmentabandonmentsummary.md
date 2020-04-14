---
title: função managedDeviceEnrollmentAbandonmentSummary
description: Metadados para o relatório de Resumo de abandono de registro
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4ebb529e5c56ee62a6836be5e27914e1ed530155
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470339"
---
# <a name="manageddeviceenrollmentabandonmentsummary-function"></a><span data-ttu-id="e7c76-103">função managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="e7c76-103">managedDeviceEnrollmentAbandonmentSummary function</span></span>

<span data-ttu-id="e7c76-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7c76-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7c76-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e7c76-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e7c76-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e7c76-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7c76-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7c76-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7c76-108">Metadados para o relatório de Resumo de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="e7c76-108">Metadata for Enrollment abandonment summary report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7c76-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e7c76-109">Prerequisites</span></span>
<span data-ttu-id="e7c76-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e7c76-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7c76-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e7c76-112">Permission type</span></span>|<span data-ttu-id="e7c76-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e7c76-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7c76-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e7c76-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e7c76-115">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="e7c76-115">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="e7c76-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7c76-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="e7c76-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e7c76-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7c76-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e7c76-118">Not supported.</span></span>|
|<span data-ttu-id="e7c76-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e7c76-119">Application</span></span>||
| <span data-ttu-id="e7c76-120">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="e7c76-120">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="e7c76-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="e7c76-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7c76-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e7c76-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentSummary
```

## <a name="request-headers"></a><span data-ttu-id="e7c76-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e7c76-123">Request headers</span></span>
|<span data-ttu-id="e7c76-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e7c76-124">Header</span></span>|<span data-ttu-id="e7c76-125">Valor</span><span class="sxs-lookup"><span data-stu-id="e7c76-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7c76-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="e7c76-126">Authorization</span></span>|<span data-ttu-id="e7c76-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e7c76-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7c76-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e7c76-128">Accept</span></span>|<span data-ttu-id="e7c76-129">application/json</span><span class="sxs-lookup"><span data-stu-id="e7c76-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7c76-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e7c76-130">Request body</span></span>
<span data-ttu-id="e7c76-131">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="e7c76-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e7c76-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="e7c76-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e7c76-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e7c76-133">Property</span></span>|<span data-ttu-id="e7c76-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="e7c76-134">Type</span></span>|<span data-ttu-id="e7c76-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7c76-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7c76-136">skip</span><span class="sxs-lookup"><span data-stu-id="e7c76-136">skip</span></span>|<span data-ttu-id="e7c76-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e7c76-137">Int32</span></span>|<span data-ttu-id="e7c76-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e7c76-138">Not yet documented</span></span>|
|<span data-ttu-id="e7c76-139">top</span><span class="sxs-lookup"><span data-stu-id="e7c76-139">top</span></span>|<span data-ttu-id="e7c76-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e7c76-140">Int32</span></span>|<span data-ttu-id="e7c76-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e7c76-141">Not yet documented</span></span>|
|<span data-ttu-id="e7c76-142">filter</span><span class="sxs-lookup"><span data-stu-id="e7c76-142">filter</span></span>|<span data-ttu-id="e7c76-143">String</span><span class="sxs-lookup"><span data-stu-id="e7c76-143">String</span></span>|<span data-ttu-id="e7c76-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e7c76-144">Not yet documented</span></span>|
|<span data-ttu-id="e7c76-145">skipToken</span><span class="sxs-lookup"><span data-stu-id="e7c76-145">skipToken</span></span>|<span data-ttu-id="e7c76-146">String</span><span class="sxs-lookup"><span data-stu-id="e7c76-146">String</span></span>|<span data-ttu-id="e7c76-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e7c76-147">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e7c76-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7c76-148">Response</span></span>
<span data-ttu-id="e7c76-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e7c76-149">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7c76-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e7c76-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7c76-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e7c76-151">Request</span></span>
<span data-ttu-id="e7c76-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e7c76-152">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentSummary(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e7c76-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="e7c76-153">Response</span></span>
<span data-ttu-id="e7c76-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e7c76-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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











