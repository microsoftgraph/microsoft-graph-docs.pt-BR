---
title: tipo de recurso educationAssignmentPointsGrade
description: Quando uma atribuição é definida como um tipo de grade de pontos, cada envio terá esse objeto associado à propriedade **enmisse.** Isso cria uma subclasse de educationAssignmentGrade,
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: bcce2fc6445c465defb2d795f3bfab9545838643
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013711"
---
# <a name="educationassignmentpointsgrade-resource-type"></a><span data-ttu-id="c66ee-104">tipo de recurso educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="c66ee-104">educationAssignmentPointsGrade resource type</span></span>

<span data-ttu-id="c66ee-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c66ee-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c66ee-106">Quando uma atribuição é definida como um tipo de grade de pontos, cada envio terá esse objeto associado à propriedade **enmisse.**</span><span class="sxs-lookup"><span data-stu-id="c66ee-106">When an assignment is set to a points grade type, each submission will have this object associated with the **submission.grade** property.</span></span> <span data-ttu-id="c66ee-107">Isso cria uma subclasse de [educationAssignmentGrade](educationassignmentgrade.md), que adicionará os dados de quem a essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="c66ee-107">This creates a subclass from [educationAssignmentGrade](educationassignmentgrade.md), which will add the who data to this property.</span></span> <span data-ttu-id="c66ee-108">O máximo de pontos é armazenado na propriedade **assignments. Grading** .</span><span class="sxs-lookup"><span data-stu-id="c66ee-108">The max points is stored in the **assignments.grading** property.</span></span>


## <a name="properties"></a><span data-ttu-id="c66ee-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c66ee-109">Properties</span></span>
| <span data-ttu-id="c66ee-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c66ee-110">Property</span></span>     | <span data-ttu-id="c66ee-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c66ee-111">Type</span></span>   |<span data-ttu-id="c66ee-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c66ee-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c66ee-113">points</span><span class="sxs-lookup"><span data-stu-id="c66ee-113">points</span></span>|<span data-ttu-id="c66ee-114">Único</span><span class="sxs-lookup"><span data-stu-id="c66ee-114">Single</span></span>|<span data-ttu-id="c66ee-115">Número de pontos que um professor está dando este objeto de envio.</span><span class="sxs-lookup"><span data-stu-id="c66ee-115">Number of points a teacher is giving this submission object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c66ee-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c66ee-116">JSON representation</span></span>

<span data-ttu-id="c66ee-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c66ee-117">The following is a JSON representation of the resource.</span></span>

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


