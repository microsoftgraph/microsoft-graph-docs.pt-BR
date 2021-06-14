---
title: Tipo de recurso educationAssignmentPointsGrade
description: Quando uma atribuição é definida como um tipo de grau de pontos, cada envio terá esse objeto associado à **propriedade submission.grade.**
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b624bd0e82336e4e416641240e072c8b4ac6392d
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912182"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="b0aec-103">Tipo de recurso educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="b0aec-103">educationAssignmentPointsGrade resource type</span></span>

<span data-ttu-id="b0aec-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0aec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b0aec-105">Quando uma atribuição é definida como um tipo de grau de pontos, cada envio terá esse objeto associado à **propriedade submission.grade.**</span><span class="sxs-lookup"><span data-stu-id="b0aec-105">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="b0aec-106">Isso cria uma subclasse [de educationAssignmentGrade](educationassignmentgrade.md), que adicionará os dados de quem a essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="b0aec-106">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="b0aec-107">Os pontos máximos são armazenados na **propriedade assignments.grading.**</span><span class="sxs-lookup"><span data-stu-id="b0aec-107">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="b0aec-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0aec-108">Properties</span></span>
| <span data-ttu-id="b0aec-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0aec-109">Property</span></span>     | <span data-ttu-id="b0aec-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0aec-110">Type</span></span>   |<span data-ttu-id="b0aec-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0aec-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b0aec-112">points</span><span class="sxs-lookup"><span data-stu-id="b0aec-112">points</span></span>|<span data-ttu-id="b0aec-113">Único</span><span class="sxs-lookup"><span data-stu-id="b0aec-113">Single</span></span>|<span data-ttu-id="b0aec-114">Número de pontos que um professor está dando a esse objeto de envio.</span><span class="sxs-lookup"><span data-stu-id="b0aec-114">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b0aec-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0aec-115">JSON representation</span></span>

<span data-ttu-id="b0aec-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0aec-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}-->

```json
{
  "points": "Double"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


