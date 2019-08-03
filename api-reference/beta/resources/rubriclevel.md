---
title: tipo de recurso rubricLevel
description: Um nível de um amostra rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: dd8e67cbf4ba8994e03d683665928f9e62608d8e
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173332"
---
# <a name="rubriclevel-resource-type"></a><span data-ttu-id="df3e4-103">tipo de recurso rubricLevel</span><span class="sxs-lookup"><span data-stu-id="df3e4-103">rubricLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df3e4-104">Um nível de um amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="df3e4-104">A level of a rubric.</span></span> <span data-ttu-id="df3e4-105">Consulte [educationRubric](educationrubric.md) para obter uma descrição da relação entre as *qualidades*, *níveis*e *critérios*do amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="df3e4-105">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="df3e4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df3e4-106">Properties</span></span>

| <span data-ttu-id="df3e4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df3e4-107">Property</span></span>     | <span data-ttu-id="df3e4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="df3e4-108">Type</span></span>        | <span data-ttu-id="df3e4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="df3e4-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="df3e4-110">description</span><span class="sxs-lookup"><span data-stu-id="df3e4-110">description</span></span>|[<span data-ttu-id="df3e4-111">itemBody</span><span class="sxs-lookup"><span data-stu-id="df3e4-111">itemBody</span></span>](itembody.md)|<span data-ttu-id="df3e4-112">A descrição desse nível de amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="df3e4-112">The description of this rubric level.</span></span>|
|<span data-ttu-id="df3e4-113">displayName</span><span class="sxs-lookup"><span data-stu-id="df3e4-113">displayName</span></span>|<span data-ttu-id="df3e4-114">String</span><span class="sxs-lookup"><span data-stu-id="df3e4-114">String</span></span>|<span data-ttu-id="df3e4-115">O nome desse nível de amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="df3e4-115">The name of this rubric level.</span></span>|
|<span data-ttu-id="df3e4-116">notas</span><span class="sxs-lookup"><span data-stu-id="df3e4-116">grading</span></span>|[<span data-ttu-id="df3e4-117">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="df3e4-117">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="df3e4-118">NULL se for um amostra rubric sem pontos; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) se for um ponto amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="df3e4-118">Null if this is a no-points rubric; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) if it is a points rubric.</span></span>|
|<span data-ttu-id="df3e4-119">levelid</span><span class="sxs-lookup"><span data-stu-id="df3e4-119">levelId</span></span>|<span data-ttu-id="df3e4-120">String</span><span class="sxs-lookup"><span data-stu-id="df3e4-120">String</span></span>|<span data-ttu-id="df3e4-121">A ID desse recurso.</span><span class="sxs-lookup"><span data-stu-id="df3e4-121">The ID of this resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="df3e4-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df3e4-122">JSON representation</span></span>

<span data-ttu-id="df3e4-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df3e4-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricLevel",
  "baseType": null
}-->

```json
{
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "levelId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->