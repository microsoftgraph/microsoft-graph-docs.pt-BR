---
title: tipo de recurso educationAssignmentPointsGradeType
description: Usada com a propriedade **assignments. Grading** . Esta é uma subclasse de educationAssignmentGradeType.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 61e6e425730685d4447875cdb074526e7ebc0a17
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334427"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="3132b-104">tipo de recurso educationAssignmentPointsGradeType</span><span class="sxs-lookup"><span data-stu-id="3132b-104">educationAssignmentPointsGradeType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3132b-105">Usada com a propriedade **assignments. Grading** .</span><span class="sxs-lookup"><span data-stu-id="3132b-105">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="3132b-106">Esta é uma subclasse de [educationAssignmentGradeType](educationassignmentgradetype.md).</span><span class="sxs-lookup"><span data-stu-id="3132b-106">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="3132b-107">Isso indica que a atribuição foi classificada e armazena o número máximo de pontos que cada aluno pode obter nesse item de trabalho.</span><span class="sxs-lookup"><span data-stu-id="3132b-107">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="3132b-108">Quando isso é definido em uma atribuição, cada envio receberá uma propriedade [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) associada ao armazenamento dos pontos de cada aluno.</span><span class="sxs-lookup"><span data-stu-id="3132b-108">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="3132b-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3132b-109">Properties</span></span>
| <span data-ttu-id="3132b-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3132b-110">Property</span></span>     | <span data-ttu-id="3132b-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="3132b-111">Type</span></span>   |<span data-ttu-id="3132b-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="3132b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3132b-113">maxPoints</span><span class="sxs-lookup"><span data-stu-id="3132b-113">maxPoints</span></span>|<span data-ttu-id="3132b-114">Único</span><span class="sxs-lookup"><span data-stu-id="3132b-114">Single</span></span>| <span data-ttu-id="3132b-115">Máximo de pontos possíveis para esta atribuição.</span><span class="sxs-lookup"><span data-stu-id="3132b-115">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="3132b-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3132b-116">JSON representation</span></span>

<span data-ttu-id="3132b-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3132b-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGradeType"
}-->

```json
{
  "maxPoints": "Single"
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
