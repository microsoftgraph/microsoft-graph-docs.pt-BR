---
title: Atualizar userExperienceAnalyticsOverview
description: Atualize as propriedades de um objeto userExperienceAnalyticsOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02383cd8ac10d7c383b3cd84c25d4dc57c9bd71b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434962"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="2e971-103">Atualizar userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="2e971-103">Update userExperienceAnalyticsOverview</span></span>

<span data-ttu-id="2e971-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e971-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2e971-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2e971-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2e971-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2e971-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2e971-107">Atualize as propriedades de [um objeto userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="2e971-107">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2e971-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2e971-108">Prerequisites</span></span>
<span data-ttu-id="2e971-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e971-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e971-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e971-111">Permission type</span></span>|<span data-ttu-id="2e971-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2e971-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e971-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e971-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2e971-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e971-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2e971-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e971-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e971-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e971-116">Not supported.</span></span>|
|<span data-ttu-id="2e971-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e971-117">Application</span></span>|<span data-ttu-id="2e971-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e971-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e971-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e971-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="2e971-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e971-120">Request headers</span></span>
|<span data-ttu-id="2e971-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2e971-121">Header</span></span>|<span data-ttu-id="2e971-122">Valor</span><span class="sxs-lookup"><span data-stu-id="2e971-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e971-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e971-123">Authorization</span></span>|<span data-ttu-id="2e971-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e971-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e971-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2e971-125">Accept</span></span>|<span data-ttu-id="2e971-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2e971-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e971-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e971-127">Request body</span></span>
<span data-ttu-id="2e971-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="2e971-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="2e971-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span><span class="sxs-lookup"><span data-stu-id="2e971-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="2e971-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2e971-130">Property</span></span>|<span data-ttu-id="2e971-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e971-131">Type</span></span>|<span data-ttu-id="2e971-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e971-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e971-133">id</span><span class="sxs-lookup"><span data-stu-id="2e971-133">id</span></span>|<span data-ttu-id="2e971-134">String</span><span class="sxs-lookup"><span data-stu-id="2e971-134">String</span></span>|<span data-ttu-id="2e971-135">O identificador exclusivo da visão geral da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="2e971-135">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="2e971-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="2e971-136">overallScore</span></span>|<span data-ttu-id="2e971-137">Int32</span><span class="sxs-lookup"><span data-stu-id="2e971-137">Int32</span></span>|<span data-ttu-id="2e971-138">A pontuação geral da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="2e971-138">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="2e971-139">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="2e971-139">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="2e971-140">Int32</span><span class="sxs-lookup"><span data-stu-id="2e971-140">Int32</span></span>|<span data-ttu-id="2e971-141">A pontuação geral do desempenho geral de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="2e971-141">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="2e971-142">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="2e971-142">bestPracticesOverallScore</span></span>|<span data-ttu-id="2e971-143">Int32</span><span class="sxs-lookup"><span data-stu-id="2e971-143">Int32</span></span>|<span data-ttu-id="2e971-144">A pontuação geral das práticas recomendadas da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="2e971-144">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="2e971-145">appHealthOverallScore</span><span class="sxs-lookup"><span data-stu-id="2e971-145">appHealthOverallScore</span></span>|<span data-ttu-id="2e971-146">Int32</span><span class="sxs-lookup"><span data-stu-id="2e971-146">Int32</span></span>|<span data-ttu-id="2e971-147">A pontuação geral de saúde geral do aplicativo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="2e971-147">The user experience analytics app health overall score.</span></span>|
|<span data-ttu-id="2e971-148">resourcePerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="2e971-148">resourcePerformanceOverallScore</span></span>|<span data-ttu-id="2e971-149">Int32</span><span class="sxs-lookup"><span data-stu-id="2e971-149">Int32</span></span>|<span data-ttu-id="2e971-150">A pontuação geral do desempenho geral do recurso de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="2e971-150">The user experience analytics resource performance overall score.</span></span>|
|<span data-ttu-id="2e971-151">insights</span><span class="sxs-lookup"><span data-stu-id="2e971-151">insights</span></span>|<span data-ttu-id="2e971-152">[Coleção userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="2e971-152">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="2e971-153">As percepções de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="2e971-153">The user experience analytics insights.</span></span>|
|<span data-ttu-id="2e971-154">state</span><span class="sxs-lookup"><span data-stu-id="2e971-154">state</span></span>|[<span data-ttu-id="2e971-155">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="2e971-155">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="2e971-156">O estado de saúde atual da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="2e971-156">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="2e971-157">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="2e971-157">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="2e971-158">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="2e971-158">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="2e971-159">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="2e971-159">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="2e971-160">O estado de saúde atual da categoria de análise de experiência do usuário 'BootPerformance'.</span><span class="sxs-lookup"><span data-stu-id="2e971-160">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="2e971-161">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="2e971-161">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="2e971-162">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="2e971-162">bestPracticesHealthState</span></span>|[<span data-ttu-id="2e971-163">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="2e971-163">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="2e971-164">O estado de saúde atual da categoria de análise de experiência do usuário "BestPractices".</span><span class="sxs-lookup"><span data-stu-id="2e971-164">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="2e971-165">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="2e971-165">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="2e971-166">appHealthState</span><span class="sxs-lookup"><span data-stu-id="2e971-166">appHealthState</span></span>|[<span data-ttu-id="2e971-167">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="2e971-167">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="2e971-168">O estado de saúde atual da categoria de análise de experiência do usuário "BestPractices".</span><span class="sxs-lookup"><span data-stu-id="2e971-168">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="2e971-169">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="2e971-169">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="2e971-170">resourcePerformanceState</span><span class="sxs-lookup"><span data-stu-id="2e971-170">resourcePerformanceState</span></span>|[<span data-ttu-id="2e971-171">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="2e971-171">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="2e971-172">O estado de saúde atual da categoria de análise de experiência do usuário 'ResourcePerformance'.</span><span class="sxs-lookup"><span data-stu-id="2e971-172">The current health state of the user experience analytics 'ResourcePerformance' category.</span></span> <span data-ttu-id="2e971-173">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="2e971-173">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="2e971-174">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e971-174">Response</span></span>
<span data-ttu-id="2e971-175">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e971-175">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e971-176">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2e971-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="2e971-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e971-177">Request</span></span>
<span data-ttu-id="2e971-178">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e971-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 906

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "appHealthOverallScore": 5,
  "resourcePerformanceOverallScore": 15,
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
  "bestPracticesHealthState": "insufficientData",
  "appHealthState": "insufficientData",
  "resourcePerformanceState": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="2e971-179">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e971-179">Response</span></span>
<span data-ttu-id="2e971-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e971-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 955

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "8228da2b-da2b-8228-2bda-28822bda2882",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "appHealthOverallScore": 5,
  "resourcePerformanceOverallScore": 15,
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
  "bestPracticesHealthState": "insufficientData",
  "appHealthState": "insufficientData",
  "resourcePerformanceState": "insufficientData"
}
```




