---
title: tipo de recurso userExperienceAnalyticsInsight
description: A visão geral da análise da experiência do usuário é a recomendação de melhorar a pontuação de análise da experiência do usuário.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c28df3bc40f02948198a67850de6fd573607a366
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783792"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a><span data-ttu-id="eca84-103">tipo de recurso userExperienceAnalyticsInsight</span><span class="sxs-lookup"><span data-stu-id="eca84-103">userExperienceAnalyticsInsight resource type</span></span>

> <span data-ttu-id="eca84-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eca84-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eca84-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eca84-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eca84-106">A visão geral da análise da experiência do usuário é a recomendação de melhorar a pontuação de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="eca84-106">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="eca84-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eca84-107">Properties</span></span>
|<span data-ttu-id="eca84-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eca84-108">Property</span></span>|<span data-ttu-id="eca84-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="eca84-109">Type</span></span>|<span data-ttu-id="eca84-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="eca84-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eca84-111">userExperienceAnalyticsMetricId</span><span class="sxs-lookup"><span data-stu-id="eca84-111">userExperienceAnalyticsMetricId</span></span>|<span data-ttu-id="eca84-112">String</span><span class="sxs-lookup"><span data-stu-id="eca84-112">String</span></span>|<span data-ttu-id="eca84-113">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="eca84-113">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="eca84-114">insightid</span><span class="sxs-lookup"><span data-stu-id="eca84-114">insightId</span></span>|<span data-ttu-id="eca84-115">String</span><span class="sxs-lookup"><span data-stu-id="eca84-115">String</span></span>|<span data-ttu-id="eca84-116">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="eca84-116">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="eca84-117">values</span><span class="sxs-lookup"><span data-stu-id="eca84-117">values</span></span>|<span data-ttu-id="eca84-118">coleção [userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)</span><span class="sxs-lookup"><span data-stu-id="eca84-118">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md) collection</span></span>|<span data-ttu-id="eca84-119">O valor da visão da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="eca84-119">The value of the user experience analytics insight.</span></span>|
|<span data-ttu-id="eca84-120">severity</span><span class="sxs-lookup"><span data-stu-id="eca84-120">severity</span></span>|[<span data-ttu-id="eca84-121">userExperienceAnalyticsInsightSeverity</span><span class="sxs-lookup"><span data-stu-id="eca84-121">userExperienceAnalyticsInsightSeverity</span></span>](../resources/intune-devices-userexperienceanalyticsinsightseverity.md)|<span data-ttu-id="eca84-122">O valor da visão da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="eca84-122">The value of the user experience analytics insight.</span></span> <span data-ttu-id="eca84-123">Os valores possíveis são: `none`, `informational`, `warning`, `error`.</span><span class="sxs-lookup"><span data-stu-id="eca84-123">Possible values are: `none`, `informational`, `warning`, `error`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eca84-124">Relações</span><span class="sxs-lookup"><span data-stu-id="eca84-124">Relationships</span></span>
<span data-ttu-id="eca84-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eca84-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eca84-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eca84-126">JSON Representation</span></span>
<span data-ttu-id="eca84-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eca84-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsInsight",
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
```



