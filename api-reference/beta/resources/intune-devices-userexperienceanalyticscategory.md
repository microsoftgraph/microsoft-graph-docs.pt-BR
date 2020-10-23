---
title: tipo de recurso userExperienceAnalyticsCategory
description: A entidade de categoria da experiência do usuário contém as pontuações e insights para as várias métricas de uma categoria.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 095e88a372d0f06c34eb61c4de0bd2e06617cdf0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728099"
---
# <a name="userexperienceanalyticscategory-resource-type"></a><span data-ttu-id="8b684-103">tipo de recurso userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="8b684-103">userExperienceAnalyticsCategory resource type</span></span>

<span data-ttu-id="8b684-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b684-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b684-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8b684-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b684-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8b684-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b684-107">A entidade de categoria da experiência do usuário contém as pontuações e insights para as várias métricas de uma categoria.</span><span class="sxs-lookup"><span data-stu-id="8b684-107">The user experience analytics category entity contains the scores and insights for the various metrics of a category.</span></span>

## <a name="methods"></a><span data-ttu-id="8b684-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="8b684-108">Methods</span></span>
|<span data-ttu-id="8b684-109">Método</span><span class="sxs-lookup"><span data-stu-id="8b684-109">Method</span></span>|<span data-ttu-id="8b684-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8b684-110">Return Type</span></span>|<span data-ttu-id="8b684-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b684-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8b684-112">Obter userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="8b684-112">Get userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-get.md)|[<span data-ttu-id="8b684-113">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="8b684-113">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="8b684-114">Leia as propriedades e as relações do objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="8b684-114">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|
|[<span data-ttu-id="8b684-115">Atualizar userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="8b684-115">Update userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-update.md)|[<span data-ttu-id="8b684-116">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="8b684-116">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="8b684-117">Atualiza as propriedades de um objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="8b684-117">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8b684-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8b684-118">Properties</span></span>
|<span data-ttu-id="8b684-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b684-119">Property</span></span>|<span data-ttu-id="8b684-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b684-120">Type</span></span>|<span data-ttu-id="8b684-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b684-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b684-122">id</span><span class="sxs-lookup"><span data-stu-id="8b684-122">id</span></span>|<span data-ttu-id="8b684-123">String</span><span class="sxs-lookup"><span data-stu-id="8b684-123">String</span></span>|<span data-ttu-id="8b684-124">O identificador exclusivo da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8b684-124">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="8b684-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="8b684-125">overallScore</span></span>|<span data-ttu-id="8b684-126">Int32</span><span class="sxs-lookup"><span data-stu-id="8b684-126">Int32</span></span>|<span data-ttu-id="8b684-127">A pontuação geral da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8b684-127">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="8b684-128">insights</span><span class="sxs-lookup"><span data-stu-id="8b684-128">insights</span></span>|<span data-ttu-id="8b684-129">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="8b684-129">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="8b684-130">O insights para a categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8b684-130">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="8b684-131">state</span><span class="sxs-lookup"><span data-stu-id="8b684-131">state</span></span>|[<span data-ttu-id="8b684-132">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="8b684-132">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="8b684-133">O estado de integridade atual da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8b684-133">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="8b684-134">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="8b684-134">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8b684-135">Relações</span><span class="sxs-lookup"><span data-stu-id="8b684-135">Relationships</span></span>
|<span data-ttu-id="8b684-136">Relação</span><span class="sxs-lookup"><span data-stu-id="8b684-136">Relationship</span></span>|<span data-ttu-id="8b684-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b684-137">Type</span></span>|<span data-ttu-id="8b684-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b684-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b684-139">metricValues</span><span class="sxs-lookup"><span data-stu-id="8b684-139">metricValues</span></span>|<span data-ttu-id="8b684-140">coleção [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)</span><span class="sxs-lookup"><span data-stu-id="8b684-140">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) collection</span></span>|<span data-ttu-id="8b684-141">Os valores de métrica da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="8b684-141">The metric values for the user experience analytics category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8b684-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8b684-142">JSON Representation</span></span>
<span data-ttu-id="8b684-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8b684-143">Here is a JSON representation of the resource.</span></span>
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
          "value": "4.2"
        }
      ],
      "severity": "String"
    }
  ],
  "state": "String"
}
```





