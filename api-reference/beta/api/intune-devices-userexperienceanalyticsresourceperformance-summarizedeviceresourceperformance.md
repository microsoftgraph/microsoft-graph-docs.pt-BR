---
title: Função summarizeDeviceResourcePerformance
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 54f0c6948f90739ad28e5a69b7b1376afc0c6f90
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162183"
---
# <a name="summarizedeviceresourceperformance-function"></a><span data-ttu-id="2f4a4-103">Função summarizeDeviceResourcePerformance</span><span class="sxs-lookup"><span data-stu-id="2f4a4-103">summarizeDeviceResourcePerformance function</span></span>

<span data-ttu-id="2f4a4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f4a4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f4a4-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f4a4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f4a4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f4a4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f4a4-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2f4a4-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f4a4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2f4a4-108">Prerequisites</span></span>
<span data-ttu-id="2f4a4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f4a4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f4a4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2f4a4-111">Permission type</span></span>|<span data-ttu-id="2f4a4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2f4a4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f4a4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2f4a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2f4a4-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f4a4-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2f4a4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2f4a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f4a4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f4a4-116">Not supported.</span></span>|
|<span data-ttu-id="2f4a4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f4a4-117">Application</span></span>|<span data-ttu-id="2f4a4-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f4a4-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f4a4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2f4a4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsResourcePerformance/summarizeDeviceResourcePerformance
```

## <a name="request-headers"></a><span data-ttu-id="2f4a4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2f4a4-120">Request headers</span></span>
|<span data-ttu-id="2f4a4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f4a4-121">Header</span></span>|<span data-ttu-id="2f4a4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2f4a4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f4a4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2f4a4-123">Authorization</span></span>|<span data-ttu-id="2f4a4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2f4a4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f4a4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2f4a4-125">Accept</span></span>|<span data-ttu-id="2f4a4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2f4a4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f4a4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2f4a4-127">Request body</span></span>
<span data-ttu-id="2f4a4-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="2f4a4-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="2f4a4-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="2f4a4-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="2f4a4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f4a4-130">Property</span></span>|<span data-ttu-id="2f4a4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f4a4-131">Type</span></span>|<span data-ttu-id="2f4a4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f4a4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f4a4-133">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="2f4a4-133">summarizeBy</span></span>|[<span data-ttu-id="2f4a4-134">userExperienceAnalyticsSummarizedBy</span><span class="sxs-lookup"><span data-stu-id="2f4a4-134">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="2f4a4-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2f4a4-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2f4a4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f4a4-136">Response</span></span>
<span data-ttu-id="2f4a4-137">Se tiver êxito, esta função retornará um código de resposta e uma coleção `200 OK` [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2f4a4-137">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsResourcePerformance](../resources/intune-devices-userexperienceanalyticsresourceperformance.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f4a4-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f4a4-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f4a4-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2f4a4-139">Request</span></span>
<span data-ttu-id="2f4a4-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2f4a4-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsResourcePerformance/summarizeDeviceResourcePerformance(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="2f4a4-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2f4a4-141">Response</span></span>
<span data-ttu-id="2f4a4-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2f4a4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 691

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsResourcePerformance",
      "id": "d34d78e8-78e8-d34d-e878-4dd3e8784dd3",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "model": "Model value",
      "deviceCount": 11,
      "manufacturer": "Manufacturer value",
      "cpuSpikeTimePercentage": 7.333333333333333,
      "ramSpikeTimePercentage": 7.333333333333333,
      "cpuSpikeTimeScore": 1,
      "cpuSpikeTimePercentageThreshold": 10.333333333333334,
      "ramSpikeTimeScore": 1,
      "ramSpikeTimePercentageThreshold": 10.333333333333334,
      "deviceResourcePerformanceScore": 14
    }
  ]
}
```




