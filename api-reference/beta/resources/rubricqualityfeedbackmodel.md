---
title: tipo de recurso rubricQualityFeedbackModel
description: Comentários relacionados a uma qualidade específica de um educationRubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 56fea149446c79dd95e50e1b5d152cc8610dc0dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016062"
---
# <a name="rubricqualityfeedbackmodel-resource-type"></a><span data-ttu-id="dbacb-103">tipo de recurso rubricQualityFeedbackModel</span><span class="sxs-lookup"><span data-stu-id="dbacb-103">rubricQualityFeedbackModel resource type</span></span>

<span data-ttu-id="dbacb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbacb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbacb-105">Comentários relacionados a uma [qualidade](rubricquality.md) específica de um [educationRubric](educationrubric.md).</span><span class="sxs-lookup"><span data-stu-id="dbacb-105">Feedback related to a specific [quality](rubricquality.md) of an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dbacb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dbacb-106">Properties</span></span>

| <span data-ttu-id="dbacb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbacb-107">Property</span></span>     | <span data-ttu-id="dbacb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbacb-108">Type</span></span>        | <span data-ttu-id="dbacb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbacb-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dbacb-110">comentários</span><span class="sxs-lookup"><span data-stu-id="dbacb-110">feedback</span></span>|[<span data-ttu-id="dbacb-111">itemBody</span><span class="sxs-lookup"><span data-stu-id="dbacb-111">itemBody</span></span>](itembody.md)|<span data-ttu-id="dbacb-112">Comentários específicos para uma qualidade desse amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="dbacb-112">Specific feedback for one quality of this rubric.</span></span>|
|<span data-ttu-id="dbacb-113">qualityid</span><span class="sxs-lookup"><span data-stu-id="dbacb-113">qualityId</span></span>|<span data-ttu-id="dbacb-114">String</span><span class="sxs-lookup"><span data-stu-id="dbacb-114">String</span></span>|<span data-ttu-id="dbacb-115">A ID do [rubricQuality](rubricquality.md) ao qual este comentário está relacionado.</span><span class="sxs-lookup"><span data-stu-id="dbacb-115">The ID of the [rubricQuality](rubricquality.md) that this feedback is related to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dbacb-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dbacb-116">JSON representation</span></span>

<span data-ttu-id="dbacb-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dbacb-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQualityFeedbackModel",
  "baseType": null
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.itemBody"},
  "qualityId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQualityFeedbackModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

