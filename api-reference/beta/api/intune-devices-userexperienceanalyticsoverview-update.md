---
title: Atualizar userExperienceAnalyticsOverview
description: Atualiza as propriedades de um objeto userExperienceAnalyticsOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6dcdb99b31608ce4712da2d1b8363aa09b5a5603
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49233954"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="4f421-103">Atualizar userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="4f421-103">Update userExperienceAnalyticsOverview</span></span>

<span data-ttu-id="4f421-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4f421-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4f421-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4f421-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f421-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4f421-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f421-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="4f421-107">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f421-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4f421-108">Prerequisites</span></span>
<span data-ttu-id="4f421-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4f421-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f421-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4f421-111">Permission type</span></span>|<span data-ttu-id="4f421-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4f421-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f421-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4f421-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4f421-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f421-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="4f421-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4f421-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f421-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4f421-116">Not supported.</span></span>|
|<span data-ttu-id="4f421-117">Application</span><span class="sxs-lookup"><span data-stu-id="4f421-117">Application</span></span>|<span data-ttu-id="4f421-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f421-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f421-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4f421-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="4f421-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4f421-120">Request headers</span></span>
|<span data-ttu-id="4f421-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4f421-121">Header</span></span>|<span data-ttu-id="4f421-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4f421-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f421-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4f421-123">Authorization</span></span>|<span data-ttu-id="4f421-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4f421-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f421-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4f421-125">Accept</span></span>|<span data-ttu-id="4f421-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4f421-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f421-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4f421-127">Request body</span></span>
<span data-ttu-id="4f421-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="4f421-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="4f421-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span><span class="sxs-lookup"><span data-stu-id="4f421-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="4f421-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f421-130">Property</span></span>|<span data-ttu-id="4f421-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f421-131">Type</span></span>|<span data-ttu-id="4f421-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f421-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f421-133">id</span><span class="sxs-lookup"><span data-stu-id="4f421-133">id</span></span>|<span data-ttu-id="4f421-134">String</span><span class="sxs-lookup"><span data-stu-id="4f421-134">String</span></span>|<span data-ttu-id="4f421-135">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="4f421-135">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="4f421-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="4f421-136">overallScore</span></span>|<span data-ttu-id="4f421-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4f421-137">Int32</span></span>|<span data-ttu-id="4f421-138">A pontuação geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="4f421-138">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="4f421-139">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="4f421-139">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="4f421-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4f421-140">Int32</span></span>|<span data-ttu-id="4f421-141">A pontuação geral do desempenho de inicialização do dispositivo analítico da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="4f421-141">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="4f421-142">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="4f421-142">bestPracticesOverallScore</span></span>|<span data-ttu-id="4f421-143">Int32</span><span class="sxs-lookup"><span data-stu-id="4f421-143">Int32</span></span>|<span data-ttu-id="4f421-144">A pontuação geral das práticas recomendadas de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="4f421-144">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="4f421-145">insights</span><span class="sxs-lookup"><span data-stu-id="4f421-145">insights</span></span>|<span data-ttu-id="4f421-146">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="4f421-146">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="4f421-147">A experiência do usuário do Analytics insights.</span><span class="sxs-lookup"><span data-stu-id="4f421-147">The user experience analytics insights.</span></span>|
|<span data-ttu-id="4f421-148">state</span><span class="sxs-lookup"><span data-stu-id="4f421-148">state</span></span>|[<span data-ttu-id="4f421-149">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="4f421-149">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="4f421-150">O estado de integridade atual da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="4f421-150">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="4f421-151">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="4f421-151">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="4f421-152">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="4f421-152">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="4f421-153">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="4f421-153">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="4f421-154">O estado de integridade atual da categoria "BootPerformance" da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="4f421-154">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="4f421-155">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="4f421-155">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="4f421-156">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="4f421-156">bestPracticesHealthState</span></span>|[<span data-ttu-id="4f421-157">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="4f421-157">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="4f421-158">O estado de integridade atual da categoria "BestPractices" da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="4f421-158">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="4f421-159">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="4f421-159">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="4f421-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f421-160">Response</span></span>
<span data-ttu-id="4f421-161">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4f421-161">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f421-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4f421-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f421-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4f421-163">Request</span></span>
<span data-ttu-id="4f421-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4f421-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 741

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
          "value": 1.6666666666666667
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData",
  "deviceBootPerformanceHealthState": "insufficientData",
  "bestPracticesHealthState": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="4f421-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="4f421-165">Response</span></span>
<span data-ttu-id="4f421-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4f421-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 790

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
          "value": 1.6666666666666667
        }
      ],
      "severity": "informational"
    }
  ],
  "state": "insufficientData",
  "deviceBootPerformanceHealthState": "insufficientData",
  "bestPracticesHealthState": "insufficientData"
}
```




