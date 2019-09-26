---
title: tipo de recurso userExperienceAnalyticsOverview
description: A entidade visão geral da análise da experiência do usuário contém a pontuação geral e as pontuações e os resultados de cada métrica de todas as categorias.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 11c7bbe64b1495a9e6cb0b8ac144d1afb539789f
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196669"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="e23f4-103">tipo de recurso userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="e23f4-103">userExperienceAnalyticsOverview resource type</span></span>

> <span data-ttu-id="e23f4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e23f4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e23f4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e23f4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e23f4-106">A entidade visão geral da análise da experiência do usuário contém a pontuação geral e as pontuações e os resultados de cada métrica de todas as categorias.</span><span class="sxs-lookup"><span data-stu-id="e23f4-106">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="e23f4-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e23f4-107">Methods</span></span>
|<span data-ttu-id="e23f4-108">Método</span><span class="sxs-lookup"><span data-stu-id="e23f4-108">Method</span></span>|<span data-ttu-id="e23f4-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e23f4-109">Return Type</span></span>|<span data-ttu-id="e23f4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e23f4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e23f4-111">Obter userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="e23f4-111">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="e23f4-112">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="e23f4-112">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="e23f4-113">Leia as propriedades e as relações do objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="e23f4-113">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="e23f4-114">Atualizar userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="e23f4-114">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="e23f4-115">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="e23f4-115">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="e23f4-116">Atualiza as propriedades de um objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="e23f4-116">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e23f4-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e23f4-117">Properties</span></span>
|<span data-ttu-id="e23f4-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e23f4-118">Property</span></span>|<span data-ttu-id="e23f4-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e23f4-119">Type</span></span>|<span data-ttu-id="e23f4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e23f4-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e23f4-121">id</span><span class="sxs-lookup"><span data-stu-id="e23f4-121">id</span></span>|<span data-ttu-id="e23f4-122">String</span><span class="sxs-lookup"><span data-stu-id="e23f4-122">String</span></span>|<span data-ttu-id="e23f4-123">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e23f4-123">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="e23f4-124">overallScore</span><span class="sxs-lookup"><span data-stu-id="e23f4-124">overallScore</span></span>|<span data-ttu-id="e23f4-125">Int32</span><span class="sxs-lookup"><span data-stu-id="e23f4-125">Int32</span></span>|<span data-ttu-id="e23f4-126">A pontuação geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e23f4-126">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="e23f4-127">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="e23f4-127">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="e23f4-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e23f4-128">Int32</span></span>|<span data-ttu-id="e23f4-129">A pontuação geral do desempenho de inicialização do dispositivo analítico da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e23f4-129">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="e23f4-130">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="e23f4-130">bestPracticesOverallScore</span></span>|<span data-ttu-id="e23f4-131">Int32</span><span class="sxs-lookup"><span data-stu-id="e23f4-131">Int32</span></span>|<span data-ttu-id="e23f4-132">A pontuação geral das práticas recomendadas de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e23f4-132">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="e23f4-133">insights</span><span class="sxs-lookup"><span data-stu-id="e23f4-133">insights</span></span>|<span data-ttu-id="e23f4-134">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="e23f4-134">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="e23f4-135">A experiência do usuário do Analytics insights.</span><span class="sxs-lookup"><span data-stu-id="e23f4-135">The user experience analytics insights.</span></span>|
|<span data-ttu-id="e23f4-136">estado</span><span class="sxs-lookup"><span data-stu-id="e23f4-136">state</span></span>|[<span data-ttu-id="e23f4-137">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="e23f4-137">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="e23f4-138">O estado de integridade atual da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e23f4-138">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="e23f4-139">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="e23f4-139">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e23f4-140">Relações</span><span class="sxs-lookup"><span data-stu-id="e23f4-140">Relationships</span></span>
<span data-ttu-id="e23f4-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e23f4-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e23f4-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e23f4-142">JSON Representation</span></span>
<span data-ttu-id="e23f4-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e23f4-143">Here is a JSON representation of the resource.</span></span>
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
  "state": "String"
}
```



