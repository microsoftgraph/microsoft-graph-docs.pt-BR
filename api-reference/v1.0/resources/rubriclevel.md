---
title: Tipo de recurso rubricLevel
description: Um nível de rubric.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b4cbd952d8c5bed366d6cfbbda5920d7eddba97d
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911376"
---
# <a name="rubriclevel-resource-type"></a><span data-ttu-id="6c3e6-103">Tipo de recurso rubricLevel</span><span class="sxs-lookup"><span data-stu-id="6c3e6-103">rubricLevel resource type</span></span>

<span data-ttu-id="6c3e6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c3e6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c3e6-105">Um nível de rubric.</span><span class="sxs-lookup"><span data-stu-id="6c3e6-105">A level of a rubric.</span></span> 

<span data-ttu-id="6c3e6-106">Consulte [educationRubric](educationrubric.md) para ver uma descrição da relação entre as qualidades *rubricas,* níveis e *critérios.*</span><span class="sxs-lookup"><span data-stu-id="6c3e6-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="6c3e6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c3e6-107">Properties</span></span>

| <span data-ttu-id="6c3e6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c3e6-108">Property</span></span>     | <span data-ttu-id="6c3e6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c3e6-109">Type</span></span>        | <span data-ttu-id="6c3e6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c3e6-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6c3e6-111">description</span><span class="sxs-lookup"><span data-stu-id="6c3e6-111">description</span></span>|[<span data-ttu-id="6c3e6-112">itemBody</span><span class="sxs-lookup"><span data-stu-id="6c3e6-112">itemBody</span></span>](itembody.md)|<span data-ttu-id="6c3e6-113">A descrição desse nível rubrico.</span><span class="sxs-lookup"><span data-stu-id="6c3e6-113">The description of this rubric level.</span></span>|
|<span data-ttu-id="6c3e6-114">displayName</span><span class="sxs-lookup"><span data-stu-id="6c3e6-114">displayName</span></span>|<span data-ttu-id="6c3e6-115">String</span><span class="sxs-lookup"><span data-stu-id="6c3e6-115">String</span></span>|<span data-ttu-id="6c3e6-116">O nome desse nível rubrico.</span><span class="sxs-lookup"><span data-stu-id="6c3e6-116">The name of this rubric level.</span></span>|
|<span data-ttu-id="6c3e6-117">grading</span><span class="sxs-lookup"><span data-stu-id="6c3e6-117">grading</span></span>|[<span data-ttu-id="6c3e6-118">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="6c3e6-118">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="6c3e6-119">Null se for uma rubrica sem pontos; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) se for uma rubrica de pontos.</span><span class="sxs-lookup"><span data-stu-id="6c3e6-119">Null if this is a no-points rubric; [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) if it is a points rubric.</span></span>|
|<span data-ttu-id="6c3e6-120">levelId</span><span class="sxs-lookup"><span data-stu-id="6c3e6-120">levelId</span></span>|<span data-ttu-id="6c3e6-121">String</span><span class="sxs-lookup"><span data-stu-id="6c3e6-121">String</span></span>|<span data-ttu-id="6c3e6-122">A ID desse recurso.</span><span class="sxs-lookup"><span data-stu-id="6c3e6-122">The ID of this resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c3e6-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c3e6-123">JSON representation</span></span>

<span data-ttu-id="6c3e6-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c3e6-124">The following is a JSON representation of the resource.</span></span>

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

