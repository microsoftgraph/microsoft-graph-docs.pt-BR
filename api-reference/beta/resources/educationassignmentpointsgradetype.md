---
title: tipo de recurso educationAssignmentPointsGradeType
description: Usada com a propriedade **assignments. Grading** . Esta é uma subclasse de educationAssignmentGradeType.
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 567bff38f8a20456dffffdd91775a1e32852fe20
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543083"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="1cac6-104">tipo de recurso educationAssignmentPointsGradeType</span><span class="sxs-lookup"><span data-stu-id="1cac6-104">educationAssignmentPointsGradeType resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cac6-105">Usada com a propriedade **assignments. Grading** .</span><span class="sxs-lookup"><span data-stu-id="1cac6-105">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="1cac6-106">Esta é uma subclasse de [educationAssignmentGradeType](educationassignmentgradetype.md).</span><span class="sxs-lookup"><span data-stu-id="1cac6-106">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="1cac6-107">Isso indica que a atribuição foi classificada e armazena o número máximo de pontos que cada aluno pode obter nesse item de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1cac6-107">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="1cac6-108">Quando isso é definido em uma atribuição, cada envio receberá uma propriedade [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) associada ao armazenamento dos pontos de cada aluno.</span><span class="sxs-lookup"><span data-stu-id="1cac6-108">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="1cac6-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1cac6-109">Properties</span></span>
| <span data-ttu-id="1cac6-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1cac6-110">Property</span></span>     | <span data-ttu-id="1cac6-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cac6-111">Type</span></span>   |<span data-ttu-id="1cac6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cac6-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1cac6-113">maxPoints</span><span class="sxs-lookup"><span data-stu-id="1cac6-113">maxPoints</span></span>|<span data-ttu-id="1cac6-114">Único</span><span class="sxs-lookup"><span data-stu-id="1cac6-114">Single</span></span>| <span data-ttu-id="1cac6-115">Máximo de pontos possíveis para esta atribuição.</span><span class="sxs-lookup"><span data-stu-id="1cac6-115">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="1cac6-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1cac6-116">JSON representation</span></span>

<span data-ttu-id="1cac6-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1cac6-117">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentpointsgradetype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
