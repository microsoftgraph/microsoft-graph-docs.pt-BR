---
title: Atualizar userExperienceAnalyticsOverview
description: Atualiza as propriedades de um objeto userExperienceAnalyticsOverview.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5e90382c1a4e50aa7f880d836c592662c94ce587
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37180080"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="a2c6b-103">Atualizar userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="a2c6b-103">Update userExperienceAnalyticsOverview</span></span>

> <span data-ttu-id="a2c6b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a2c6b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2c6b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2c6b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2c6b-106">Atualiza as propriedades de um objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="a2c6b-106">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2c6b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a2c6b-107">Prerequisites</span></span>
<span data-ttu-id="a2c6b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2c6b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2c6b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2c6b-110">Permission type</span></span>|<span data-ttu-id="a2c6b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a2c6b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2c6b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2c6b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2c6b-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2c6b-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="a2c6b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2c6b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2c6b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2c6b-115">Not supported.</span></span>|
|<span data-ttu-id="a2c6b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2c6b-116">Application</span></span>|<span data-ttu-id="a2c6b-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2c6b-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2c6b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2c6b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="a2c6b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2c6b-119">Request headers</span></span>
|<span data-ttu-id="a2c6b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a2c6b-120">Header</span></span>|<span data-ttu-id="a2c6b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a2c6b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2c6b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2c6b-122">Authorization</span></span>|<span data-ttu-id="a2c6b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2c6b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2c6b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a2c6b-124">Accept</span></span>|<span data-ttu-id="a2c6b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2c6b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2c6b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2c6b-126">Request body</span></span>
<span data-ttu-id="a2c6b-127">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="a2c6b-127">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="a2c6b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span><span class="sxs-lookup"><span data-stu-id="a2c6b-128">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="a2c6b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2c6b-129">Property</span></span>|<span data-ttu-id="a2c6b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2c6b-130">Type</span></span>|<span data-ttu-id="a2c6b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2c6b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2c6b-132">id</span><span class="sxs-lookup"><span data-stu-id="a2c6b-132">id</span></span>|<span data-ttu-id="a2c6b-133">String</span><span class="sxs-lookup"><span data-stu-id="a2c6b-133">String</span></span>|<span data-ttu-id="a2c6b-134">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a2c6b-134">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="a2c6b-135">overallScore</span><span class="sxs-lookup"><span data-stu-id="a2c6b-135">overallScore</span></span>|<span data-ttu-id="a2c6b-136">Int32</span><span class="sxs-lookup"><span data-stu-id="a2c6b-136">Int32</span></span>|<span data-ttu-id="a2c6b-137">A pontuação geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a2c6b-137">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="a2c6b-138">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="a2c6b-138">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="a2c6b-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a2c6b-139">Int32</span></span>|<span data-ttu-id="a2c6b-140">A pontuação geral do desempenho de inicialização do dispositivo analítico da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a2c6b-140">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="a2c6b-141">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="a2c6b-141">bestPracticesOverallScore</span></span>|<span data-ttu-id="a2c6b-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a2c6b-142">Int32</span></span>|<span data-ttu-id="a2c6b-143">A pontuação geral das práticas recomendadas de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a2c6b-143">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="a2c6b-144">insights</span><span class="sxs-lookup"><span data-stu-id="a2c6b-144">insights</span></span>|<span data-ttu-id="a2c6b-145">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="a2c6b-145">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="a2c6b-146">A experiência do usuário do Analytics insights.</span><span class="sxs-lookup"><span data-stu-id="a2c6b-146">The user experience analytics insights.</span></span>|
|<span data-ttu-id="a2c6b-147">estado</span><span class="sxs-lookup"><span data-stu-id="a2c6b-147">state</span></span>|[<span data-ttu-id="a2c6b-148">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="a2c6b-148">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="a2c6b-149">O estado de integridade atual da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a2c6b-149">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="a2c6b-150">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="a2c6b-150">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="a2c6b-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2c6b-151">Response</span></span>
<span data-ttu-id="a2c6b-152">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2c6b-152">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2c6b-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2c6b-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2c6b-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2c6b-154">Request</span></span>
<span data-ttu-id="a2c6b-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2c6b-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 650

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": "<Unknown Primitive Type Edm.Double>"
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="a2c6b-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2c6b-156">Response</span></span>
<span data-ttu-id="a2c6b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2c6b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 699

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "8228da2b-da2b-8228-2bda-28822bda2882",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "User Experience Analytics Metric Id value",
      "insightId": "Insight Id value",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": "<Unknown Primitive Type Edm.Double>"
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData"
}
```




