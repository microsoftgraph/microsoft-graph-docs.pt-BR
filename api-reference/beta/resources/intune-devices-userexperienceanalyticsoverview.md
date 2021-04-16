---
title: Tipo de recurso userExperienceAnalyticsOverview
description: A entidade de visão geral da análise de experiência do usuário contém a pontuação geral e as pontuações e percepções de cada métrica de todas as categorias.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 32466ea9fa14efe0c46b812ac1f6babc9ba32102
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866549"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="45ac0-103">Tipo de recurso userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="45ac0-103">userExperienceAnalyticsOverview resource type</span></span>

<span data-ttu-id="45ac0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45ac0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45ac0-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45ac0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45ac0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45ac0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45ac0-107">A entidade de visão geral da análise de experiência do usuário contém a pontuação geral e as pontuações e percepções de cada métrica de todas as categorias.</span><span class="sxs-lookup"><span data-stu-id="45ac0-107">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="45ac0-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="45ac0-108">Methods</span></span>
|<span data-ttu-id="45ac0-109">Método</span><span class="sxs-lookup"><span data-stu-id="45ac0-109">Method</span></span>|<span data-ttu-id="45ac0-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="45ac0-110">Return Type</span></span>|<span data-ttu-id="45ac0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="45ac0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="45ac0-112">Obter userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="45ac0-112">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="45ac0-113">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="45ac0-113">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="45ac0-114">Ler propriedades e relações do [objeto userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="45ac0-114">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="45ac0-115">Atualizar userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="45ac0-115">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="45ac0-116">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="45ac0-116">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="45ac0-117">Atualize as propriedades de [um objeto userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="45ac0-117">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="45ac0-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45ac0-118">Properties</span></span>
|<span data-ttu-id="45ac0-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45ac0-119">Property</span></span>|<span data-ttu-id="45ac0-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="45ac0-120">Type</span></span>|<span data-ttu-id="45ac0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="45ac0-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45ac0-122">id</span><span class="sxs-lookup"><span data-stu-id="45ac0-122">id</span></span>|<span data-ttu-id="45ac0-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45ac0-123">String</span></span>|<span data-ttu-id="45ac0-124">O identificador exclusivo da visão geral da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="45ac0-124">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="45ac0-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="45ac0-125">overallScore</span></span>|<span data-ttu-id="45ac0-126">Int32</span><span class="sxs-lookup"><span data-stu-id="45ac0-126">Int32</span></span>|<span data-ttu-id="45ac0-127">A pontuação geral da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="45ac0-127">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="45ac0-128">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="45ac0-128">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="45ac0-129">Int32</span><span class="sxs-lookup"><span data-stu-id="45ac0-129">Int32</span></span>|<span data-ttu-id="45ac0-130">A pontuação geral do desempenho geral de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="45ac0-130">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="45ac0-131">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="45ac0-131">bestPracticesOverallScore</span></span>|<span data-ttu-id="45ac0-132">Int32</span><span class="sxs-lookup"><span data-stu-id="45ac0-132">Int32</span></span>|<span data-ttu-id="45ac0-133">A pontuação geral das práticas recomendadas da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="45ac0-133">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="45ac0-134">workFromAnywhereOverallScore</span><span class="sxs-lookup"><span data-stu-id="45ac0-134">workFromAnywhereOverallScore</span></span>|<span data-ttu-id="45ac0-135">Int32</span><span class="sxs-lookup"><span data-stu-id="45ac0-135">Int32</span></span>|<span data-ttu-id="45ac0-136">A pontuação geral da análise de experiência do usuário Work From Anywhere.</span><span class="sxs-lookup"><span data-stu-id="45ac0-136">The user experience analytics Work From Anywhere overall score.</span></span>|
|<span data-ttu-id="45ac0-137">appHealthOverallScore</span><span class="sxs-lookup"><span data-stu-id="45ac0-137">appHealthOverallScore</span></span>|<span data-ttu-id="45ac0-138">Int32</span><span class="sxs-lookup"><span data-stu-id="45ac0-138">Int32</span></span>|<span data-ttu-id="45ac0-139">A pontuação geral de saúde geral do aplicativo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="45ac0-139">The user experience analytics app health overall score.</span></span>|
|<span data-ttu-id="45ac0-140">resourcePerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="45ac0-140">resourcePerformanceOverallScore</span></span>|<span data-ttu-id="45ac0-141">Int32</span><span class="sxs-lookup"><span data-stu-id="45ac0-141">Int32</span></span>|<span data-ttu-id="45ac0-142">A pontuação geral do desempenho geral do recurso de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="45ac0-142">The user experience analytics resource performance overall score.</span></span>|
|<span data-ttu-id="45ac0-143">insights</span><span class="sxs-lookup"><span data-stu-id="45ac0-143">insights</span></span>|<span data-ttu-id="45ac0-144">[Coleção userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="45ac0-144">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="45ac0-145">As percepções de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="45ac0-145">The user experience analytics insights.</span></span>|
|<span data-ttu-id="45ac0-146">state</span><span class="sxs-lookup"><span data-stu-id="45ac0-146">state</span></span>|[<span data-ttu-id="45ac0-147">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="45ac0-147">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="45ac0-148">O estado de saúde atual da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="45ac0-148">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="45ac0-149">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="45ac0-149">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="45ac0-150">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="45ac0-150">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="45ac0-151">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="45ac0-151">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="45ac0-152">O estado de saúde atual da categoria de análise de experiência do usuário 'BootPerformance'.</span><span class="sxs-lookup"><span data-stu-id="45ac0-152">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="45ac0-153">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="45ac0-153">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="45ac0-154">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="45ac0-154">bestPracticesHealthState</span></span>|[<span data-ttu-id="45ac0-155">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="45ac0-155">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="45ac0-156">O estado de saúde atual da categoria de análise de experiência do usuário "BestPractices".</span><span class="sxs-lookup"><span data-stu-id="45ac0-156">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="45ac0-157">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="45ac0-157">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="45ac0-158">workFromAnywhereHealthState</span><span class="sxs-lookup"><span data-stu-id="45ac0-158">workFromAnywhereHealthState</span></span>|[<span data-ttu-id="45ac0-159">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="45ac0-159">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="45ac0-160">O estado de saúde atual da categoria de análise de experiência do usuário 'WorkFromAnywhere'.</span><span class="sxs-lookup"><span data-stu-id="45ac0-160">The current health state of the user experience analytics 'WorkFromAnywhere' category.</span></span> <span data-ttu-id="45ac0-161">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="45ac0-161">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="45ac0-162">appHealthState</span><span class="sxs-lookup"><span data-stu-id="45ac0-162">appHealthState</span></span>|[<span data-ttu-id="45ac0-163">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="45ac0-163">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="45ac0-164">O estado de saúde atual da categoria de análise de experiência do usuário "BestPractices".</span><span class="sxs-lookup"><span data-stu-id="45ac0-164">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="45ac0-165">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="45ac0-165">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="45ac0-166">resourcePerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="45ac0-166">resourcePerformanceHealthState</span></span>|[<span data-ttu-id="45ac0-167">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="45ac0-167">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="45ac0-168">O estado de saúde atual da categoria de análise de experiência do usuário 'ResourcePerformance'.</span><span class="sxs-lookup"><span data-stu-id="45ac0-168">The current health state of the user experience analytics 'ResourcePerformance' category.</span></span> <span data-ttu-id="45ac0-169">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="45ac0-169">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45ac0-170">Relações</span><span class="sxs-lookup"><span data-stu-id="45ac0-170">Relationships</span></span>
<span data-ttu-id="45ac0-171">Nenhum</span><span class="sxs-lookup"><span data-stu-id="45ac0-171">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45ac0-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45ac0-172">JSON Representation</span></span>
<span data-ttu-id="45ac0-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="45ac0-173">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsOverview"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "String (identifier)",
  "overallScore": 1024,
  "deviceBootPerformanceOverallScore": 1024,
  "bestPracticesOverallScore": 1024,
  "workFromAnywhereOverallScore": 1024,
  "appHealthOverallScore": 1024,
  "resourcePerformanceOverallScore": 1024,
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight",
      "userExperienceAnalyticsMetricId": "String",
      "insightId": "String",
      "values": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble",
          "value": "4.2"
        }
      ],
      "severity": "String"
    }
  ],
  "state": "String",
  "deviceBootPerformanceHealthState": "String",
  "bestPracticesHealthState": "String",
  "workFromAnywhereHealthState": "String",
  "appHealthState": "String",
  "resourcePerformanceHealthState": "String"
}
```




