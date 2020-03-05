---
title: função managedDeviceEnrollmentAbandonmentSummary
description: Metadados para o relatório de Resumo de abandono de registro
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e0ac224ec30110abd39675c1fcb8c64e3087185a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42458165"
---
# <a name="manageddeviceenrollmentabandonmentsummary-function"></a><span data-ttu-id="239f2-103">função managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="239f2-103">managedDeviceEnrollmentAbandonmentSummary function</span></span>

<span data-ttu-id="239f2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="239f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="239f2-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="239f2-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="239f2-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="239f2-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="239f2-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="239f2-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="239f2-108">Metadados para o relatório de Resumo de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="239f2-108">Metadata for Enrollment abandonment summary report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="239f2-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="239f2-109">Prerequisites</span></span>
<span data-ttu-id="239f2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="239f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="239f2-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="239f2-112">Permission type</span></span>|<span data-ttu-id="239f2-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="239f2-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="239f2-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="239f2-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="239f2-115">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="239f2-115">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="239f2-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="239f2-116">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="239f2-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="239f2-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="239f2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="239f2-118">Not supported.</span></span>|
|<span data-ttu-id="239f2-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="239f2-119">Application</span></span>||
| <span data-ttu-id="239f2-120">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="239f2-120">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="239f2-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="239f2-121">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="239f2-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="239f2-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentSummary
```

## <a name="request-headers"></a><span data-ttu-id="239f2-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="239f2-123">Request headers</span></span>
|<span data-ttu-id="239f2-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="239f2-124">Header</span></span>|<span data-ttu-id="239f2-125">Valor</span><span class="sxs-lookup"><span data-stu-id="239f2-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="239f2-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="239f2-126">Authorization</span></span>|<span data-ttu-id="239f2-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="239f2-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="239f2-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="239f2-128">Accept</span></span>|<span data-ttu-id="239f2-129">application/json</span><span class="sxs-lookup"><span data-stu-id="239f2-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="239f2-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="239f2-130">Request body</span></span>
<span data-ttu-id="239f2-131">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="239f2-131">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="239f2-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="239f2-132">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="239f2-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="239f2-133">Property</span></span>|<span data-ttu-id="239f2-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="239f2-134">Type</span></span>|<span data-ttu-id="239f2-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="239f2-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="239f2-136">skip</span><span class="sxs-lookup"><span data-stu-id="239f2-136">skip</span></span>|<span data-ttu-id="239f2-137">Int32</span><span class="sxs-lookup"><span data-stu-id="239f2-137">Int32</span></span>|<span data-ttu-id="239f2-138">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="239f2-138">Not yet documented</span></span>|
|<span data-ttu-id="239f2-139">top</span><span class="sxs-lookup"><span data-stu-id="239f2-139">top</span></span>|<span data-ttu-id="239f2-140">Int32</span><span class="sxs-lookup"><span data-stu-id="239f2-140">Int32</span></span>|<span data-ttu-id="239f2-141">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="239f2-141">Not yet documented</span></span>|
|<span data-ttu-id="239f2-142">filter</span><span class="sxs-lookup"><span data-stu-id="239f2-142">filter</span></span>|<span data-ttu-id="239f2-143">String</span><span class="sxs-lookup"><span data-stu-id="239f2-143">String</span></span>|<span data-ttu-id="239f2-144">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="239f2-144">Not yet documented</span></span>|
|<span data-ttu-id="239f2-145">skipToken</span><span class="sxs-lookup"><span data-stu-id="239f2-145">skipToken</span></span>|<span data-ttu-id="239f2-146">String</span><span class="sxs-lookup"><span data-stu-id="239f2-146">String</span></span>|<span data-ttu-id="239f2-147">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="239f2-147">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="239f2-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="239f2-148">Response</span></span>
<span data-ttu-id="239f2-149">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="239f2-149">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="239f2-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="239f2-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="239f2-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="239f2-151">Request</span></span>
<span data-ttu-id="239f2-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="239f2-152">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentSummary(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="239f2-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="239f2-153">Response</span></span>
<span data-ttu-id="239f2-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="239f2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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













