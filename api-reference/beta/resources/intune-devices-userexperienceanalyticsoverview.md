---
title: tipo de recurso userExperienceAnalyticsOverview
description: A entidade visão geral da análise da experiência do usuário contém a pontuação geral e as pontuações e os resultados de cada métrica de todas as categorias.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 90a33468dfe0d68303625f7a682fdc23d34b7504
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536108"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="e23f1-103">tipo de recurso userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="e23f1-103">userExperienceAnalyticsOverview resource type</span></span>

> <span data-ttu-id="e23f1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e23f1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e23f1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e23f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e23f1-106">A entidade visão geral da análise da experiência do usuário contém a pontuação geral e as pontuações e os resultados de cada métrica de todas as categorias.</span><span class="sxs-lookup"><span data-stu-id="e23f1-106">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="e23f1-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e23f1-107">Methods</span></span>
|<span data-ttu-id="e23f1-108">Método</span><span class="sxs-lookup"><span data-stu-id="e23f1-108">Method</span></span>|<span data-ttu-id="e23f1-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e23f1-109">Return Type</span></span>|<span data-ttu-id="e23f1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e23f1-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e23f1-111">Obter userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="e23f1-111">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="e23f1-112">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="e23f1-112">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="e23f1-113">Leia as propriedades e as relações do objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="e23f1-113">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="e23f1-114">Atualizar userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="e23f1-114">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="e23f1-115">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="e23f1-115">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="e23f1-116">Atualiza as propriedades de um objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="e23f1-116">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e23f1-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e23f1-117">Properties</span></span>
|<span data-ttu-id="e23f1-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e23f1-118">Property</span></span>|<span data-ttu-id="e23f1-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e23f1-119">Type</span></span>|<span data-ttu-id="e23f1-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e23f1-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e23f1-121">id</span><span class="sxs-lookup"><span data-stu-id="e23f1-121">id</span></span>|<span data-ttu-id="e23f1-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e23f1-122">String</span></span>|<span data-ttu-id="e23f1-123">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e23f1-123">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="e23f1-124">overallScore</span><span class="sxs-lookup"><span data-stu-id="e23f1-124">overallScore</span></span>|<span data-ttu-id="e23f1-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e23f1-125">Int32</span></span>|<span data-ttu-id="e23f1-126">A pontuação geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e23f1-126">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="e23f1-127">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="e23f1-127">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="e23f1-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e23f1-128">Int32</span></span>|<span data-ttu-id="e23f1-129">A pontuação geral do desempenho de inicialização do dispositivo analítico da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e23f1-129">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="e23f1-130">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="e23f1-130">bestPracticesOverallScore</span></span>|<span data-ttu-id="e23f1-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e23f1-131">Int32</span></span>|<span data-ttu-id="e23f1-132">A pontuação geral das práticas recomendadas de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e23f1-132">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="e23f1-133">insights</span><span class="sxs-lookup"><span data-stu-id="e23f1-133">insights</span></span>|<span data-ttu-id="e23f1-134">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="e23f1-134">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="e23f1-135">A experiência do usuário do Analytics insights.</span><span class="sxs-lookup"><span data-stu-id="e23f1-135">The user experience analytics insights.</span></span>|
|<span data-ttu-id="e23f1-136">state</span><span class="sxs-lookup"><span data-stu-id="e23f1-136">state</span></span>|[<span data-ttu-id="e23f1-137">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="e23f1-137">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="e23f1-138">O estado de integridade atual da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e23f1-138">The current health state of the user experience analytics overview.</span></span> <span data-ttu-id="e23f1-139">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="e23f1-139">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="e23f1-140">deviceBootPerformanceHealthState</span><span class="sxs-lookup"><span data-stu-id="e23f1-140">deviceBootPerformanceHealthState</span></span>|[<span data-ttu-id="e23f1-141">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="e23f1-141">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="e23f1-142">O estado de integridade atual da categoria "BootPerformance" da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e23f1-142">The current health state of the user experience analytics 'BootPerformance' category.</span></span> <span data-ttu-id="e23f1-143">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="e23f1-143">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|
|<span data-ttu-id="e23f1-144">bestPracticesHealthState</span><span class="sxs-lookup"><span data-stu-id="e23f1-144">bestPracticesHealthState</span></span>|[<span data-ttu-id="e23f1-145">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="e23f1-145">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="e23f1-146">O estado de integridade atual da categoria "BestPractices" da análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e23f1-146">The current health state of the user experience analytics 'BestPractices' category.</span></span> <span data-ttu-id="e23f1-147">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="e23f1-147">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e23f1-148">Relações</span><span class="sxs-lookup"><span data-stu-id="e23f1-148">Relationships</span></span>
<span data-ttu-id="e23f1-149">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e23f1-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e23f1-150">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e23f1-150">JSON Representation</span></span>
<span data-ttu-id="e23f1-151">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e23f1-151">Here is a JSON representation of the resource.</span></span>
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
          "value": "<Unknown Primitive Type Edm.Double>"
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



