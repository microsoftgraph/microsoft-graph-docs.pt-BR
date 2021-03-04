---
title: Tipo de recurso userExperienceAnalyticsOverview
description: A entidade de visão geral da análise de experiência do usuário contém a pontuação geral e as pontuações e percepções de cada métrica de todas as categorias.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b63fdbd00b0a93a5a8bc3536bab7f66c35f8f155
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444466"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="a2ad2-103">Tipo de recurso userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="a2ad2-103">userExperienceAnalyticsOverview resource type</span></span>

<span data-ttu-id="a2ad2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2ad2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2ad2-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2ad2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2ad2-107">A entidade de visão geral da análise de experiência do usuário contém a pontuação geral e as pontuações e percepções de cada métrica de todas as categorias.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-107">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="a2ad2-108">Methods</span><span class="sxs-lookup"><span data-stu-id="a2ad2-108">Methods</span></span>
|<span data-ttu-id="a2ad2-109">Método</span><span class="sxs-lookup"><span data-stu-id="a2ad2-109">Method</span></span>|<span data-ttu-id="a2ad2-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a2ad2-110">Return Type</span></span>|<span data-ttu-id="a2ad2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2ad2-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a2ad2-112">Obter userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="a2ad2-112">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="a2ad2-113">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="a2ad2-113">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="a2ad2-114">Ler propriedades e relações do [objeto userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="a2ad2-114">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="a2ad2-115">Atualizar userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="a2ad2-115">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="a2ad2-116">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="a2ad2-116">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="a2ad2-117">Atualize as propriedades de [um objeto userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="a2ad2-117">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a2ad2-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a2ad2-118">Properties</span></span>
|<span data-ttu-id="a2ad2-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2ad2-119">Property</span></span>|<span data-ttu-id="a2ad2-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2ad2-120">Type</span></span>|<span data-ttu-id="a2ad2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2ad2-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2ad2-122">id</span><span class="sxs-lookup"><span data-stu-id="a2ad2-122">id</span></span>|<span data-ttu-id="a2ad2-123">String</span><span class="sxs-lookup"><span data-stu-id="a2ad2-123">String</span></span>|<span data-ttu-id="a2ad2-124">O identificador exclusivo da visão geral da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-124">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="a2ad2-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="a2ad2-125">overallScore</span></span>|<span data-ttu-id="a2ad2-126">Int32</span><span class="sxs-lookup"><span data-stu-id="a2ad2-126">Int32</span></span>|<span data-ttu-id="a2ad2-127">A pontuação geral da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-127">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="a2ad2-128">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="a2ad2-128">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="a2ad2-129">Int32</span><span class="sxs-lookup"><span data-stu-id="a2ad2-129">Int32</span></span>|<span data-ttu-id="a2ad2-130">A pontuação geral do desempenho geral de inicialização do dispositivo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-130">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="a2ad2-131">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="a2ad2-131">bestPracticesOverallScore</span></span>|<span data-ttu-id="a2ad2-132">Int32</span><span class="sxs-lookup"><span data-stu-id="a2ad2-132">Int32</span></span>|<span data-ttu-id="a2ad2-133">A pontuação geral das práticas recomendadas da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-133">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="a2ad2-134">appHealthOverallScore</span><span class="sxs-lookup"><span data-stu-id="a2ad2-134">appHealthOverallScore</span></span>|<span data-ttu-id="a2ad2-135">Int32</span><span class="sxs-lookup"><span data-stu-id="a2ad2-135">Int32</span></span>|<span data-ttu-id="a2ad2-136">A pontuação geral de saúde geral do aplicativo de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-136">The user experience analytics app health overall score.</span></span>|
|<span data-ttu-id="a2ad2-137">resourcePerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="a2ad2-137">resourcePerformanceOverallScore</span></span>|<span data-ttu-id="a2ad2-138">Int32</span><span class="sxs-lookup"><span data-stu-id="a2ad2-138">Int32</span></span>|<span data-ttu-id="a2ad2-139">A pontuação geral do desempenho geral do recurso de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-139">The user experience analytics resource performance overall score.</span></span>|
|<span data-ttu-id="a2ad2-140">insights</span><span class="sxs-lookup"><span data-stu-id="a2ad2-140">insights</span></span>|<span data-ttu-id="a2ad2-141">[Coleção userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="a2ad2-141">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="a2ad2-142">As percepções de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-142">The user experience analytics insights.</span></span>|
|<span data-ttu-id="a2ad2-143">state</span><span class="sxs-lookup"><span data-stu-id="a2ad2-143">state</span></span>|[<span data-ttu-id="a2ad2-144">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="a2ad2-144">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="a2ad2-145">O estado de saúde atual da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-145">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="a2ad2-146">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-146">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="a2ad2-147">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="a2ad2-147">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="a2ad2-148">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="a2ad2-148">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="a2ad2-149">O estado de saúde atual da categoria de análise de experiência do usuário 'BootPerformance'.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-149">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="a2ad2-150">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-150">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="a2ad2-151">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="a2ad2-151">bestPracticesHealthState</span></span>|[<span data-ttu-id="a2ad2-152">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="a2ad2-152">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="a2ad2-153">O estado de saúde atual da categoria de análise de experiência do usuário "BestPractices".</span><span class="sxs-lookup"><span data-stu-id="a2ad2-153">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="a2ad2-154">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-154">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="a2ad2-155">appHealthState</span><span class="sxs-lookup"><span data-stu-id="a2ad2-155">appHealthState</span></span>|[<span data-ttu-id="a2ad2-156">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="a2ad2-156">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="a2ad2-157">O estado de saúde atual da categoria de análise de experiência do usuário "BestPractices".</span><span class="sxs-lookup"><span data-stu-id="a2ad2-157">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="a2ad2-158">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-158">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="a2ad2-159">resourcePerformanceState</span><span class="sxs-lookup"><span data-stu-id="a2ad2-159">resourcePerformanceState</span></span>|[<span data-ttu-id="a2ad2-160">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="a2ad2-160">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="a2ad2-161">O estado de saúde atual da categoria de análise de experiência do usuário 'ResourcePerformance'.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-161">The current health state of the user experience analytics 'ResourcePerformance' category.</span></span> <span data-ttu-id="a2ad2-162">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-162">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2ad2-163">Relações</span><span class="sxs-lookup"><span data-stu-id="a2ad2-163">Relationships</span></span>
<span data-ttu-id="a2ad2-164">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a2ad2-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2ad2-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a2ad2-165">JSON Representation</span></span>
<span data-ttu-id="a2ad2-166">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a2ad2-166">Here is a JSON representation of the resource.</span></span>
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
  "appHealthState": "String",
  "resourcePerformanceState": "String"
}
```




