---
title: tipo de recurso rubricCriterion
description: Um critério de um amostra rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 250132ab5304ab9df94707349df951e5b1e995a6
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173339"
---
# <a name="rubriccriterion-resource-type"></a><span data-ttu-id="c1a10-103">tipo de recurso rubricCriterion</span><span class="sxs-lookup"><span data-stu-id="c1a10-103">rubricCriterion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1a10-104">Um critério de um amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="c1a10-104">A criterion of a rubric.</span></span> <span data-ttu-id="c1a10-105">Consulte [educationRubric](educationrubric.md) para obter uma descrição da relação entre as *qualidades*, *níveis*e *critérios*do amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="c1a10-105">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="c1a10-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1a10-106">Properties</span></span>

| <span data-ttu-id="c1a10-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1a10-107">Property</span></span>     | <span data-ttu-id="c1a10-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1a10-108">Type</span></span>        | <span data-ttu-id="c1a10-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1a10-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c1a10-110">description</span><span class="sxs-lookup"><span data-stu-id="c1a10-110">description</span></span>|[<span data-ttu-id="c1a10-111">itemBody</span><span class="sxs-lookup"><span data-stu-id="c1a10-111">itemBody</span></span>](itembody.md)|<span data-ttu-id="c1a10-112">A descrição desse critério.</span><span class="sxs-lookup"><span data-stu-id="c1a10-112">The description of this criterion.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c1a10-113">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1a10-113">JSON representation</span></span>

<span data-ttu-id="c1a10-114">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1a10-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricCriterion",
  "baseType": null
}-->

```json
{
  "description": {"@odata.type": "microsoft.graph.itemBody"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricCriterion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->