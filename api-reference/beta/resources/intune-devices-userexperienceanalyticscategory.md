---
title: tipo de recurso userExperienceAnalyticsCategory
description: A entidade de categoria da experiência do usuário contém as pontuações e insights para as várias métricas de uma categoria.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8d80a287b736786a14eac1244b3e42e07b8e6dad
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178098"
---
# <a name="userexperienceanalyticscategory-resource-type"></a><span data-ttu-id="e890c-103">tipo de recurso userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="e890c-103">userExperienceAnalyticsCategory resource type</span></span>

<span data-ttu-id="e890c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e890c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e890c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e890c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e890c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e890c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e890c-107">A entidade de categoria da experiência do usuário contém as pontuações e insights para as várias métricas de uma categoria.</span><span class="sxs-lookup"><span data-stu-id="e890c-107">The user experience analytics category entity contains the scores and insights for the various metrics of a category.</span></span>

## <a name="methods"></a><span data-ttu-id="e890c-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="e890c-108">Methods</span></span>
|<span data-ttu-id="e890c-109">Método</span><span class="sxs-lookup"><span data-stu-id="e890c-109">Method</span></span>|<span data-ttu-id="e890c-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e890c-110">Return Type</span></span>|<span data-ttu-id="e890c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e890c-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e890c-112">Obter userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="e890c-112">Get userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-get.md)|[<span data-ttu-id="e890c-113">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="e890c-113">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="e890c-114">Leia as propriedades e as relações do objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="e890c-114">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|
|[<span data-ttu-id="e890c-115">Atualizar userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="e890c-115">Update userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-update.md)|[<span data-ttu-id="e890c-116">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="e890c-116">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="e890c-117">Atualiza as propriedades de um objeto [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) .</span><span class="sxs-lookup"><span data-stu-id="e890c-117">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e890c-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e890c-118">Properties</span></span>
|<span data-ttu-id="e890c-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e890c-119">Property</span></span>|<span data-ttu-id="e890c-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="e890c-120">Type</span></span>|<span data-ttu-id="e890c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e890c-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e890c-122">id</span><span class="sxs-lookup"><span data-stu-id="e890c-122">id</span></span>|<span data-ttu-id="e890c-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e890c-123">String</span></span>|<span data-ttu-id="e890c-124">O identificador exclusivo da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e890c-124">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="e890c-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="e890c-125">overallScore</span></span>|<span data-ttu-id="e890c-126">Int32</span><span class="sxs-lookup"><span data-stu-id="e890c-126">Int32</span></span>|<span data-ttu-id="e890c-127">A pontuação geral da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e890c-127">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="e890c-128">insights</span><span class="sxs-lookup"><span data-stu-id="e890c-128">insights</span></span>|<span data-ttu-id="e890c-129">coleção [userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="e890c-129">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="e890c-130">O insights para a categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e890c-130">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="e890c-131">state</span><span class="sxs-lookup"><span data-stu-id="e890c-131">state</span></span>|[<span data-ttu-id="e890c-132">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="e890c-132">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="e890c-133">O estado de integridade atual da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e890c-133">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="e890c-134">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="e890c-134">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e890c-135">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="e890c-135">Relationships</span></span>
|<span data-ttu-id="e890c-136">Relação</span><span class="sxs-lookup"><span data-stu-id="e890c-136">Relationship</span></span>|<span data-ttu-id="e890c-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="e890c-137">Type</span></span>|<span data-ttu-id="e890c-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="e890c-138">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e890c-139">metricValues</span><span class="sxs-lookup"><span data-stu-id="e890c-139">metricValues</span></span>|<span data-ttu-id="e890c-140">coleção [userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)</span><span class="sxs-lookup"><span data-stu-id="e890c-140">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) collection</span></span>|<span data-ttu-id="e890c-141">Os valores de métrica da categoria de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="e890c-141">The metric values for the user experience analytics category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e890c-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e890c-142">JSON Representation</span></span>
<span data-ttu-id="e890c-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e890c-143">Here is a JSON representation of the resource.</span></span>
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



