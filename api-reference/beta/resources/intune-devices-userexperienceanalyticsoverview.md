---
title: tipo de recurso userExperienceAnalyticsOverview
description: A entidade visão geral da análise da experiência do usuário contém a pontuação geral e as pontuações e os resultados de cada métrica de todas as categorias.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 152f5ef93db38ffced60bf93e3215d45cf822ba5
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44175515"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="ba026-103">tipo de recurso userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="ba026-103">userExperienceAnalyticsOverview resource type</span></span>

<span data-ttu-id="ba026-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba026-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba026-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ba026-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba026-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ba026-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba026-107">A entidade visão geral da análise da experiência do usuário contém a pontuação geral e as pontuações e os resultados de cada métrica de todas as categorias.</span><span class="sxs-lookup"><span data-stu-id="ba026-107">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="ba026-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="ba026-108">Methods</span></span>
|<span data-ttu-id="ba026-109">Método</span><span class="sxs-lookup"><span data-stu-id="ba026-109">Method</span></span>|<span data-ttu-id="ba026-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ba026-110">Return Type</span></span>|<span data-ttu-id="ba026-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba026-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ba026-112">Obter userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="ba026-112">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="ba026-113">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="ba026-113">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="ba026-114">Leia as propriedades e as relações do objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="ba026-114">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="ba026-115">Atualizar userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="ba026-115">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="ba026-116">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="ba026-116">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="ba026-117">Atualiza as propriedades de um objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="ba026-117">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ba026-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba026-118">Properties</span></span>
|<span data-ttu-id="ba026-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba026-119">Property</span></span>|<span data-ttu-id="ba026-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba026-120">Type</span></span>|<span data-ttu-id="ba026-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba026-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba026-122">id</span><span class="sxs-lookup"><span data-stu-id="ba026-122">id</span></span>|<span data-ttu-id="ba026-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba026-123">String</span></span>|<span data-ttu-id="ba026-124">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ba026-124">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="ba026-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="ba026-125">overallScore</span></span>|<span data-ttu-id="ba026-126">Int32</span><span class="sxs-lookup"><span data-stu-id="ba026-126">Int32</span></span>|<span data-ttu-id="ba026-127">A pontuação geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ba026-127">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="ba026-128">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="ba026-128">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="ba026-129">Int32</span><span class="sxs-lookup"><span data-stu-id="ba026-129">Int32</span></span>|<span data-ttu-id="ba026-130">A pontuação geral do desempenho de inicialização do dispositivo analítico da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ba026-130">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="ba026-131">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="ba026-131">bestPracticesOverallScore</span></span>|<span data-ttu-id="ba026-132">Int32</span><span class="sxs-lookup"><span data-stu-id="ba026-132">Int32</span></span>|<span data-ttu-id="ba026-133">A pontuação geral das práticas recomendadas de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ba026-133">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="ba026-134">insights</span><span class="sxs-lookup"><span data-stu-id="ba026-134">insights</span></span>|<span data-ttu-id="ba026-135">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="ba026-135">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="ba026-136">A experiência do usuário do Analytics insights.</span><span class="sxs-lookup"><span data-stu-id="ba026-136">The user experience analytics insights.</span></span>|
|<span data-ttu-id="ba026-137">state</span><span class="sxs-lookup"><span data-stu-id="ba026-137">state</span></span>|[<span data-ttu-id="ba026-138">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="ba026-138">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="ba026-139">O estado de integridade atual da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ba026-139">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="ba026-140">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="ba026-140">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="ba026-141">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="ba026-141">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="ba026-142">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="ba026-142">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="ba026-143">O estado de integridade atual da categoria "BootPerformance" da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ba026-143">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="ba026-144">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="ba026-144">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="ba026-145">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="ba026-145">bestPracticesHealthState</span></span>|[<span data-ttu-id="ba026-146">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="ba026-146">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="ba026-147">O estado de integridade atual da categoria "BestPractices" da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ba026-147">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="ba026-148">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="ba026-148">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ba026-149">Relações</span><span class="sxs-lookup"><span data-stu-id="ba026-149">Relationships</span></span>
<span data-ttu-id="ba026-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ba026-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba026-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba026-151">JSON Representation</span></span>
<span data-ttu-id="ba026-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba026-152">Here is a JSON representation of the resource.</span></span>
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
  "bestPracticesHealthState": "String"
}
```



