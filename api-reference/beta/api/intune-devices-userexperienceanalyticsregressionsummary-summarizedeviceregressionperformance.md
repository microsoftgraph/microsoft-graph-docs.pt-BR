---
title: função summarizeDeviceRegressionPerformance
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 51b89f20bd8c6d8df789d2e10ce896109d091e9a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48047480"
---
# <a name="summarizedeviceregressionperformance-function"></a><span data-ttu-id="98b90-103">função summarizeDeviceRegressionPerformance</span><span class="sxs-lookup"><span data-stu-id="98b90-103">summarizeDeviceRegressionPerformance function</span></span>

<span data-ttu-id="98b90-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98b90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98b90-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="98b90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98b90-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="98b90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98b90-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="98b90-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="98b90-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="98b90-108">Prerequisites</span></span>
<span data-ttu-id="98b90-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98b90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98b90-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="98b90-111">Permission type</span></span>|<span data-ttu-id="98b90-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="98b90-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="98b90-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="98b90-113">Delegated (work or school account)</span></span>|<span data-ttu-id="98b90-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="98b90-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="98b90-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="98b90-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="98b90-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="98b90-116">Not supported.</span></span>|
|<span data-ttu-id="98b90-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="98b90-117">Application</span></span>|<span data-ttu-id="98b90-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="98b90-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="98b90-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="98b90-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsRegressionSummary/summarizeDeviceRegressionPerformance
```

## <a name="request-headers"></a><span data-ttu-id="98b90-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="98b90-120">Request headers</span></span>
|<span data-ttu-id="98b90-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="98b90-121">Header</span></span>|<span data-ttu-id="98b90-122">Valor</span><span class="sxs-lookup"><span data-stu-id="98b90-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="98b90-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="98b90-123">Authorization</span></span>|<span data-ttu-id="98b90-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="98b90-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="98b90-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="98b90-125">Accept</span></span>|<span data-ttu-id="98b90-126">application/json</span><span class="sxs-lookup"><span data-stu-id="98b90-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="98b90-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="98b90-127">Request body</span></span>
<span data-ttu-id="98b90-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="98b90-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="98b90-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="98b90-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="98b90-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98b90-130">Property</span></span>|<span data-ttu-id="98b90-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="98b90-131">Type</span></span>|<span data-ttu-id="98b90-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="98b90-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98b90-133">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="98b90-133">summarizeBy</span></span>|[<span data-ttu-id="98b90-134">userExperienceAnalyticsSummarizedBy</span><span class="sxs-lookup"><span data-stu-id="98b90-134">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="98b90-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="98b90-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="98b90-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="98b90-136">Response</span></span>
<span data-ttu-id="98b90-137">Se tiver êxito, essa função retornará um `200 OK` código de resposta e um [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="98b90-137">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsRegressionSummary](../resources/intune-devices-userexperienceanalyticsregressionsummary.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98b90-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="98b90-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="98b90-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="98b90-139">Request</span></span>
<span data-ttu-id="98b90-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="98b90-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsRegressionSummary/summarizeDeviceRegressionPerformance(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="98b90-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="98b90-141">Response</span></span>
<span data-ttu-id="98b90-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="98b90-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 154

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsRegressionSummary",
    "id": "41683327-3327-4168-2733-684127336841"
  }
}
```






