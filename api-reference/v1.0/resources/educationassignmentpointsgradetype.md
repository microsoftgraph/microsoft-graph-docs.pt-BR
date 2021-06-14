---
title: tipo de recurso educationAssignmentPointsGradeType
description: Tipo de recurso usado com a **propriedade assignments.grading.** Esta é uma subclasse de educationAssignmentGradeType.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ca5a6ba0dd6674d55b4659fbdb1e2c288a65eb12
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912201"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="9c68a-104">tipo de recurso educationAssignmentPointsGradeType</span><span class="sxs-lookup"><span data-stu-id="9c68a-104">educationAssignmentPointsGradeType resource type</span></span>

<span data-ttu-id="9c68a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c68a-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9c68a-106">Tipo de recurso usado com a **propriedade assignments.grading.**</span><span class="sxs-lookup"><span data-stu-id="9c68a-106">Resource type that is used with the **assignments.grading** property.</span></span> <span data-ttu-id="9c68a-107">Esta é uma subclasse [de educationAssignmentGradeType](educationassignmentgradetype.md).</span><span class="sxs-lookup"><span data-stu-id="9c68a-107">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="9c68a-108">Isso indica que a atribuição é gradeada e armazena o número máximo de pontos que cada aluno pode alcançar neste item de trabalho.</span><span class="sxs-lookup"><span data-stu-id="9c68a-108">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="9c68a-109">Quando isso for definido em uma atribuição, cada envio receberá uma propriedade [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) associada a ela para o armazenamento dos pontos de cada aluno.</span><span class="sxs-lookup"><span data-stu-id="9c68a-109">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="9c68a-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c68a-110">Properties</span></span>
| <span data-ttu-id="9c68a-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9c68a-111">Property</span></span>     | <span data-ttu-id="9c68a-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c68a-112">Type</span></span>   |<span data-ttu-id="9c68a-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c68a-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c68a-114">maxPoints</span><span class="sxs-lookup"><span data-stu-id="9c68a-114">maxPoints</span></span>|<span data-ttu-id="9c68a-115">Único</span><span class="sxs-lookup"><span data-stu-id="9c68a-115">Single</span></span>| <span data-ttu-id="9c68a-116">Pontos máximos possíveis para essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="9c68a-116">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="9c68a-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c68a-117">JSON representation</span></span>

<span data-ttu-id="9c68a-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c68a-118">The following is a JSON representation of the resource.</span></span>

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


