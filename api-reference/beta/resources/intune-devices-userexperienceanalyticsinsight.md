---
title: tipo de recurso userExperienceAnalyticsInsight
description: A visão geral da análise da experiência do usuário é a recomendação de melhorar a pontuação de análise da experiência do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d000afacb82365e06c5728dd8eedc2e6eb4217dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080891"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a><span data-ttu-id="84e7e-103">tipo de recurso userExperienceAnalyticsInsight</span><span class="sxs-lookup"><span data-stu-id="84e7e-103">userExperienceAnalyticsInsight resource type</span></span>

<span data-ttu-id="84e7e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84e7e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84e7e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="84e7e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84e7e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="84e7e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84e7e-107">A visão geral da análise da experiência do usuário é a recomendação de melhorar a pontuação de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="84e7e-107">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="84e7e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="84e7e-108">Properties</span></span>
|<span data-ttu-id="84e7e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="84e7e-109">Property</span></span>|<span data-ttu-id="84e7e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="84e7e-110">Type</span></span>|<span data-ttu-id="84e7e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="84e7e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84e7e-112">userExperienceAnalyticsMetricId</span><span class="sxs-lookup"><span data-stu-id="84e7e-112">userExperienceAnalyticsMetricId</span></span>|<span data-ttu-id="84e7e-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84e7e-113">String</span></span>|<span data-ttu-id="84e7e-114">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="84e7e-114">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="84e7e-115">insightid</span><span class="sxs-lookup"><span data-stu-id="84e7e-115">insightId</span></span>|<span data-ttu-id="84e7e-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="84e7e-116">String</span></span>|<span data-ttu-id="84e7e-117">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="84e7e-117">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="84e7e-118">values</span><span class="sxs-lookup"><span data-stu-id="84e7e-118">values</span></span>|<span data-ttu-id="84e7e-119">coleção [userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)</span><span class="sxs-lookup"><span data-stu-id="84e7e-119">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md) collection</span></span>|<span data-ttu-id="84e7e-120">O valor da visão da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="84e7e-120">The value of the user experience analytics insight.</span></span>|
|<span data-ttu-id="84e7e-121">severity</span><span class="sxs-lookup"><span data-stu-id="84e7e-121">severity</span></span>|[<span data-ttu-id="84e7e-122">userExperienceAnalyticsInsightSeverity</span><span class="sxs-lookup"><span data-stu-id="84e7e-122">userExperienceAnalyticsInsightSeverity</span></span>](../resources/intune-devices-userexperienceanalyticsinsightseverity.md)|<span data-ttu-id="84e7e-123">O valor da visão da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="84e7e-123">The value of the user experience analytics insight.</span></span> <span data-ttu-id="84e7e-124">Os valores possíveis são: `none`, `informational`, `warning`, `error`.</span><span class="sxs-lookup"><span data-stu-id="84e7e-124">Possible values are: `none`, `informational`, `warning`, `error`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84e7e-125">Relações</span><span class="sxs-lookup"><span data-stu-id="84e7e-125">Relationships</span></span>
<span data-ttu-id="84e7e-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="84e7e-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84e7e-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="84e7e-127">JSON Representation</span></span>
<span data-ttu-id="84e7e-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="84e7e-128">Here is a JSON representation of the resource.</span></span>
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
      "value": "4.2"
    }
  ],
  "severity": "String"
}
```






