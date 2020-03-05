---
title: tipo de recurso educationAssignmentPointsGradeType
description: Usada com a propriedade **assignments. Grading** . Esta é uma subclasse de educationAssignmentGradeType.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2e233faa1ab550c5f970018b6d4bf6879ba99c8f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502470"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="1a783-104">tipo de recurso educationAssignmentPointsGradeType</span><span class="sxs-lookup"><span data-stu-id="1a783-104">educationAssignmentPointsGradeType resource type</span></span>

<span data-ttu-id="1a783-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1a783-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a783-106">Usada com a propriedade **assignments. Grading** .</span><span class="sxs-lookup"><span data-stu-id="1a783-106">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="1a783-107">Esta é uma subclasse de [educationAssignmentGradeType](educationassignmentgradetype.md).</span><span class="sxs-lookup"><span data-stu-id="1a783-107">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="1a783-108">Isso indica que a atribuição foi classificada e armazena o número máximo de pontos que cada aluno pode obter nesse item de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1a783-108">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="1a783-109">Quando isso é definido em uma atribuição, cada envio receberá uma propriedade [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) associada ao armazenamento dos pontos de cada aluno.</span><span class="sxs-lookup"><span data-stu-id="1a783-109">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="1a783-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a783-110">Properties</span></span>
| <span data-ttu-id="1a783-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a783-111">Property</span></span>     | <span data-ttu-id="1a783-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a783-112">Type</span></span>   |<span data-ttu-id="1a783-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a783-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a783-114">maxPoints</span><span class="sxs-lookup"><span data-stu-id="1a783-114">maxPoints</span></span>|<span data-ttu-id="1a783-115">Único</span><span class="sxs-lookup"><span data-stu-id="1a783-115">Single</span></span>| <span data-ttu-id="1a783-116">Máximo de pontos possíveis para esta atribuição.</span><span class="sxs-lookup"><span data-stu-id="1a783-116">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="1a783-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a783-117">JSON representation</span></span>

<span data-ttu-id="1a783-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a783-118">The following is a JSON representation of the resource.</span></span>

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
