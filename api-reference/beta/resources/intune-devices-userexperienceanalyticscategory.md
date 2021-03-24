---
title: Tipo de recurso userExperienceAnalyticsCategory
description: A entidade de categoria de análise de experiência do usuário contém as pontuações e percepções para as várias métricas de uma categoria.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f138b2417bccd6ed089810335e375eb721af80c6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51141439"
---
# <a name="userexperienceanalyticscategory-resource-type"></a><span data-ttu-id="ed4bc-103">Tipo de recurso userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="ed4bc-103">userExperienceAnalyticsCategory resource type</span></span>

<span data-ttu-id="ed4bc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed4bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed4bc-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ed4bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ed4bc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ed4bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed4bc-107">A entidade de categoria de análise de experiência do usuário contém as pontuações e percepções para as várias métricas de uma categoria.</span><span class="sxs-lookup"><span data-stu-id="ed4bc-107">The user experience analytics category entity contains the scores and insights for the various metrics of a category.</span></span>

## <a name="methods"></a><span data-ttu-id="ed4bc-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="ed4bc-108">Methods</span></span>
|<span data-ttu-id="ed4bc-109">Método</span><span class="sxs-lookup"><span data-stu-id="ed4bc-109">Method</span></span>|<span data-ttu-id="ed4bc-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ed4bc-110">Return Type</span></span>|<span data-ttu-id="ed4bc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed4bc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ed4bc-112">Obter userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="ed4bc-112">Get userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-get.md)|[<span data-ttu-id="ed4bc-113">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="ed4bc-113">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="ed4bc-114">Ler propriedades e relações do [objeto userExperienceAnalyticsCategory.](../resources/intune-devices-userexperienceanalyticscategory.md)</span><span class="sxs-lookup"><span data-stu-id="ed4bc-114">Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|
|[<span data-ttu-id="ed4bc-115">Atualizar userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="ed4bc-115">Update userExperienceAnalyticsCategory</span></span>](../api/intune-devices-userexperienceanalyticscategory-update.md)|[<span data-ttu-id="ed4bc-116">userExperienceAnalyticsCategory</span><span class="sxs-lookup"><span data-stu-id="ed4bc-116">userExperienceAnalyticsCategory</span></span>](../resources/intune-devices-userexperienceanalyticscategory.md)|<span data-ttu-id="ed4bc-117">Atualize as propriedades de [um objeto userExperienceAnalyticsCategory.](../resources/intune-devices-userexperienceanalyticscategory.md)</span><span class="sxs-lookup"><span data-stu-id="ed4bc-117">Update the properties of a [userExperienceAnalyticsCategory](../resources/intune-devices-userexperienceanalyticscategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ed4bc-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ed4bc-118">Properties</span></span>
|<span data-ttu-id="ed4bc-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ed4bc-119">Property</span></span>|<span data-ttu-id="ed4bc-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed4bc-120">Type</span></span>|<span data-ttu-id="ed4bc-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed4bc-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed4bc-122">id</span><span class="sxs-lookup"><span data-stu-id="ed4bc-122">id</span></span>|<span data-ttu-id="ed4bc-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ed4bc-123">String</span></span>|<span data-ttu-id="ed4bc-124">O identificador exclusivo da categoria de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ed4bc-124">The unique identifier of the user experience analytics category.</span></span>|
|<span data-ttu-id="ed4bc-125">overallScore</span><span class="sxs-lookup"><span data-stu-id="ed4bc-125">overallScore</span></span>|<span data-ttu-id="ed4bc-126">Int32</span><span class="sxs-lookup"><span data-stu-id="ed4bc-126">Int32</span></span>|<span data-ttu-id="ed4bc-127">A pontuação geral da categoria de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ed4bc-127">The overall score of the user experience analytics category.</span></span>|
|<span data-ttu-id="ed4bc-128">totalDevices</span><span class="sxs-lookup"><span data-stu-id="ed4bc-128">totalDevices</span></span>|<span data-ttu-id="ed4bc-129">Int32</span><span class="sxs-lookup"><span data-stu-id="ed4bc-129">Int32</span></span>|<span data-ttu-id="ed4bc-130">A contagem total de dispositivos da categoria de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ed4bc-130">The total device count of the user experience analytics category.</span></span>|
|<span data-ttu-id="ed4bc-131">insights</span><span class="sxs-lookup"><span data-stu-id="ed4bc-131">insights</span></span>|<span data-ttu-id="ed4bc-132">[Coleção userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md)</span><span class="sxs-lookup"><span data-stu-id="ed4bc-132">[userExperienceAnalyticsInsight](../resources/intune-devices-userexperienceanalyticsinsight.md) collection</span></span>|<span data-ttu-id="ed4bc-133">Os insights para a categoria de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ed4bc-133">The insights for the user experience analytics category.</span></span>|
|<span data-ttu-id="ed4bc-134">state</span><span class="sxs-lookup"><span data-stu-id="ed4bc-134">state</span></span>|[<span data-ttu-id="ed4bc-135">userExperienceAnalyticsHealthState</span><span class="sxs-lookup"><span data-stu-id="ed4bc-135">userExperienceAnalyticsHealthState</span></span>](../resources/intune-devices-userexperienceanalyticshealthstate.md)|<span data-ttu-id="ed4bc-136">O estado de saúde atual da categoria de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ed4bc-136">The current health state of the user experience analytics category.</span></span> <span data-ttu-id="ed4bc-137">Os valores possíveis são: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span><span class="sxs-lookup"><span data-stu-id="ed4bc-137">Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ed4bc-138">Relações</span><span class="sxs-lookup"><span data-stu-id="ed4bc-138">Relationships</span></span>
|<span data-ttu-id="ed4bc-139">Relação</span><span class="sxs-lookup"><span data-stu-id="ed4bc-139">Relationship</span></span>|<span data-ttu-id="ed4bc-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="ed4bc-140">Type</span></span>|<span data-ttu-id="ed4bc-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="ed4bc-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed4bc-142">metricValues</span><span class="sxs-lookup"><span data-stu-id="ed4bc-142">metricValues</span></span>|<span data-ttu-id="ed4bc-143">[Coleção userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md)</span><span class="sxs-lookup"><span data-stu-id="ed4bc-143">[userExperienceAnalyticsMetric](../resources/intune-devices-userexperienceanalyticsmetric.md) collection</span></span>|<span data-ttu-id="ed4bc-144">Os valores métricos para a categoria de análise de experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="ed4bc-144">The metric values for the user experience analytics category.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ed4bc-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ed4bc-145">JSON Representation</span></span>
<span data-ttu-id="ed4bc-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ed4bc-146">Here is a JSON representation of the resource.</span></span>
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
  "totalDevices": 1024,
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




