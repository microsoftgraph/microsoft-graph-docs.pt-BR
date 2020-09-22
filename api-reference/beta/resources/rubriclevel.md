---
title: tipo de recurso rubricLevel
description: Um nível de um amostra rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 14a7c084aad907ce2e5f90b06f17b64aca9c331e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016091"
---
# <a name="rubriclevel-resource-type"></a><span data-ttu-id="c9b16-103">tipo de recurso rubricLevel</span><span class="sxs-lookup"><span data-stu-id="c9b16-103">rubricLevel resource type</span></span>

<span data-ttu-id="c9b16-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9b16-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9b16-105">Um nível de um amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="c9b16-105">A level of a rubric.</span></span> <span data-ttu-id="c9b16-106">Consulte [educationRubric](educationrubric.md) para obter uma descrição da relação entre as *qualidades*, *níveis*e *critérios*do amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="c9b16-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="c9b16-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9b16-107">Properties</span></span>

| <span data-ttu-id="c9b16-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9b16-108">Property</span></span>     | <span data-ttu-id="c9b16-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9b16-109">Type</span></span>        | <span data-ttu-id="c9b16-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9b16-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c9b16-111">description</span><span class="sxs-lookup"><span data-stu-id="c9b16-111">description</span></span>|[<span data-ttu-id="c9b16-112">itemBody</span><span class="sxs-lookup"><span data-stu-id="c9b16-112">itemBody</span></span>](itembody.md)|<span data-ttu-id="c9b16-113">A descrição desse nível de amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="c9b16-113">The description of this rubric level.</span></span>|
|<span data-ttu-id="c9b16-114">displayName</span><span class="sxs-lookup"><span data-stu-id="c9b16-114">displayName</span></span>|<span data-ttu-id="c9b16-115">String</span><span class="sxs-lookup"><span data-stu-id="c9b16-115">String</span></span>|<span data-ttu-id="c9b16-116">O nome desse nível de amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="c9b16-116">The name of this rubric level.</span></span>|
|<span data-ttu-id="c9b16-117">notas</span><span class="sxs-lookup"><span data-stu-id="c9b16-117">grading</span></span>|[<span data-ttu-id="c9b16-118">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="c9b16-118">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="c9b16-119">NULL se for um amostra rubric sem pontos; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) se for um ponto amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="c9b16-119">Null if this is a no-points rubric; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) if it is a points rubric.</span></span>|
|<span data-ttu-id="c9b16-120">levelid</span><span class="sxs-lookup"><span data-stu-id="c9b16-120">levelId</span></span>|<span data-ttu-id="c9b16-121">String</span><span class="sxs-lookup"><span data-stu-id="c9b16-121">String</span></span>|<span data-ttu-id="c9b16-122">A ID desse recurso.</span><span class="sxs-lookup"><span data-stu-id="c9b16-122">The ID of this resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9b16-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9b16-123">JSON representation</span></span>

<span data-ttu-id="c9b16-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c9b16-124">The following is a JSON representation of the resource.</span></span>

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

