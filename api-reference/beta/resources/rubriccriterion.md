---
title: tipo de recurso rubricCriterion
description: Um critério de um amostra rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e1a2a0550a7e1f9f5865b8381b3f730d31cac6b6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521016"
---
# <a name="rubriccriterion-resource-type"></a><span data-ttu-id="4b78d-103">tipo de recurso rubricCriterion</span><span class="sxs-lookup"><span data-stu-id="4b78d-103">rubricCriterion resource type</span></span>

<span data-ttu-id="4b78d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4b78d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b78d-105">Um critério de um amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="4b78d-105">A criterion of a rubric.</span></span> <span data-ttu-id="4b78d-106">Consulte [educationRubric](educationrubric.md) para obter uma descrição da relação entre as *qualidades*, *níveis*e *critérios*do amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="4b78d-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="4b78d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4b78d-107">Properties</span></span>

| <span data-ttu-id="4b78d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4b78d-108">Property</span></span>     | <span data-ttu-id="4b78d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4b78d-109">Type</span></span>        | <span data-ttu-id="4b78d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4b78d-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4b78d-111">description</span><span class="sxs-lookup"><span data-stu-id="4b78d-111">description</span></span>|[<span data-ttu-id="4b78d-112">itemBody</span><span class="sxs-lookup"><span data-stu-id="4b78d-112">itemBody</span></span>](itembody.md)|<span data-ttu-id="4b78d-113">A descrição desse critério.</span><span class="sxs-lookup"><span data-stu-id="4b78d-113">The description of this criterion.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b78d-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4b78d-114">JSON representation</span></span>

<span data-ttu-id="4b78d-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4b78d-115">The following is a JSON representation of the resource.</span></span>

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