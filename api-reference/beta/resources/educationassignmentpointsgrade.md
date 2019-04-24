---
title: tipo de recurso educationAssignmentPointsGrade
description: Quando uma atribuição é definida como um tipo de grade de pontos, cada envio terá esse objeto associado à propriedade enmisse **.** Isso cria uma subclasse de educationAssignmentGrade,
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 5d2a5cf6f6f886185179c6f1a61c1bb1d9d1ecfc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507333"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="07461-104">tipo de recurso educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="07461-104">educationAssignmentPointsGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07461-105">Quando uma atribuição é definida como um tipo de grade de pontos, cada envio terá esse objeto associado à propriedade enmisse **.**</span><span class="sxs-lookup"><span data-stu-id="07461-105">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="07461-106">Isso cria uma subclasse de [educationAssignmentGrade](educationassignmentgrade.md), que adicionará os dados de quem a essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="07461-106">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="07461-107">O máximo de pontos é armazenado na propriedade **assignments. Grading** .</span><span class="sxs-lookup"><span data-stu-id="07461-107">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="07461-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07461-108">Properties</span></span>
| <span data-ttu-id="07461-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07461-109">Property</span></span>     | <span data-ttu-id="07461-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="07461-110">Type</span></span>   |<span data-ttu-id="07461-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="07461-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="07461-112">points</span><span class="sxs-lookup"><span data-stu-id="07461-112">points</span></span>|<span data-ttu-id="07461-113">Único</span><span class="sxs-lookup"><span data-stu-id="07461-113">Single</span></span>|<span data-ttu-id="07461-114">Número de pontos que um professor está dando este objeto de envio.</span><span class="sxs-lookup"><span data-stu-id="07461-114">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="07461-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07461-115">JSON representation</span></span>

<span data-ttu-id="07461-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07461-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}-->

```json
{
  "points": "Single"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentpointsgrade.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
