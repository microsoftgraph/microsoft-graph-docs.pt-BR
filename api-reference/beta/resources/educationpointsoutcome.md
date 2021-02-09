---
title: Tipo de recurso educationPointsOutcome
description: Um educationOutcome que fornece uma nota numérica
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ebf9a0bf12b7c4a78f28c9d75c93469afec2c34c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153617"
---
# <a name="educationpointsoutcome-resource-type"></a><span data-ttu-id="b8e94-103">Tipo de recurso educationPointsOutcome</span><span class="sxs-lookup"><span data-stu-id="b8e94-103">educationPointsOutcome resource type</span></span>

<span data-ttu-id="b8e94-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8e94-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8e94-105">Um [educationOutcome](educationoutcome.md) que fornece uma nota numérica.</span><span class="sxs-lookup"><span data-stu-id="b8e94-105">An [educationOutcome](educationoutcome.md) that gives a numerical grade.</span></span>

## <a name="methods"></a><span data-ttu-id="b8e94-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="b8e94-106">Methods</span></span>

| <span data-ttu-id="b8e94-107">Método</span><span class="sxs-lookup"><span data-stu-id="b8e94-107">Method</span></span>       | <span data-ttu-id="b8e94-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b8e94-108">Return Type</span></span> | <span data-ttu-id="b8e94-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8e94-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b8e94-110">Atualizar educationOutcome</span><span class="sxs-lookup"><span data-stu-id="b8e94-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="b8e94-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="b8e94-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="b8e94-112">Atualize o objeto educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="b8e94-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b8e94-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b8e94-113">Properties</span></span>

| <span data-ttu-id="b8e94-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b8e94-114">Property</span></span>     | <span data-ttu-id="b8e94-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="b8e94-115">Type</span></span>        | <span data-ttu-id="b8e94-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="b8e94-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b8e94-117">points</span><span class="sxs-lookup"><span data-stu-id="b8e94-117">points</span></span>|[<span data-ttu-id="b8e94-118">educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="b8e94-118">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="b8e94-119">A nota numérica que o professor deu ao aluno para essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="b8e94-119">The numeric grade the teacher has given the student for this assignment.</span></span>|
|<span data-ttu-id="b8e94-120">publishedPoints</span><span class="sxs-lookup"><span data-stu-id="b8e94-120">publishedPoints</span></span>|[<span data-ttu-id="b8e94-121">educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="b8e94-121">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="b8e94-122">Uma cópia da propriedade points que é feita quando a nota é liberada para o aluno.</span><span class="sxs-lookup"><span data-stu-id="b8e94-122">A copy of the points property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8e94-123">Relações</span><span class="sxs-lookup"><span data-stu-id="b8e94-123">Relationships</span></span>

<span data-ttu-id="b8e94-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b8e94-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8e94-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b8e94-125">JSON representation</span></span>

<span data-ttu-id="b8e94-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b8e94-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPointsOutcome",
  "keyProperty": "id"
}-->

```json
{
  "points": {"@odata.type": "microsoft.graph.educationAssignmentPointsGrade"},
  "publishedPoints": {"@odata.type": "microsoft.graph.educationAssignmentPointsGrade"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationPointsOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

