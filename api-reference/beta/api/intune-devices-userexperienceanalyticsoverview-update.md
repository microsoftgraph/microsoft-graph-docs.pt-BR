---
title: Atualizar userExperienceAnalyticsOverview
description: Atualiza as propriedades de um objeto userExperienceAnalyticsOverview.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3ab0d189772159ceec940d4434611621cff7bcfb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43379135"
---
# <a name="update-userexperienceanalyticsoverview"></a><span data-ttu-id="ac284-103">Atualizar userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="ac284-103">Update userExperienceAnalyticsOverview</span></span>

<span data-ttu-id="ac284-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac284-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ac284-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ac284-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac284-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ac284-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac284-107">Atualiza as propriedades de um objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="ac284-107">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac284-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ac284-108">Prerequisites</span></span>
<span data-ttu-id="ac284-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac284-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac284-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac284-111">Permission type</span></span>|<span data-ttu-id="ac284-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ac284-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac284-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac284-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ac284-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac284-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ac284-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac284-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac284-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac284-116">Not supported.</span></span>|
|<span data-ttu-id="ac284-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac284-117">Application</span></span>|<span data-ttu-id="ac284-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac284-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac284-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac284-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsOverview
```

## <a name="request-headers"></a><span data-ttu-id="ac284-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac284-120">Request headers</span></span>
|<span data-ttu-id="ac284-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ac284-121">Header</span></span>|<span data-ttu-id="ac284-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ac284-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac284-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac284-123">Authorization</span></span>|<span data-ttu-id="ac284-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac284-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac284-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ac284-125">Accept</span></span>|<span data-ttu-id="ac284-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ac284-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac284-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac284-127">Request body</span></span>
<span data-ttu-id="ac284-128">No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="ac284-128">In the request body, supply a JSON representation for the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>

<span data-ttu-id="ac284-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span><span class="sxs-lookup"><span data-stu-id="ac284-129">The following table shows the properties that are required when you create the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md).</span></span>

|<span data-ttu-id="ac284-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac284-130">Property</span></span>|<span data-ttu-id="ac284-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac284-131">Type</span></span>|<span data-ttu-id="ac284-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac284-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac284-133">id</span><span class="sxs-lookup"><span data-stu-id="ac284-133">id</span></span>|<span data-ttu-id="ac284-134">String</span><span class="sxs-lookup"><span data-stu-id="ac284-134">String</span></span>|<span data-ttu-id="ac284-135">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ac284-135">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="ac284-136">overallScore</span><span class="sxs-lookup"><span data-stu-id="ac284-136">overallScore</span></span>|<span data-ttu-id="ac284-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ac284-137">Int32</span></span>|<span data-ttu-id="ac284-138">A pontuação geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ac284-138">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="ac284-139">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="ac284-139">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="ac284-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ac284-140">Int32</span></span>|<span data-ttu-id="ac284-141">A pontuação geral do desempenho de inicialização do dispositivo analítico da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ac284-141">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="ac284-142">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="ac284-142">bestPracticesOverallScore</span></span>|<span data-ttu-id="ac284-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ac284-143">Int32</span></span>|<span data-ttu-id="ac284-144">A pontuação geral das práticas recomendadas de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ac284-144">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="ac284-145">insights</span><span class="sxs-lookup"><span data-stu-id="ac284-145">insights</span></span>|<span data-ttu-id="ac284-146">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="ac284-146">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="ac284-147">A experiência do usuário do Analytics insights.</span><span class="sxs-lookup"><span data-stu-id="ac284-147">The user experience analytics insights.</span></span>|
|<span data-ttu-id="ac284-148">state</span><span class="sxs-lookup"><span data-stu-id="ac284-148">state</span></span>|[<span data-ttu-id="ac284-149">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="ac284-149">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="ac284-150">O estado de integridade atual da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ac284-150">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="ac284-151">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="ac284-151">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="ac284-152">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="ac284-152">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="ac284-153">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="ac284-153">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="ac284-154">O estado de integridade atual da categoria "BootPerformance" da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ac284-154">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="ac284-155">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="ac284-155">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="ac284-156">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="ac284-156">bestPracticesHealthState</span></span>|[<span data-ttu-id="ac284-157">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="ac284-157">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="ac284-158">O estado de integridade atual da categoria "BestPractices" da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ac284-158">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="ac284-159">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="ac284-159">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|



## <a name="response"></a><span data-ttu-id="ac284-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac284-160">Response</span></span>
<span data-ttu-id="ac284-161">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac284-161">If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac284-162">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac284-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac284-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac284-163">Request</span></span>
<span data-ttu-id="ac284-164">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac284-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsOverview
Content-type: application/json
Content-length: 760

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
  "state": "insufficientData",
  "deviceBootPerformanceHealthState": "insufficientData",
  "bestPracticesHealthState": "insufficientData"
}
```

### <a name="response"></a><span data-ttu-id="ac284-165">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac284-165">Response</span></span>
<span data-ttu-id="ac284-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac284-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 809

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
  "state": "insufficientData",
  "deviceBootPerformanceHealthState": "insufficientData",
  "bestPracticesHealthState": "insufficientData"
}
```



