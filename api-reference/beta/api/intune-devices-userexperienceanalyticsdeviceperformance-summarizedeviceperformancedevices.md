---
title: função summarizeDevicePerformanceDevices
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 10752b98e4d27c9f300c16c7b2e4a597048d7fc4
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791460"
---
# <a name="summarizedeviceperformancedevices-function"></a><span data-ttu-id="700ac-103">função summarizeDevicePerformanceDevices</span><span class="sxs-lookup"><span data-stu-id="700ac-103">summarizeDevicePerformanceDevices function</span></span>

<span data-ttu-id="700ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="700ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="700ac-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="700ac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="700ac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="700ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="700ac-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="700ac-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="700ac-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="700ac-108">Prerequisites</span></span>
<span data-ttu-id="700ac-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="700ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="700ac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="700ac-111">Permission type</span></span>|<span data-ttu-id="700ac-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="700ac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="700ac-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="700ac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="700ac-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="700ac-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="700ac-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="700ac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="700ac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="700ac-116">Not supported.</span></span>|
|<span data-ttu-id="700ac-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="700ac-117">Application</span></span>|<span data-ttu-id="700ac-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="700ac-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="700ac-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="700ac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices
```

## <a name="request-headers"></a><span data-ttu-id="700ac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="700ac-120">Request headers</span></span>
|<span data-ttu-id="700ac-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="700ac-121">Header</span></span>|<span data-ttu-id="700ac-122">Valor</span><span class="sxs-lookup"><span data-stu-id="700ac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="700ac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="700ac-123">Authorization</span></span>|<span data-ttu-id="700ac-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="700ac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="700ac-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="700ac-125">Accept</span></span>|<span data-ttu-id="700ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="700ac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="700ac-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="700ac-127">Request body</span></span>
<span data-ttu-id="700ac-128">Na URL da solicitação, forneça os seguintes parâmetros de consulta com valores.</span><span class="sxs-lookup"><span data-stu-id="700ac-128">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="700ac-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta função.</span><span class="sxs-lookup"><span data-stu-id="700ac-129">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="700ac-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="700ac-130">Property</span></span>|<span data-ttu-id="700ac-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="700ac-131">Type</span></span>|<span data-ttu-id="700ac-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="700ac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="700ac-133">summarizeBy</span><span class="sxs-lookup"><span data-stu-id="700ac-133">summarizeBy</span></span>|[<span data-ttu-id="700ac-134">userExperienceAnalyticsSummarizedBy</span><span class="sxs-lookup"><span data-stu-id="700ac-134">userExperienceAnalyticsSummarizedBy</span></span>](../resources/intune-devices-userexperienceanalyticssummarizedby.md)|<span data-ttu-id="700ac-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="700ac-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="700ac-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="700ac-136">Response</span></span>
<span data-ttu-id="700ac-137">Se tiver êxito, essa função retornará um `200 OK` código de resposta e uma coleção [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="700ac-137">If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsDevicePerformance](../resources/intune-devices-userexperienceanalyticsdeviceperformance.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="700ac-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="700ac-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="700ac-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="700ac-139">Request</span></span>
<span data-ttu-id="700ac-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="700ac-140">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices(summarizeBy='parameterValue')
```

### <a name="response"></a><span data-ttu-id="700ac-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="700ac-141">Response</span></span>
<span data-ttu-id="700ac-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="700ac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 797

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
      "responsiveDesktopTimeInMs": 9,
      "blueScreenCount": 15,
      "restartCount": 12,
      "averageBlueScreens": 6.0,
      "averageRestarts": 5.0
    }
  ]
}
```



