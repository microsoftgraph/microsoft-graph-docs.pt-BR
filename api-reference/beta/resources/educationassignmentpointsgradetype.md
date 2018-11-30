---
title: tipo de recurso de educationAssignmentPointsGradeType
description: Usada com a propriedade **assignments.grading** . Isso é uma subclasse de educationAssignmentGradeType.
ms.openlocfilehash: 5c170540e99003a78df0550d4d6542c07df8f1ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040151"
---
# <a name="educationassignmentpointsgradetype-resource-type"></a><span data-ttu-id="95512-104">tipo de recurso de educationAssignmentPointsGradeType</span><span class="sxs-lookup"><span data-stu-id="95512-104">educationAssignmentPointsGradeType resource type</span></span>

> <span data-ttu-id="95512-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="95512-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95512-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="95512-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="95512-107">Usada com a propriedade **assignments.grading** .</span><span class="sxs-lookup"><span data-stu-id="95512-107">Used with the **assignments.grading** property.</span></span> <span data-ttu-id="95512-108">Isso é uma subclasse de [educationAssignmentGradeType](educationassignmentgradetype.md).</span><span class="sxs-lookup"><span data-stu-id="95512-108">This is a subclass of [educationAssignmentGradeType](educationassignmentgradetype.md).</span></span>

<span data-ttu-id="95512-109">Isso indica que a atribuição varie e armazena o número máximo de pontos que cada estudante pode alcançar este item de trabalho.</span><span class="sxs-lookup"><span data-stu-id="95512-109">This indicates that the assignment is graded and stores the maximum number of points each student can achieve on this work item.</span></span> <span data-ttu-id="95512-110">Quando isso é definido em uma atribuição, cada envio receberá uma propriedade [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) associada a ela para o armazenamento de pontos de cada student.</span><span class="sxs-lookup"><span data-stu-id="95512-110">When this is set on an assignment, each submission will get an [educationAssignmentPointsGrade](educationassignmentpointsgrade.md) property associated with it for the storage of each student's points.</span></span>

## <a name="properties"></a><span data-ttu-id="95512-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95512-111">Properties</span></span>
| <span data-ttu-id="95512-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95512-112">Property</span></span>     | <span data-ttu-id="95512-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="95512-113">Type</span></span>   |<span data-ttu-id="95512-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="95512-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95512-115">maxPoints</span><span class="sxs-lookup"><span data-stu-id="95512-115">maxPoints</span></span>|<span data-ttu-id="95512-116">Single</span><span class="sxs-lookup"><span data-stu-id="95512-116">Single</span></span>| <span data-ttu-id="95512-117">Max aponta possíveis para essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="95512-117">Max points possible for this assignment.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="95512-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95512-118">JSON representation</span></span>

<span data-ttu-id="95512-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="95512-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentPointsGradeType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->