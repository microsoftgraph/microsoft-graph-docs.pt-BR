---
title: tipo de recurso userExperienceAnalyticsInsight
description: A visão geral da análise da experiência do usuário é a recomendação de melhorar a pontuação de análise da experiência do usuário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b9e9e40916e92dd45726fb5bc04387f180bf8395
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528465"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a><span data-ttu-id="1df3d-103">tipo de recurso userExperienceAnalyticsInsight</span><span class="sxs-lookup"><span data-stu-id="1df3d-103">userExperienceAnalyticsInsight resource type</span></span>

<span data-ttu-id="1df3d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1df3d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1df3d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1df3d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1df3d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1df3d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1df3d-107">A visão geral da análise da experiência do usuário é a recomendação de melhorar a pontuação de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="1df3d-107">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="1df3d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1df3d-108">Properties</span></span>
|<span data-ttu-id="1df3d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1df3d-109">Property</span></span>|<span data-ttu-id="1df3d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1df3d-110">Type</span></span>|<span data-ttu-id="1df3d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1df3d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1df3d-112">userExperienceAnalyticsMetricId</span><span class="sxs-lookup"><span data-stu-id="1df3d-112">userExperienceAnalyticsMetricId</span></span>|<span data-ttu-id="1df3d-113">String</span><span class="sxs-lookup"><span data-stu-id="1df3d-113">String</span></span>|<span data-ttu-id="1df3d-114">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="1df3d-114">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="1df3d-115">insightid</span><span class="sxs-lookup"><span data-stu-id="1df3d-115">insightId</span></span>|<span data-ttu-id="1df3d-116">String</span><span class="sxs-lookup"><span data-stu-id="1df3d-116">String</span></span>|<span data-ttu-id="1df3d-117">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="1df3d-117">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="1df3d-118">values</span><span class="sxs-lookup"><span data-stu-id="1df3d-118">values</span></span>|<span data-ttu-id="1df3d-119">coleção [userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)</span><span class="sxs-lookup"><span data-stu-id="1df3d-119">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md) collection</span></span>|<span data-ttu-id="1df3d-120">O valor da visão da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="1df3d-120">The value of the user experience analytics insight.</span></span>|
|<span data-ttu-id="1df3d-121">severity</span><span class="sxs-lookup"><span data-stu-id="1df3d-121">severity</span></span>|[<span data-ttu-id="1df3d-122">userExperienceAnalyticsInsightSeverity</span><span class="sxs-lookup"><span data-stu-id="1df3d-122">userExperienceAnalyticsInsightSeverity</span></span>](../resources/intune-devices-userexperienceanalyticsinsightseverity.md)|<span data-ttu-id="1df3d-123">O valor da visão da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="1df3d-123">The value of the user experience analytics insight.</span></span> <span data-ttu-id="1df3d-124">Os valores possíveis são: `none`, `informational`, `warning`, `error`.</span><span class="sxs-lookup"><span data-stu-id="1df3d-124">Possible values are: `none`, `informational`, `warning`, `error`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1df3d-125">Relações</span><span class="sxs-lookup"><span data-stu-id="1df3d-125">Relationships</span></span>
<span data-ttu-id="1df3d-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1df3d-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1df3d-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1df3d-127">JSON Representation</span></span>
<span data-ttu-id="1df3d-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1df3d-128">Here is a JSON representation of the resource.</span></span>
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



