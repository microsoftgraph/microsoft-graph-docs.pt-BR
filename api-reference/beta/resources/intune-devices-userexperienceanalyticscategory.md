---
title: tipo de recurso userExperienceAnalyticsCategory
description: A entidade de categoria da experiência do usuário contém as pontuações e insights para as várias métricas de uma categoria.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5c04f2caaa7b9ee6c093a58e4c8123250113b3a9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36329639"
---
# <a name="userexperienceanalyticscategory-resource-type"></a><span data-ttu-id="13ca7-103">tipo de recurso userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="13ca7-103">userExperienceAnalyticsCategory resource type</span></span>

> <span data-ttu-id="13ca7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="13ca7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13ca7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="13ca7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13ca7-106">A entidade de categoria da experiência do usuário contém as pontuações e insights para as várias métricas de uma categoria.</span><span class="sxs-lookup"><span data-stu-id="13ca7-106">The user experience analytics category entity contains the scores and insights for the various metrics of a category.</span></span>

## <a name="methods"></a><span data-ttu-id="13ca7-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="13ca7-107">Methods</span></span>
|<span data-ttu-id="13ca7-108">Método</span><span class="sxs-lookup"><span data-stu-id="13ca7-108">Method</span></span>|<span data-ttu-id="13ca7-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="13ca7-109">Return Type</span></span>|<span data-ttu-id="13ca7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="13ca7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="13ca7-111">Obter userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="13ca7-111">Get userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-get.md)|[<span data-ttu-id="13ca7-112">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="13ca7-112">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="13ca7-113">Leia as propriedades e as relações do objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="13ca7-113">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|
|[<span data-ttu-id="13ca7-114">Atualizar userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="13ca7-114">Update userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-update.md)|[<span data-ttu-id="13ca7-115">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="13ca7-115">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="13ca7-116">Atualiza as propriedades de um objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="13ca7-116">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="13ca7-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="13ca7-117">Properties</span></span>
|<span data-ttu-id="13ca7-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="13ca7-118">Property</span></span>|<span data-ttu-id="13ca7-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="13ca7-119">Type</span></span>|<span data-ttu-id="13ca7-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="13ca7-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13ca7-121">id</span><span class="sxs-lookup"><span data-stu-id="13ca7-121">id</span></span>|<span data-ttu-id="13ca7-122">String</span><span class="sxs-lookup"><span data-stu-id="13ca7-122">String</span></span>|<span data-ttu-id="13ca7-123">O identificador exclusivo da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="13ca7-123">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="13ca7-124">displayName</span><span class="sxs-lookup"><span data-stu-id="13ca7-124">displayName</span></span>|<span data-ttu-id="13ca7-125">String</span><span class="sxs-lookup"><span data-stu-id="13ca7-125">String</span></span>|<span data-ttu-id="13ca7-126">O nome da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="13ca7-126">The name of the user experience analytics category.</span></span>|
|<span data-ttu-id="13ca7-127">overallScore</span><span class="sxs-lookup"><span data-stu-id="13ca7-127">overallScore</span></span>|<span data-ttu-id="13ca7-128">Int32</span><span class="sxs-lookup"><span data-stu-id="13ca7-128">Int32</span></span>|<span data-ttu-id="13ca7-129">A pontuação geral da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="13ca7-129">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="13ca7-130">insights</span><span class="sxs-lookup"><span data-stu-id="13ca7-130">insights</span></span>|<span data-ttu-id="13ca7-131">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="13ca7-131">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="13ca7-132">O insights para a categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="13ca7-132">The insights for the user experience analytics category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13ca7-133">Relações</span><span class="sxs-lookup"><span data-stu-id="13ca7-133">Relationships</span></span>
|<span data-ttu-id="13ca7-134">Relação</span><span class="sxs-lookup"><span data-stu-id="13ca7-134">Relationship</span></span>|<span data-ttu-id="13ca7-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="13ca7-135">Type</span></span>|<span data-ttu-id="13ca7-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="13ca7-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13ca7-137">metricValues</span><span class="sxs-lookup"><span data-stu-id="13ca7-137">metricValues</span></span>|<span data-ttu-id="13ca7-138">coleção [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)</span><span class="sxs-lookup"><span data-stu-id="13ca7-138">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) collection</span></span>|<span data-ttu-id="13ca7-139">Os valores de métrica da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="13ca7-139">The metric values for the user experience analytics category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13ca7-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="13ca7-140">JSON Representation</span></span>
<span data-ttu-id="13ca7-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="13ca7-141">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "overallScore": 1024,
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



