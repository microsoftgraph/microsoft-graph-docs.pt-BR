---
title: tipo de recurso userExperienceAnalyticsInsight
description: A visão geral da análise da experiência do usuário é a recomendação de melhorar a pontuação de análise da experiência do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d624863a07309b3962122fb93a1ebbaea895a44b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49226383"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a><span data-ttu-id="42666-103">tipo de recurso userExperienceAnalyticsInsight</span><span class="sxs-lookup"><span data-stu-id="42666-103">userExperienceAnalyticsInsight resource type</span></span>

<span data-ttu-id="42666-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42666-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42666-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="42666-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42666-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42666-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42666-107">A visão geral da análise da experiência do usuário é a recomendação de melhorar a pontuação de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="42666-107">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="42666-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42666-108">Properties</span></span>
|<span data-ttu-id="42666-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42666-109">Property</span></span>|<span data-ttu-id="42666-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="42666-110">Type</span></span>|<span data-ttu-id="42666-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="42666-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42666-112">userExperienceAnalyticsMetricId</span><span class="sxs-lookup"><span data-stu-id="42666-112">userExperienceAnalyticsMetricId</span></span>|<span data-ttu-id="42666-113">String</span><span class="sxs-lookup"><span data-stu-id="42666-113">String</span></span>|<span data-ttu-id="42666-114">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="42666-114">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="42666-115">insightid</span><span class="sxs-lookup"><span data-stu-id="42666-115">insightId</span></span>|<span data-ttu-id="42666-116">String</span><span class="sxs-lookup"><span data-stu-id="42666-116">String</span></span>|<span data-ttu-id="42666-117">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="42666-117">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="42666-118">values</span><span class="sxs-lookup"><span data-stu-id="42666-118">values</span></span>|<span data-ttu-id="42666-119">coleção [userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)</span><span class="sxs-lookup"><span data-stu-id="42666-119">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md) collection</span></span>|<span data-ttu-id="42666-120">O valor da visão da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="42666-120">The value of the user experience analytics insight.</span></span>|
|<span data-ttu-id="42666-121">severity</span><span class="sxs-lookup"><span data-stu-id="42666-121">severity</span></span>|[<span data-ttu-id="42666-122">userExperienceAnalyticsInsightSeverity</span><span class="sxs-lookup"><span data-stu-id="42666-122">userExperienceAnalyticsInsightSeverity</span></span>](../resources/intune-devices-userexperienceanalyticsinsightseverity.md)|<span data-ttu-id="42666-123">O valor da visão da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="42666-123">The value of the user experience analytics insight.</span></span> <span data-ttu-id="42666-124">Os valores possíveis são: `none`, `informational`, `warning`, `error`.</span><span class="sxs-lookup"><span data-stu-id="42666-124">Possible values are: `none`, `informational`, `warning`, `error`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42666-125">Relações</span><span class="sxs-lookup"><span data-stu-id="42666-125">Relationships</span></span>
<span data-ttu-id="42666-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="42666-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42666-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42666-127">JSON Representation</span></span>
<span data-ttu-id="42666-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42666-128">Here is a JSON representation of the resource.</span></span>
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




