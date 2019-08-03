---
title: tipo de recurso educationAssignmentPointsGradeType
description: Usada com a propriedade **assignments. Grading** . Esta é uma subclasse de educationAssignmentGradeType.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ef866debcf2c70862aae30048f68bd026c4e5250
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172790"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="21ec1-104">tipo de recurso educationAssignmentPointsGradeType</span><span class="sxs-lookup"><span data-stu-id="21ec1-104">educationAssignmentPointsGradeType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21ec1-105">Usada com a propriedade **assignments. Grading** .</span><span class="sxs-lookup"><span data-stu-id="21ec1-105">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="21ec1-106">Esta é uma subclasse de [educationAssignmentGradeType](educationassignmentgradetype.md).</span><span class="sxs-lookup"><span data-stu-id="21ec1-106">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="21ec1-107">Isso indica que a atribuição foi classificada e armazena o número máximo de pontos que cada aluno pode obter nesse item de trabalho.</span><span class="sxs-lookup"><span data-stu-id="21ec1-107">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="21ec1-108">Quando isso é definido em uma atribuição, cada envio receberá uma propriedade [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) associada ao armazenamento dos pontos de cada aluno.</span><span class="sxs-lookup"><span data-stu-id="21ec1-108">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="21ec1-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21ec1-109">Properties</span></span>
| <span data-ttu-id="21ec1-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21ec1-110">Property</span></span>     | <span data-ttu-id="21ec1-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="21ec1-111">Type</span></span>   |<span data-ttu-id="21ec1-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="21ec1-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21ec1-113">maxPoints</span><span class="sxs-lookup"><span data-stu-id="21ec1-113">maxPoints</span></span>|<span data-ttu-id="21ec1-114">Único</span><span class="sxs-lookup"><span data-stu-id="21ec1-114">Single</span></span>| <span data-ttu-id="21ec1-115">Máximo de pontos possíveis para esta atribuição.</span><span class="sxs-lookup"><span data-stu-id="21ec1-115">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="21ec1-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21ec1-116">JSON representation</span></span>

<span data-ttu-id="21ec1-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21ec1-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType"
}-->

```json
{
  "maxPoints": "Double"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
