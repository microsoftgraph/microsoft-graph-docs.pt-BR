---
title: Atualizar userExperienceAnalyticsOverview
description: Atualize as propriedades de um objeto userExperienceAnalyticsOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dbe91b8e131e4379c8d658cea6420aad9fbf2c9e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149972"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="8742e-103">Atualizar userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="8742e-103">Update userExperienceAnalyticsOverview</span></span>

<span data-ttu-id="8742e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8742e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8742e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8742e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8742e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8742e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8742e-107">Atualize as propriedades de [um objeto userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="8742e-107">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8742e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8742e-108">Prerequisites</span></span>
<span data-ttu-id="8742e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8742e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8742e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8742e-111">Permission type</span></span>|<span data-ttu-id="8742e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8742e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8742e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8742e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8742e-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8742e-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8742e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8742e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8742e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8742e-116">Not supported.</span></span>|
|<span data-ttu-id="8742e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8742e-117">Application</span></span>|<span data-ttu-id="8742e-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8742e-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8742e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8742e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="8742e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8742e-120">Request headers</span></span>
|<span data-ttu-id="8742e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8742e-121">Header</span></span>|<span data-ttu-id="8742e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8742e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8742e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8742e-123">Authorization</span></span>|<span data-ttu-id="8742e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8742e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8742e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8742e-125">Accept</span></span>|<span data-ttu-id="8742e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8742e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8742e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8742e-127">Request body</span></span>
<span data-ttu-id="8742e-128">No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="8742e-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="8742e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span><span class="sxs-lookup"><span data-stu-id="8742e-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="8742e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8742e-130">Property</span></span>|<span data-ttu-id="8742e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8742e-131">Type</span></span>|<span data-ttu-id="8742e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8742e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8742e-133">id</span><span class="sxs-lookup"><span data-stu-id="8742e-133">id</span></span>|<span data-ttu-id="8742e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8742e-134">String</span></span>|<span data-ttu-id="8742e-135">O identificador exclusivo da visão geral da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8742e-135">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="8742e-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="8742e-136">overallScore</span></span>|<span data-ttu-id="8742e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8742e-137">Int32</span></span>|<span data-ttu-id="8742e-138">A pontuação geral da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8742e-138">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="8742e-139">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="8742e-139">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="8742e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="8742e-140">Int32</span></span>|<span data-ttu-id="8742e-141">A pontuação geral do desempenho geral de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8742e-141">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="8742e-142">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="8742e-142">bestPracticesOverallScore</span></span>|<span data-ttu-id="8742e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="8742e-143">Int32</span></span>|<span data-ttu-id="8742e-144">A pontuação geral das práticas recomendadas da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8742e-144">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="8742e-145">workFromAnywhereOverallScore</span><span class="sxs-lookup"><span data-stu-id="8742e-145">workFromAnywhereOverallScore</span></span>|<span data-ttu-id="8742e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="8742e-146">Int32</span></span>|<span data-ttu-id="8742e-147">A pontuação geral da análise de experiência do usuário Work From Anywhere.</span><span class="sxs-lookup"><span data-stu-id="8742e-147">The user experience analytics Work From Anywhere overall score.</span></span>|
|<span data-ttu-id="8742e-148">appHealthOverallScore</span><span class="sxs-lookup"><span data-stu-id="8742e-148">appHealthOverallScore</span></span>|<span data-ttu-id="8742e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="8742e-149">Int32</span></span>|<span data-ttu-id="8742e-150">A pontuação geral de saúde geral do aplicativo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8742e-150">The user experience analytics app health overall score.</span></span>|
|<span data-ttu-id="8742e-151">resourcePerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="8742e-151">resourcePerformanceOverallScore</span></span>|<span data-ttu-id="8742e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8742e-152">Int32</span></span>|<span data-ttu-id="8742e-153">A pontuação geral do desempenho geral do recurso de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8742e-153">The user experience analytics resource performance overall score.</span></span>|
|<span data-ttu-id="8742e-154">insights</span><span class="sxs-lookup"><span data-stu-id="8742e-154">insights</span></span>|<span data-ttu-id="8742e-155">[Coleção userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="8742e-155">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="8742e-156">As percepções de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8742e-156">The user experience analytics insights.</span></span>|
|<span data-ttu-id="8742e-157">state</span><span class="sxs-lookup"><span data-stu-id="8742e-157">state</span></span>|[<span data-ttu-id="8742e-158">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="8742e-158">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="8742e-159">O estado de saúde atual da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8742e-159">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="8742e-160">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="8742e-160">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="8742e-161">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="8742e-161">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="8742e-162">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="8742e-162">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="8742e-163">O estado de saúde atual da categoria de análise de experiência do usuário 'BootPerformance'.</span><span class="sxs-lookup"><span data-stu-id="8742e-163">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="8742e-164">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="8742e-164">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="8742e-165">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="8742e-165">bestPracticesHealthState</span></span>|[<span data-ttu-id="8742e-166">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="8742e-166">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="8742e-167">O estado de saúde atual da categoria de análise de experiência do usuário "BestPractices".</span><span class="sxs-lookup"><span data-stu-id="8742e-167">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="8742e-168">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="8742e-168">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="8742e-169">workFromAnywhereHealthState</span><span class="sxs-lookup"><span data-stu-id="8742e-169">workFromAnywhereHealthState</span></span>|[<span data-ttu-id="8742e-170">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="8742e-170">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="8742e-171">O estado de saúde atual da categoria de análise de experiência do usuário 'WorkFromAnywhere'.</span><span class="sxs-lookup"><span data-stu-id="8742e-171">The current health state of the user experience analytics 'WorkFromAnywhere' category.</span></span> <span data-ttu-id="8742e-172">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="8742e-172">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="8742e-173">appHealthState</span><span class="sxs-lookup"><span data-stu-id="8742e-173">appHealthState</span></span>|[<span data-ttu-id="8742e-174">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="8742e-174">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="8742e-175">O estado de saúde atual da categoria de análise de experiência do usuário "BestPractices".</span><span class="sxs-lookup"><span data-stu-id="8742e-175">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="8742e-176">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="8742e-176">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="8742e-177">resourcePerformanceState</span><span class="sxs-lookup"><span data-stu-id="8742e-177">resourcePerformanceState</span></span>|[<span data-ttu-id="8742e-178">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="8742e-178">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="8742e-179">O estado de saúde atual da categoria de análise de experiência do usuário 'ResourcePerformance'.</span><span class="sxs-lookup"><span data-stu-id="8742e-179">The current health state of the user experience analytics 'ResourcePerformance' category.</span></span> <span data-ttu-id="8742e-180">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="8742e-180">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="8742e-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="8742e-181">Response</span></span>
<span data-ttu-id="8742e-182">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8742e-182">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8742e-183">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8742e-183">Example</span></span>

### <a name="request"></a><span data-ttu-id="8742e-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8742e-184">Request</span></span>
<span data-ttu-id="8742e-185">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8742e-185">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 999

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "workFromAnywhereOverallScore": 12,
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
  "workFromAnywhereHealthState": "insufficientData",
  "appHealthState": "insufficientData",
  "resourcePerformanceState": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="8742e-186">Resposta</span><span class="sxs-lookup"><span data-stu-id="8742e-186">Response</span></span>
<span data-ttu-id="8742e-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8742e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1048

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "8228da2b-da2b-8228-2bda-28822bda2882",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "workFromAnywhereOverallScore": 12,
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
  "workFromAnywhereHealthState": "insufficientData",
  "appHealthState": "insufficientData",
  "resourcePerformanceState": "insufficientData"
}
```




