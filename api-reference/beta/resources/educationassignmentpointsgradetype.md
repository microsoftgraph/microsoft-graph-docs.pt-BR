---
title: tipo de recurso educationAssignmentPointsGradeType
description: Usada com a propriedade **assignments. Grading** . Esta é uma subclasse de educationAssignmentGradeType.
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b11ba94bba2147e2ef1d084a66cd7628371a57fa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998877"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="33c14-104">tipo de recurso educationAssignmentPointsGradeType</span><span class="sxs-lookup"><span data-stu-id="33c14-104">educationAssignmentPointsGradeType resource type</span></span>

<span data-ttu-id="33c14-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33c14-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33c14-106">Usada com a propriedade **assignments. Grading** .</span><span class="sxs-lookup"><span data-stu-id="33c14-106">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="33c14-107">Esta é uma subclasse de [educationAssignmentGradeType](educationassignmentgradetype.md).</span><span class="sxs-lookup"><span data-stu-id="33c14-107">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="33c14-108">Isso indica que a atribuição foi classificada e armazena o número máximo de pontos que cada aluno pode obter nesse item de trabalho.</span><span class="sxs-lookup"><span data-stu-id="33c14-108">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="33c14-109">Quando isso é definido em uma atribuição, cada envio receberá uma propriedade [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) associada ao armazenamento dos pontos de cada aluno.</span><span class="sxs-lookup"><span data-stu-id="33c14-109">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="33c14-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="33c14-110">Properties</span></span>
| <span data-ttu-id="33c14-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="33c14-111">Property</span></span>     | <span data-ttu-id="33c14-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="33c14-112">Type</span></span>   |<span data-ttu-id="33c14-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="33c14-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="33c14-114">maxPoints</span><span class="sxs-lookup"><span data-stu-id="33c14-114">maxPoints</span></span>|<span data-ttu-id="33c14-115">Único</span><span class="sxs-lookup"><span data-stu-id="33c14-115">Single</span></span>| <span data-ttu-id="33c14-116">Máximo de pontos possíveis para esta atribuição.</span><span class="sxs-lookup"><span data-stu-id="33c14-116">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="33c14-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="33c14-117">JSON representation</span></span>

<span data-ttu-id="33c14-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="33c14-118">The following is a JSON representation of the resource.</span></span>

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


