---
title: Atualizar userExperienceAnalyticsOverview
description: Atualizar as propriedades de um objeto userExperienceAnalyticsOverview.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 77d0107c7a1ca3255bcc87f60b3dba0ff140d133
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161233"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="239f7-103">Atualizar userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="239f7-103">Update userExperienceAnalyticsOverview</span></span>

<span data-ttu-id="239f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="239f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="239f7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="239f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="239f7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="239f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="239f7-107">Atualizar as propriedades de um [objeto userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="239f7-107">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="239f7-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="239f7-108">Prerequisites</span></span>
<span data-ttu-id="239f7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="239f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="239f7-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="239f7-111">Permission type</span></span>|<span data-ttu-id="239f7-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="239f7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="239f7-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="239f7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="239f7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="239f7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="239f7-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="239f7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="239f7-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="239f7-116">Not supported.</span></span>|
|<span data-ttu-id="239f7-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="239f7-117">Application</span></span>|<span data-ttu-id="239f7-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="239f7-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="239f7-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="239f7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="239f7-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="239f7-120">Request headers</span></span>
|<span data-ttu-id="239f7-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="239f7-121">Header</span></span>|<span data-ttu-id="239f7-122">Valor</span><span class="sxs-lookup"><span data-stu-id="239f7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="239f7-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="239f7-123">Authorization</span></span>|<span data-ttu-id="239f7-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="239f7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="239f7-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="239f7-125">Accept</span></span>|<span data-ttu-id="239f7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="239f7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="239f7-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="239f7-127">Request body</span></span>
<span data-ttu-id="239f7-128">No corpo da solicitação, fornece uma representação JSON do [objeto userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="239f7-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="239f7-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span><span class="sxs-lookup"><span data-stu-id="239f7-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="239f7-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="239f7-130">Property</span></span>|<span data-ttu-id="239f7-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="239f7-131">Type</span></span>|<span data-ttu-id="239f7-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="239f7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="239f7-133">id</span><span class="sxs-lookup"><span data-stu-id="239f7-133">id</span></span>|<span data-ttu-id="239f7-134">String</span><span class="sxs-lookup"><span data-stu-id="239f7-134">String</span></span>|<span data-ttu-id="239f7-135">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="239f7-135">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="239f7-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="239f7-136">overallScore</span></span>|<span data-ttu-id="239f7-137">Int32</span><span class="sxs-lookup"><span data-stu-id="239f7-137">Int32</span></span>|<span data-ttu-id="239f7-138">A pontuação geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="239f7-138">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="239f7-139">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="239f7-139">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="239f7-140">Int32</span><span class="sxs-lookup"><span data-stu-id="239f7-140">Int32</span></span>|<span data-ttu-id="239f7-141">A pontuação geral do desempenho de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="239f7-141">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="239f7-142">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="239f7-142">bestPracticesOverallScore</span></span>|<span data-ttu-id="239f7-143">Int32</span><span class="sxs-lookup"><span data-stu-id="239f7-143">Int32</span></span>|<span data-ttu-id="239f7-144">A pontuação geral das práticas recomendadas da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="239f7-144">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="239f7-145">appHealthOverallScore</span><span class="sxs-lookup"><span data-stu-id="239f7-145">appHealthOverallScore</span></span>|<span data-ttu-id="239f7-146">Int32</span><span class="sxs-lookup"><span data-stu-id="239f7-146">Int32</span></span>|<span data-ttu-id="239f7-147">A pontuação geral de saúde do aplicativo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="239f7-147">The user experience analytics app health overall score.</span></span>|
|<span data-ttu-id="239f7-148">insights</span><span class="sxs-lookup"><span data-stu-id="239f7-148">insights</span></span>|<span data-ttu-id="239f7-149">[Coleção userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="239f7-149">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="239f7-150">As informações de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="239f7-150">The user experience analytics insights.</span></span>|
|<span data-ttu-id="239f7-151">estado</span><span class="sxs-lookup"><span data-stu-id="239f7-151">state</span></span>|[<span data-ttu-id="239f7-152">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="239f7-152">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="239f7-153">O estado de saúde atual da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="239f7-153">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="239f7-154">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="239f7-154">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="239f7-155">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="239f7-155">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="239f7-156">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="239f7-156">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="239f7-157">O estado de saúde atual da categoria "BootPerformance" da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="239f7-157">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="239f7-158">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="239f7-158">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="239f7-159">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="239f7-159">bestPracticesHealthState</span></span>|[<span data-ttu-id="239f7-160">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="239f7-160">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="239f7-161">O estado de saúde atual da categoria "BestPratices" da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="239f7-161">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="239f7-162">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="239f7-162">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="239f7-163">appHealthState</span><span class="sxs-lookup"><span data-stu-id="239f7-163">appHealthState</span></span>|[<span data-ttu-id="239f7-164">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="239f7-164">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="239f7-165">O estado de saúde atual da categoria "BestPratices" da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="239f7-165">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="239f7-166">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="239f7-166">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="239f7-167">Resposta</span><span class="sxs-lookup"><span data-stu-id="239f7-167">Response</span></span>
<span data-ttu-id="239f7-168">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="239f7-168">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="239f7-169">Exemplo</span><span class="sxs-lookup"><span data-stu-id="239f7-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="239f7-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="239f7-170">Request</span></span>
<span data-ttu-id="239f7-171">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="239f7-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 813

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "appHealthOverallScore": 5,
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
  "appHealthState": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="239f7-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="239f7-172">Response</span></span>
<span data-ttu-id="239f7-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="239f7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 862

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "8228da2b-da2b-8228-2bda-28822bda2882",
  "overallScore": 12,
  "deviceBootPerformanceOverallScore": 1,
  "bestPracticesOverallScore": 9,
  "appHealthOverallScore": 5,
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
  "appHealthState": "insufficientData"
}
```




