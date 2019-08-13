---
title: função managedDeviceEnrollmentAbandonmentSummary
description: Metadados para o relatório de Resumo de abandono de registro
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4d988136da29680bd32b2ff24427bbf69135ab10
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350773"
---
# <a name="manageddeviceenrollmentabandonmentsummary-function"></a><span data-ttu-id="9c2cf-103">função managedDeviceEnrollmentAbandonmentSummary</span><span class="sxs-lookup"><span data-stu-id="9c2cf-103">managedDeviceEnrollmentAbandonmentSummary function</span></span>

> <span data-ttu-id="9c2cf-104">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9c2cf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9c2cf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9c2cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9c2cf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9c2cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c2cf-107">Metadados para o relatório de Resumo de abandono de registro</span><span class="sxs-lookup"><span data-stu-id="9c2cf-107">Metadata for Enrollment abandonment summary report</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9c2cf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9c2cf-108">Prerequisites</span></span>
<span data-ttu-id="9c2cf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c2cf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c2cf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c2cf-111">Permission type</span></span>|<span data-ttu-id="9c2cf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9c2cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c2cf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c2cf-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9c2cf-114">&nbsp;&nbsp; **Troublshooting**</span><span class="sxs-lookup"><span data-stu-id="9c2cf-114">&nbsp; &nbsp; **Troublshooting**</span></span> | <span data-ttu-id="9c2cf-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="9c2cf-115">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="9c2cf-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c2cf-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c2cf-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c2cf-117">Not supported.</span></span>|
|<span data-ttu-id="9c2cf-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9c2cf-118">Application</span></span>|<span data-ttu-id="9c2cf-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c2cf-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c2cf-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c2cf-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/managedDeviceEnrollmentAbandonmentSummary
```

## <a name="request-headers"></a><span data-ttu-id="9c2cf-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c2cf-121">Request headers</span></span>
|<span data-ttu-id="9c2cf-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9c2cf-122">Header</span></span>|<span data-ttu-id="9c2cf-123">Valor</span><span class="sxs-lookup"><span data-stu-id="9c2cf-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c2cf-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c2cf-124">Authorization</span></span>|<span data-ttu-id="9c2cf-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c2cf-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c2cf-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9c2cf-126">Accept</span></span>|<span data-ttu-id="9c2cf-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9c2cf-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c2cf-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c2cf-128">Request body</span></span>
<span data-ttu-id="9c2cf-129">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="9c2cf-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="9c2cf-130">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="9c2cf-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="9c2cf-131">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c2cf-131">Property</span></span>|<span data-ttu-id="9c2cf-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c2cf-132">Type</span></span>|<span data-ttu-id="9c2cf-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c2cf-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c2cf-134">skip</span><span class="sxs-lookup"><span data-stu-id="9c2cf-134">skip</span></span>|<span data-ttu-id="9c2cf-135">Int32</span><span class="sxs-lookup"><span data-stu-id="9c2cf-135">Int32</span></span>|<span data-ttu-id="9c2cf-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9c2cf-136">Not yet documented</span></span>|
|<span data-ttu-id="9c2cf-137">top</span><span class="sxs-lookup"><span data-stu-id="9c2cf-137">top</span></span>|<span data-ttu-id="9c2cf-138">Int32</span><span class="sxs-lookup"><span data-stu-id="9c2cf-138">Int32</span></span>|<span data-ttu-id="9c2cf-139">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9c2cf-139">Not yet documented</span></span>|
|<span data-ttu-id="9c2cf-140">filter</span><span class="sxs-lookup"><span data-stu-id="9c2cf-140">filter</span></span>|<span data-ttu-id="9c2cf-141">String</span><span class="sxs-lookup"><span data-stu-id="9c2cf-141">String</span></span>|<span data-ttu-id="9c2cf-142">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9c2cf-142">Not yet documented</span></span>|
|<span data-ttu-id="9c2cf-143">skipToken</span><span class="sxs-lookup"><span data-stu-id="9c2cf-143">skipToken</span></span>|<span data-ttu-id="9c2cf-144">String</span><span class="sxs-lookup"><span data-stu-id="9c2cf-144">String</span></span>|<span data-ttu-id="9c2cf-145">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9c2cf-145">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9c2cf-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c2cf-146">Response</span></span>
<span data-ttu-id="9c2cf-147">Se tiver êxito, este método retornará um código de resposta `200 OK` e um [relatório](../resources/intune-shared-report.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9c2cf-147">If successful, this function returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c2cf-148">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c2cf-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="9c2cf-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c2cf-149">Request</span></span>
<span data-ttu-id="9c2cf-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c2cf-150">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/reports/managedDeviceEnrollmentAbandonmentSummary(skip=4,top=3,filter='parameterValue',skipToken='parameterValue')
```

### <a name="response"></a><span data-ttu-id="9c2cf-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c2cf-151">Response</span></span>
<span data-ttu-id="9c2cf-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9c2cf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








