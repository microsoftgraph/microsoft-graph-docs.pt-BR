---
title: tipo de recurso userExperienceAnalyticsOverview
description: A entidade visão geral da análise da experiência do usuário contém a pontuação geral e as pontuações e os resultados de cada métrica de todas as categorias.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff3be73059f913943236bfce8bcb4e729a39081d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371436"
---
# <a name="userexperienceanalyticsoverview-resource-type"></a><span data-ttu-id="87555-103">tipo de recurso userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="87555-103">userExperienceAnalyticsOverview resource type</span></span>

> <span data-ttu-id="87555-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="87555-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87555-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87555-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87555-106">A entidade visão geral da análise da experiência do usuário contém a pontuação geral e as pontuações e os resultados de cada métrica de todas as categorias.</span><span class="sxs-lookup"><span data-stu-id="87555-106">The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.</span></span>

## <a name="methods"></a><span data-ttu-id="87555-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="87555-107">Methods</span></span>
|<span data-ttu-id="87555-108">Método</span><span class="sxs-lookup"><span data-stu-id="87555-108">Method</span></span>|<span data-ttu-id="87555-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="87555-109">Return Type</span></span>|<span data-ttu-id="87555-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="87555-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="87555-111">Obter userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="87555-111">Get userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[<span data-ttu-id="87555-112">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="87555-112">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="87555-113">Leia as propriedades e as relações do objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="87555-113">Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|
|[<span data-ttu-id="87555-114">Atualizar userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="87555-114">Update userExperienceAnalyticsOverview</span></span>](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[<span data-ttu-id="87555-115">userExperienceAnalyticsOverview</span><span class="sxs-lookup"><span data-stu-id="87555-115">userExperienceAnalyticsOverview</span></span>](../resources/intune-devices-userexperienceanalyticsoverview.md)|<span data-ttu-id="87555-116">Atualiza as propriedades de um objeto [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) .</span><span class="sxs-lookup"><span data-stu-id="87555-116">Update the properties of a [userExperienceAnalyticsOverview](../resources/intune-devices-userexperienceanalyticsoverview.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="87555-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87555-117">Properties</span></span>
|<span data-ttu-id="87555-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87555-118">Property</span></span>|<span data-ttu-id="87555-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="87555-119">Type</span></span>|<span data-ttu-id="87555-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="87555-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87555-121">id</span><span class="sxs-lookup"><span data-stu-id="87555-121">id</span></span>|<span data-ttu-id="87555-122">String</span><span class="sxs-lookup"><span data-stu-id="87555-122">String</span></span>|<span data-ttu-id="87555-123">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="87555-123">The unique identifier of the user experience analytics overview.</span></span>|
|<span data-ttu-id="87555-124">overallScore</span><span class="sxs-lookup"><span data-stu-id="87555-124">overallScore</span></span>|<span data-ttu-id="87555-125">Int32</span><span class="sxs-lookup"><span data-stu-id="87555-125">Int32</span></span>|<span data-ttu-id="87555-126">A pontuação geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="87555-126">The user experience analytics overall score.</span></span>|
|<span data-ttu-id="87555-127">deviceBootPerformanceOverallScore</span><span class="sxs-lookup"><span data-stu-id="87555-127">deviceBootPerformanceOverallScore</span></span>|<span data-ttu-id="87555-128">Int32</span><span class="sxs-lookup"><span data-stu-id="87555-128">Int32</span></span>|<span data-ttu-id="87555-129">A pontuação geral do desempenho de inicialização do dispositivo analítico da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="87555-129">The user experience analytics device boot performance overall score.</span></span>|
|<span data-ttu-id="87555-130">bestPracticesOverallScore</span><span class="sxs-lookup"><span data-stu-id="87555-130">bestPracticesOverallScore</span></span>|<span data-ttu-id="87555-131">Int32</span><span class="sxs-lookup"><span data-stu-id="87555-131">Int32</span></span>|<span data-ttu-id="87555-132">A pontuação geral das práticas recomendadas de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="87555-132">The user experience analytics best practices overall score.</span></span>|
|<span data-ttu-id="87555-133">insights</span><span class="sxs-lookup"><span data-stu-id="87555-133">insights</span></span>|<span data-ttu-id="87555-134">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="87555-134">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="87555-135">A experiência do usuário do Analytics insights.</span><span class="sxs-lookup"><span data-stu-id="87555-135">The user experience analytics insights.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87555-136">Relações</span><span class="sxs-lookup"><span data-stu-id="87555-136">Relationships</span></span>
<span data-ttu-id="87555-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="87555-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87555-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87555-138">JSON Representation</span></span>
<span data-ttu-id="87555-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87555-139">Here is a JSON representation of the resource.</span></span>
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
      "value": [
        {
          "@odata.type": "microsoft.graph.insightValueDouble"
        }
      ]
    }
  ]
}
```



