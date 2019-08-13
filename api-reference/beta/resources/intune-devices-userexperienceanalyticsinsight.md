---
title: tipo de recurso userExperienceAnalyticsInsight
description: A visão geral da análise da experiência do usuário é a recomendação de melhorar a pontuação de análise da experiência do usuário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 36277b147e7eabc6f28aef3877538ebbc429f381
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36341210"
---
# <a name="userexperienceanalyticsinsight-resource-type"></a><span data-ttu-id="837fd-103">tipo de recurso userExperienceAnalyticsInsight</span><span class="sxs-lookup"><span data-stu-id="837fd-103">userExperienceAnalyticsInsight resource type</span></span>

> <span data-ttu-id="837fd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="837fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="837fd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="837fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="837fd-106">A visão geral da análise da experiência do usuário é a recomendação de melhorar a pontuação de análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="837fd-106">The user experience analytics insight is the recomendation to improve the user experience analytics score.</span></span>

## <a name="properties"></a><span data-ttu-id="837fd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="837fd-107">Properties</span></span>
|<span data-ttu-id="837fd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="837fd-108">Property</span></span>|<span data-ttu-id="837fd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="837fd-109">Type</span></span>|<span data-ttu-id="837fd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="837fd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="837fd-111">userExperienceAnalyticsMetricId</span><span class="sxs-lookup"><span data-stu-id="837fd-111">userExperienceAnalyticsMetricId</span></span>|<span data-ttu-id="837fd-112">String</span><span class="sxs-lookup"><span data-stu-id="837fd-112">String</span></span>|<span data-ttu-id="837fd-113">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="837fd-113">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="837fd-114">insightid</span><span class="sxs-lookup"><span data-stu-id="837fd-114">insightId</span></span>|<span data-ttu-id="837fd-115">String</span><span class="sxs-lookup"><span data-stu-id="837fd-115">String</span></span>|<span data-ttu-id="837fd-116">O identificador exclusivo da visão geral da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="837fd-116">The unique identifier of the user experience analytics insight.</span></span>|
|<span data-ttu-id="837fd-117">valor</span><span class="sxs-lookup"><span data-stu-id="837fd-117">value</span></span>|<span data-ttu-id="837fd-118">coleção [userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md)</span><span class="sxs-lookup"><span data-stu-id="837fd-118">[userExperienceAnalyticsInsightValue](../resources/intune-devices-userexperienceanalyticsinsightvalue.md) collection</span></span>|<span data-ttu-id="837fd-119">O valor da visão da análise da experiência do usuário.</span><span class="sxs-lookup"><span data-stu-id="837fd-119">The value of the user experience analytics insight.</span></span>|

## <a name="relationships"></a><span data-ttu-id="837fd-120">Relações</span><span class="sxs-lookup"><span data-stu-id="837fd-120">Relationships</span></span>
<span data-ttu-id="837fd-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="837fd-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="837fd-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="837fd-122">JSON Representation</span></span>
<span data-ttu-id="837fd-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="837fd-123">Here is a JSON representation of the resource.</span></span>
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
  "value": [
    {
      "@odata.type": "microsoft.graph.insightValueDouble"
    }
  ]
}
```



