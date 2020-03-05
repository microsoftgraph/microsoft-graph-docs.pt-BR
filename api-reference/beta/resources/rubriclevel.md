---
title: tipo de recurso rubricLevel
description: Um nível de um amostra rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 24af9e9be6dc9b63934a02193958e0267dde8dea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521009"
---
# <a name="rubriclevel-resource-type"></a><span data-ttu-id="fda62-103">tipo de recurso rubricLevel</span><span class="sxs-lookup"><span data-stu-id="fda62-103">rubricLevel resource type</span></span>

<span data-ttu-id="fda62-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fda62-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fda62-105">Um nível de um amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="fda62-105">A level of a rubric.</span></span> <span data-ttu-id="fda62-106">Consulte [educationRubric](educationrubric.md) para obter uma descrição da relação entre as *qualidades*, *níveis*e *critérios*do amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="fda62-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="fda62-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fda62-107">Properties</span></span>

| <span data-ttu-id="fda62-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fda62-108">Property</span></span>     | <span data-ttu-id="fda62-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="fda62-109">Type</span></span>        | <span data-ttu-id="fda62-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="fda62-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fda62-111">description</span><span class="sxs-lookup"><span data-stu-id="fda62-111">description</span></span>|[<span data-ttu-id="fda62-112">itemBody</span><span class="sxs-lookup"><span data-stu-id="fda62-112">itemBody</span></span>](itembody.md)|<span data-ttu-id="fda62-113">A descrição desse nível de amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="fda62-113">The description of this rubric level.</span></span>|
|<span data-ttu-id="fda62-114">displayName</span><span class="sxs-lookup"><span data-stu-id="fda62-114">displayName</span></span>|<span data-ttu-id="fda62-115">String</span><span class="sxs-lookup"><span data-stu-id="fda62-115">String</span></span>|<span data-ttu-id="fda62-116">O nome desse nível de amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="fda62-116">The name of this rubric level.</span></span>|
|<span data-ttu-id="fda62-117">notas</span><span class="sxs-lookup"><span data-stu-id="fda62-117">grading</span></span>|[<span data-ttu-id="fda62-118">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="fda62-118">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="fda62-119">NULL se for um amostra rubric sem pontos; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) se for um ponto amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="fda62-119">Null if this is a no-points rubric; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) if it is a points rubric.</span></span>|
|<span data-ttu-id="fda62-120">levelid</span><span class="sxs-lookup"><span data-stu-id="fda62-120">levelId</span></span>|<span data-ttu-id="fda62-121">String</span><span class="sxs-lookup"><span data-stu-id="fda62-121">String</span></span>|<span data-ttu-id="fda62-122">A ID desse recurso.</span><span class="sxs-lookup"><span data-stu-id="fda62-122">The ID of this resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fda62-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fda62-123">JSON representation</span></span>

<span data-ttu-id="fda62-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fda62-124">The following is a JSON representation of the resource.</span></span>

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