---
title: função summarizeDevicePerformanceDevices
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 00e6210ed2eb10ee79289451624159bba8769000
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813962"
---
# <a name="summarizedeviceperformancedevices-function"></a><span data-ttu-id="81962-103">função summarizeDevicePerformanceDevices</span><span class="sxs-lookup"><span data-stu-id="81962-103">summarizeDevicePerformanceDevices function</span></span>

> <span data-ttu-id="81962-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81962-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81962-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81962-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81962-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="81962-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81962-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81962-107">Prerequisites</span></span>
<span data-ttu-id="81962-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81962-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81962-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81962-110">Permission type</span></span>|<span data-ttu-id="81962-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="81962-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81962-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81962-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81962-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="81962-113">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="81962-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81962-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81962-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81962-115">Not supported.</span></span>|
|<span data-ttu-id="81962-116">Application</span><span class="sxs-lookup"><span data-stu-id="81962-116">Application</span></span>|<span data-ttu-id="81962-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="81962-117">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81962-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81962-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices
```

## <a name="request-headers"></a><span data-ttu-id="81962-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81962-119">Request headers</span></span>
|<span data-ttu-id="81962-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81962-120">Header</span></span>|<span data-ttu-id="81962-121">Valor</span><span class="sxs-lookup"><span data-stu-id="81962-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81962-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="81962-122">Authorization</span></span>|<span data-ttu-id="81962-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81962-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81962-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="81962-124">Accept</span></span>|<span data-ttu-id="81962-125">application/json</span><span class="sxs-lookup"><span data-stu-id="81962-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81962-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81962-126">Request body</span></span>
<span data-ttu-id="81962-127">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="81962-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="81962-128">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="81962-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="81962-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="81962-129">Property</span></span>|<span data-ttu-id="81962-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="81962-130">Type</span></span>|<span data-ttu-id="81962-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="81962-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81962-132">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="81962-132">summarizeBy</span></span>|[<span data-ttu-id="81962-133">userExperienceAnalyticsSummarizedBy</span><span class="sxs-lookup"><span data-stu-id="81962-133">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="81962-134">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="81962-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="81962-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="81962-135">Response</span></span>
<span data-ttu-id="81962-136">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81962-136">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81962-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81962-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="81962-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81962-138">Request</span></span>
<span data-ttu-id="81962-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81962-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="81962-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="81962-140">Response</span></span>
<span data-ttu-id="81962-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81962-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

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
      "deviceCount": 11,
      "responsiveDesktopTimeInMs": 9
    }
  ]
}
```




