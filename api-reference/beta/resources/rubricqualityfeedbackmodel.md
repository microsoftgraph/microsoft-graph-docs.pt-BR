---
title: tipo de recurso rubricQualityFeedbackModel
description: Comentários relacionados a uma qualidade específica de um educationRubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 0a7c2b80a2cef18b50157ae9a54c66d35822fa51
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173297"
---
# <a name="rubricqualityfeedbackmodel-resource-type"></a><span data-ttu-id="ab956-103">tipo de recurso rubricQualityFeedbackModel</span><span class="sxs-lookup"><span data-stu-id="ab956-103">rubricQualityFeedbackModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab956-104">Comentários relacionados a uma [qualidade](rubricquality.md) específica de um [educationRubric](educationrubric.md).</span><span class="sxs-lookup"><span data-stu-id="ab956-104">Feedback related to a specific [quality](rubricquality.md) of an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ab956-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab956-105">Properties</span></span>

| <span data-ttu-id="ab956-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab956-106">Property</span></span>     | <span data-ttu-id="ab956-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab956-107">Type</span></span>        | <span data-ttu-id="ab956-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab956-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ab956-109">comentários</span><span class="sxs-lookup"><span data-stu-id="ab956-109">feedback</span></span>|[<span data-ttu-id="ab956-110">itemBody</span><span class="sxs-lookup"><span data-stu-id="ab956-110">itemBody</span></span>](itembody.md)|<span data-ttu-id="ab956-111">Comentários específicos para uma qualidade desse amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="ab956-111">Specific feedback for one quality of this rubric.</span></span>|
|<span data-ttu-id="ab956-112">qualityid</span><span class="sxs-lookup"><span data-stu-id="ab956-112">qualityId</span></span>|<span data-ttu-id="ab956-113">String</span><span class="sxs-lookup"><span data-stu-id="ab956-113">String</span></span>|<span data-ttu-id="ab956-114">A ID do [rubricQuality](rubricquality.md) ao qual este comentário está relacionado.</span><span class="sxs-lookup"><span data-stu-id="ab956-114">The ID of the [rubricQuality](rubricquality.md) that this feedback is related to.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab956-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab956-115">JSON representation</span></span>

<span data-ttu-id="ab956-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab956-116">The following is a JSON representation of the resource.</span></span>

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