---
title: tipo de recurso userExperienceAnalyticsCategory
description: A entidade de categoria da experiência do usuário contém as pontuações e insights para as várias métricas de uma categoria.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 81da542a14e20460f9b7b9f3dc81df390e344dd3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528483"
---
# <a name="userexperienceanalyticscategory-resource-type"></a><span data-ttu-id="e9ef4-103">tipo de recurso userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="e9ef4-103">userExperienceAnalyticsCategory resource type</span></span>

<span data-ttu-id="e9ef4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e9ef4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9ef4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e9ef4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9ef4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e9ef4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9ef4-107">A entidade de categoria da experiência do usuário contém as pontuações e insights para as várias métricas de uma categoria.</span><span class="sxs-lookup"><span data-stu-id="e9ef4-107">The user experience analytics category entity contains the scores and insights for the various metrics of a category.</span></span>

## <a name="methods"></a><span data-ttu-id="e9ef4-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="e9ef4-108">Methods</span></span>
|<span data-ttu-id="e9ef4-109">Método</span><span class="sxs-lookup"><span data-stu-id="e9ef4-109">Method</span></span>|<span data-ttu-id="e9ef4-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e9ef4-110">Return Type</span></span>|<span data-ttu-id="e9ef4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9ef4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e9ef4-112">Obter userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="e9ef4-112">Get userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-get.md)|[<span data-ttu-id="e9ef4-113">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="e9ef4-113">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="e9ef4-114">Leia as propriedades e as relações do objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="e9ef4-114">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|
|[<span data-ttu-id="e9ef4-115">Atualizar userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="e9ef4-115">Update userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-update.md)|[<span data-ttu-id="e9ef4-116">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="e9ef4-116">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="e9ef4-117">Atualiza as propriedades de um objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="e9ef4-117">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e9ef4-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e9ef4-118">Properties</span></span>
|<span data-ttu-id="e9ef4-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e9ef4-119">Property</span></span>|<span data-ttu-id="e9ef4-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9ef4-120">Type</span></span>|<span data-ttu-id="e9ef4-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9ef4-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9ef4-122">id</span><span class="sxs-lookup"><span data-stu-id="e9ef4-122">id</span></span>|<span data-ttu-id="e9ef4-123">String</span><span class="sxs-lookup"><span data-stu-id="e9ef4-123">String</span></span>|<span data-ttu-id="e9ef4-124">O identificador exclusivo da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9ef4-124">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="e9ef4-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="e9ef4-125">overallScore</span></span>|<span data-ttu-id="e9ef4-126">Int32</span><span class="sxs-lookup"><span data-stu-id="e9ef4-126">Int32</span></span>|<span data-ttu-id="e9ef4-127">A pontuação geral da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9ef4-127">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="e9ef4-128">insights</span><span class="sxs-lookup"><span data-stu-id="e9ef4-128">insights</span></span>|<span data-ttu-id="e9ef4-129">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="e9ef4-129">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="e9ef4-130">O insights para a categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9ef4-130">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="e9ef4-131">state</span><span class="sxs-lookup"><span data-stu-id="e9ef4-131">state</span></span>|[<span data-ttu-id="e9ef4-132">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="e9ef4-132">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="e9ef4-133">O estado de integridade atual da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9ef4-133">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="e9ef4-134">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="e9ef4-134">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9ef4-135">Relações</span><span class="sxs-lookup"><span data-stu-id="e9ef4-135">Relationships</span></span>
|<span data-ttu-id="e9ef4-136">Relação</span><span class="sxs-lookup"><span data-stu-id="e9ef4-136">Relationship</span></span>|<span data-ttu-id="e9ef4-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="e9ef4-137">Type</span></span>|<span data-ttu-id="e9ef4-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="e9ef4-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9ef4-139">metricValues</span><span class="sxs-lookup"><span data-stu-id="e9ef4-139">metricValues</span></span>|<span data-ttu-id="e9ef4-140">coleção [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)</span><span class="sxs-lookup"><span data-stu-id="e9ef4-140">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) collection</span></span>|<span data-ttu-id="e9ef4-141">Os valores de métrica da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e9ef4-141">The metric values for the user experience analytics category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9ef4-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e9ef4-142">JSON Representation</span></span>
<span data-ttu-id="e9ef4-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e9ef4-143">Here is a JSON representation of the resource.</span></span>
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
  "overallScore": 1024,
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



