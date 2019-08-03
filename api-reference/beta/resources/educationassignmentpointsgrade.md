---
title: tipo de recurso educationAssignmentPointsGrade
description: Quando uma atribuição é definida como um tipo de grade de pontos, cada envio terá esse objeto associado à propriedade enmisse **.** Isso cria uma subclasse de educationAssignmentGrade,
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5476d84e156ae0294fc3502d6de6d808644574c7
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173073"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="9c926-104">tipo de recurso educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="9c926-104">educationAssignmentPointsGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c926-105">Quando uma atribuição é definida como um tipo de grade de pontos, cada envio terá esse objeto associado à propriedade enmisse **.**</span><span class="sxs-lookup"><span data-stu-id="9c926-105">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="9c926-106">Isso cria uma subclasse de [educationAssignmentGrade](educationassignmentgrade.md), que adicionará os dados de quem a essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="9c926-106">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="9c926-107">O máximo de pontos é armazenado na propriedade **assignments. Grading** .</span><span class="sxs-lookup"><span data-stu-id="9c926-107">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="9c926-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c926-108">Properties</span></span>
| <span data-ttu-id="9c926-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c926-109">Property</span></span>     | <span data-ttu-id="9c926-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c926-110">Type</span></span>   |<span data-ttu-id="9c926-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c926-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c926-112">points</span><span class="sxs-lookup"><span data-stu-id="9c926-112">points</span></span>|<span data-ttu-id="9c926-113">Único</span><span class="sxs-lookup"><span data-stu-id="9c926-113">Single</span></span>|<span data-ttu-id="9c926-114">Número de pontos que um professor está dando este objeto de envio.</span><span class="sxs-lookup"><span data-stu-id="9c926-114">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c926-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c926-115">JSON representation</span></span>

<span data-ttu-id="9c926-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c926-116">The following is a JSON representation of the resource.</span></span>

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
