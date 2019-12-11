---
title: função summarizeDevicePerformanceDevices
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4ec7d75d22b1d3eae4561c093ebfed006c728885
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39944481"
---
# <a name="summarizedeviceperformancedevices-function"></a><span data-ttu-id="21dbb-103">função summarizeDevicePerformanceDevices</span><span class="sxs-lookup"><span data-stu-id="21dbb-103">summarizeDevicePerformanceDevices function</span></span>

> <span data-ttu-id="21dbb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="21dbb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21dbb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="21dbb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21dbb-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="21dbb-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="21dbb-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="21dbb-107">Prerequisites</span></span>
<span data-ttu-id="21dbb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="21dbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21dbb-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="21dbb-110">Permission type</span></span>|<span data-ttu-id="21dbb-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="21dbb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="21dbb-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="21dbb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="21dbb-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="21dbb-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="21dbb-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="21dbb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="21dbb-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="21dbb-115">Not supported.</span></span>|
|<span data-ttu-id="21dbb-116">Application</span><span class="sxs-lookup"><span data-stu-id="21dbb-116">Application</span></span>|<span data-ttu-id="21dbb-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="21dbb-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="21dbb-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="21dbb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices
```

## <a name="request-headers"></a><span data-ttu-id="21dbb-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21dbb-119">Request headers</span></span>
|<span data-ttu-id="21dbb-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="21dbb-120">Header</span></span>|<span data-ttu-id="21dbb-121">Valor</span><span class="sxs-lookup"><span data-stu-id="21dbb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="21dbb-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="21dbb-122">Authorization</span></span>|<span data-ttu-id="21dbb-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="21dbb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="21dbb-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="21dbb-124">Accept</span></span>|<span data-ttu-id="21dbb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="21dbb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="21dbb-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="21dbb-126">Request body</span></span>
<span data-ttu-id="21dbb-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="21dbb-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="21dbb-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="21dbb-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="21dbb-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21dbb-129">Property</span></span>|<span data-ttu-id="21dbb-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="21dbb-130">Type</span></span>|<span data-ttu-id="21dbb-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="21dbb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21dbb-132">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="21dbb-132">summarizeBy</span></span>|[<span data-ttu-id="21dbb-133">userExperienceAnalyticsSummarizedBy</span><span class="sxs-lookup"><span data-stu-id="21dbb-133">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="21dbb-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="21dbb-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="21dbb-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="21dbb-135">Response</span></span>
<span data-ttu-id="21dbb-136">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="21dbb-136">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21dbb-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="21dbb-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="21dbb-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="21dbb-138">Request</span></span>
<span data-ttu-id="21dbb-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="21dbb-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="21dbb-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="21dbb-140">Response</span></span>
<span data-ttu-id="21dbb-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="21dbb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 636

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsDevicePerformance",
      "id": "852ae826-e826-852a-26e8-2a8526e82a85",
      "deviceName": "Device Name value",
      "model": "Model value",
      "manufacturer": "Manufacturer value",
      "diskType": "hdd",
      "operatingSystemVersion": "Operating System Version value",
      "bootScore": 9,
      "coreBootTimeInMs": 0,
      "groupPolicyBootTimeInMs": 7,
      "healthStatus": "insufficientData",
      "loginScore": 10,
      "coreLoginTimeInMs": 1,
      "groupPolicyLoginTimeInMs": 8,
      "deviceCount": 11
    }
  ]
}
```





