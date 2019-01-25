---
title: tipo de recurso de educationAssignmentPointsGrade
description: Quando uma atribuição for definida como um tipo de nível de pontos, a cada envio terão este objeto associado com a propriedade **submission.grade** . Isso cria uma subclasse do educationAssignmentGrade,
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 5d2a5cf6f6f886185179c6f1a61c1bb1d9d1ecfc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523733"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="0d508-104">tipo de recurso de educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="0d508-104">educationAssignmentPointsGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d508-105">Quando uma atribuição for definida como um tipo de nível de pontos, a cada envio terão este objeto associado com a propriedade **submission.grade** .</span><span class="sxs-lookup"><span data-stu-id="0d508-105">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="0d508-106">Isso cria uma subclasse do [educationAssignmentGrade](educationassignmentgrade.md), que adicionará a quem dados para esta propriedade.</span><span class="sxs-lookup"><span data-stu-id="0d508-106">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="0d508-107">Os pontos máximo é armazenado na propriedade **assignments.grading** .</span><span class="sxs-lookup"><span data-stu-id="0d508-107">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="0d508-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0d508-108">Properties</span></span>
| <span data-ttu-id="0d508-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0d508-109">Property</span></span>     | <span data-ttu-id="0d508-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0d508-110">Type</span></span>   |<span data-ttu-id="0d508-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0d508-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d508-112">points</span><span class="sxs-lookup"><span data-stu-id="0d508-112">points</span></span>|<span data-ttu-id="0d508-113">Single</span><span class="sxs-lookup"><span data-stu-id="0d508-113">Single</span></span>|<span data-ttu-id="0d508-114">Número de pontos um professor está dando este objeto de envio.</span><span class="sxs-lookup"><span data-stu-id="0d508-114">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d508-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0d508-115">JSON representation</span></span>

<span data-ttu-id="0d508-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0d508-116">The following is a JSON representation of the resource.</span></span>

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
