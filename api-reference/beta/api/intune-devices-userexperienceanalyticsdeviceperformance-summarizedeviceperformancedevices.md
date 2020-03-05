---
title: função summarizeDevicePerformanceDevices
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3c66c72a27296c3b28460874899e7a0b78bde760
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42468394"
---
# <a name="summarizedeviceperformancedevices-function"></a><span data-ttu-id="92647-103">função summarizeDevicePerformanceDevices</span><span class="sxs-lookup"><span data-stu-id="92647-103">summarizeDevicePerformanceDevices function</span></span>

<span data-ttu-id="92647-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="92647-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92647-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="92647-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92647-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="92647-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92647-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="92647-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92647-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="92647-108">Prerequisites</span></span>
<span data-ttu-id="92647-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="92647-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92647-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="92647-111">Permission type</span></span>|<span data-ttu-id="92647-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="92647-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92647-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="92647-113">Delegated (work or school account)</span></span>|<span data-ttu-id="92647-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="92647-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="92647-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="92647-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92647-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="92647-116">Not supported.</span></span>|
|<span data-ttu-id="92647-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="92647-117">Application</span></span>|<span data-ttu-id="92647-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="92647-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="92647-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="92647-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices
```

## <a name="request-headers"></a><span data-ttu-id="92647-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="92647-120">Request headers</span></span>
|<span data-ttu-id="92647-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="92647-121">Header</span></span>|<span data-ttu-id="92647-122">Valor</span><span class="sxs-lookup"><span data-stu-id="92647-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92647-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="92647-123">Authorization</span></span>|<span data-ttu-id="92647-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="92647-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92647-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="92647-125">Accept</span></span>|<span data-ttu-id="92647-126">application/json</span><span class="sxs-lookup"><span data-stu-id="92647-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92647-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="92647-127">Request body</span></span>
<span data-ttu-id="92647-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="92647-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="92647-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="92647-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="92647-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="92647-130">Property</span></span>|<span data-ttu-id="92647-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="92647-131">Type</span></span>|<span data-ttu-id="92647-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="92647-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92647-133">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="92647-133">summarizeBy</span></span>|[<span data-ttu-id="92647-134">userExperienceAnalyticsSummarizedBy</span><span class="sxs-lookup"><span data-stu-id="92647-134">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="92647-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="92647-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="92647-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="92647-136">Response</span></span>
<span data-ttu-id="92647-137">Se tiver êxito, essa função retornará `200 OK` um código de resposta e uma coleção [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="92647-137">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92647-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="92647-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="92647-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="92647-139">Request</span></span>
<span data-ttu-id="92647-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="92647-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="92647-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="92647-141">Response</span></span>
<span data-ttu-id="92647-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="92647-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





