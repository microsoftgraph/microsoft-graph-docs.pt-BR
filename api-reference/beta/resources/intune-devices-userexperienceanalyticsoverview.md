---
title: Tipo de recurso userExperienceAnalyticsOverview
description: A entidade de visão geral da análise da experiência do usuário contém a pontuação geral e as pontuações e percepções de cada métrica de todas as categorias.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 655eedf3cfab990c6c83998ff7c0fd3ae78b6dff
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159546"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="28032-103">Tipo de recurso userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="28032-103">userExperienceAnalyticsOverview resource type</span></span>

<span data-ttu-id="28032-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28032-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="28032-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="28032-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28032-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="28032-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28032-107">A entidade de visão geral da análise da experiência do usuário contém a pontuação geral e as pontuações e percepções de cada métrica de todas as categorias.</span><span class="sxs-lookup"><span data-stu-id="28032-107">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="28032-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="28032-108">Methods</span></span>
|<span data-ttu-id="28032-109">Método</span><span class="sxs-lookup"><span data-stu-id="28032-109">Method</span></span>|<span data-ttu-id="28032-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="28032-110">Return Type</span></span>|<span data-ttu-id="28032-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="28032-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="28032-112">Obter userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="28032-112">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="28032-113">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="28032-113">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="28032-114">Leia as propriedades e as relações do [objeto userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="28032-114">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="28032-115">Atualizar userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="28032-115">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="28032-116">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="28032-116">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="28032-117">Atualizar as propriedades de um [objeto userExperienceAnalyticsOverview.](../resources/intune-devices-userexperienceanalyticsoverview.md)</span><span class="sxs-lookup"><span data-stu-id="28032-117">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="28032-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28032-118">Properties</span></span>
|<span data-ttu-id="28032-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28032-119">Property</span></span>|<span data-ttu-id="28032-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="28032-120">Type</span></span>|<span data-ttu-id="28032-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="28032-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28032-122">id</span><span class="sxs-lookup"><span data-stu-id="28032-122">id</span></span>|<span data-ttu-id="28032-123">String</span><span class="sxs-lookup"><span data-stu-id="28032-123">String</span></span>|<span data-ttu-id="28032-124">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="28032-124">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="28032-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="28032-125">overallScore</span></span>|<span data-ttu-id="28032-126">Int32</span><span class="sxs-lookup"><span data-stu-id="28032-126">Int32</span></span>|<span data-ttu-id="28032-127">A pontuação geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="28032-127">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="28032-128">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="28032-128">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="28032-129">Int32</span><span class="sxs-lookup"><span data-stu-id="28032-129">Int32</span></span>|<span data-ttu-id="28032-130">A pontuação geral do desempenho de inicialização do dispositivo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="28032-130">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="28032-131">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="28032-131">bestPracticesOverallScore</span></span>|<span data-ttu-id="28032-132">Int32</span><span class="sxs-lookup"><span data-stu-id="28032-132">Int32</span></span>|<span data-ttu-id="28032-133">A pontuação geral das práticas recomendadas da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="28032-133">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="28032-134">appHealthOverallScore</span><span class="sxs-lookup"><span data-stu-id="28032-134">appHealthOverallScore</span></span>|<span data-ttu-id="28032-135">Int32</span><span class="sxs-lookup"><span data-stu-id="28032-135">Int32</span></span>|<span data-ttu-id="28032-136">A pontuação geral de saúde do aplicativo de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="28032-136">The user experience analytics app health overall score.</span></span>|
|<span data-ttu-id="28032-137">insights</span><span class="sxs-lookup"><span data-stu-id="28032-137">insights</span></span>|<span data-ttu-id="28032-138">[Coleção userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="28032-138">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="28032-139">As informações de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="28032-139">The user experience analytics insights.</span></span>|
|<span data-ttu-id="28032-140">estado</span><span class="sxs-lookup"><span data-stu-id="28032-140">state</span></span>|[<span data-ttu-id="28032-141">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="28032-141">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="28032-142">O estado de saúde atual da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="28032-142">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="28032-143">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="28032-143">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="28032-144">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="28032-144">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="28032-145">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="28032-145">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="28032-146">O estado de saúde atual da categoria "BootPerformance" da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="28032-146">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="28032-147">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="28032-147">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="28032-148">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="28032-148">bestPracticesHealthState</span></span>|[<span data-ttu-id="28032-149">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="28032-149">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="28032-150">O estado de saúde atual da categoria "BestPratices" da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="28032-150">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="28032-151">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="28032-151">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="28032-152">appHealthState</span><span class="sxs-lookup"><span data-stu-id="28032-152">appHealthState</span></span>|[<span data-ttu-id="28032-153">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="28032-153">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="28032-154">O estado de saúde atual da categoria "BestPratices" da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="28032-154">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="28032-155">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="28032-155">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28032-156">Relações</span><span class="sxs-lookup"><span data-stu-id="28032-156">Relationships</span></span>
<span data-ttu-id="28032-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="28032-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28032-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28032-158">JSON Representation</span></span>
<span data-ttu-id="28032-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="28032-159">Here is a JSON representation of the resource.</span></span>
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
  "appHealthState": "String"
}
```




