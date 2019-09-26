---
title: tipo de recurso userExperienceAnalyticsCategory
description: A entidade de categoria da experiência do usuário contém as pontuações e insights para as várias métricas de uma categoria.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2f9bd4947a65d98c465671e338e0d21a6218211f
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196711"
---
# <a name="userexperienceanalyticscategory-resource-type"></a><span data-ttu-id="581dc-103">tipo de recurso userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="581dc-103">userExperienceAnalyticsCategory resource type</span></span>

> <span data-ttu-id="581dc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="581dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="581dc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="581dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="581dc-106">A entidade de categoria da experiência do usuário contém as pontuações e insights para as várias métricas de uma categoria.</span><span class="sxs-lookup"><span data-stu-id="581dc-106">The user experience analytics category entity contains the scores and insights for the various metrics of a category.</span></span>

## <a name="methods"></a><span data-ttu-id="581dc-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="581dc-107">Methods</span></span>
|<span data-ttu-id="581dc-108">Método</span><span class="sxs-lookup"><span data-stu-id="581dc-108">Method</span></span>|<span data-ttu-id="581dc-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="581dc-109">Return Type</span></span>|<span data-ttu-id="581dc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="581dc-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="581dc-111">Obter userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="581dc-111">Get userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-get.md)|[<span data-ttu-id="581dc-112">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="581dc-112">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="581dc-113">Leia as propriedades e as relações do objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="581dc-113">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|
|[<span data-ttu-id="581dc-114">Atualizar userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="581dc-114">Update userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-update.md)|[<span data-ttu-id="581dc-115">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="581dc-115">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="581dc-116">Atualiza as propriedades de um objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="581dc-116">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="581dc-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="581dc-117">Properties</span></span>
|<span data-ttu-id="581dc-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="581dc-118">Property</span></span>|<span data-ttu-id="581dc-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="581dc-119">Type</span></span>|<span data-ttu-id="581dc-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="581dc-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="581dc-121">id</span><span class="sxs-lookup"><span data-stu-id="581dc-121">id</span></span>|<span data-ttu-id="581dc-122">String</span><span class="sxs-lookup"><span data-stu-id="581dc-122">String</span></span>|<span data-ttu-id="581dc-123">O identificador exclusivo da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="581dc-123">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="581dc-124">overallScore</span><span class="sxs-lookup"><span data-stu-id="581dc-124">overallScore</span></span>|<span data-ttu-id="581dc-125">Int32</span><span class="sxs-lookup"><span data-stu-id="581dc-125">Int32</span></span>|<span data-ttu-id="581dc-126">A pontuação geral da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="581dc-126">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="581dc-127">insights</span><span class="sxs-lookup"><span data-stu-id="581dc-127">insights</span></span>|<span data-ttu-id="581dc-128">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="581dc-128">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="581dc-129">O insights para a categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="581dc-129">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="581dc-130">estado</span><span class="sxs-lookup"><span data-stu-id="581dc-130">state</span></span>|[<span data-ttu-id="581dc-131">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="581dc-131">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="581dc-132">O estado de integridade atual da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="581dc-132">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="581dc-133">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="581dc-133">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="581dc-134">Relações</span><span class="sxs-lookup"><span data-stu-id="581dc-134">Relationships</span></span>
|<span data-ttu-id="581dc-135">Relação</span><span class="sxs-lookup"><span data-stu-id="581dc-135">Relationship</span></span>|<span data-ttu-id="581dc-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="581dc-136">Type</span></span>|<span data-ttu-id="581dc-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="581dc-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="581dc-138">metricValues</span><span class="sxs-lookup"><span data-stu-id="581dc-138">metricValues</span></span>|<span data-ttu-id="581dc-139">coleção [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)</span><span class="sxs-lookup"><span data-stu-id="581dc-139">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) collection</span></span>|<span data-ttu-id="581dc-140">Os valores de métrica da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="581dc-140">The metric values for the user experience analytics category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="581dc-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="581dc-141">JSON Representation</span></span>
<span data-ttu-id="581dc-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="581dc-142">Here is a JSON representation of the resource.</span></span>
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



