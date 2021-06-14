---
title: Tipo de recurso educationPointsOutcome
description: Um educationOutcome que fornece uma nota numérica.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2fdef09c65203c8fc17786f0e663db326057323d
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912143"
---
# <a name="educationpointsoutcome-resource-type"></a><span data-ttu-id="5d655-103">Tipo de recurso educationPointsOutcome</span><span class="sxs-lookup"><span data-stu-id="5d655-103">educationPointsOutcome resource type</span></span>

<span data-ttu-id="5d655-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d655-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d655-105">Um [educationOutcome](educationoutcome.md) que fornece uma nota numérica.</span><span class="sxs-lookup"><span data-stu-id="5d655-105">An [educationOutcome](educationoutcome.md) that gives a numerical grade.</span></span>

## <a name="methods"></a><span data-ttu-id="5d655-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="5d655-106">Methods</span></span>

| <span data-ttu-id="5d655-107">Método</span><span class="sxs-lookup"><span data-stu-id="5d655-107">Method</span></span>       | <span data-ttu-id="5d655-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5d655-108">Return Type</span></span> | <span data-ttu-id="5d655-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d655-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5d655-110">Atualizar educationOutcome</span><span class="sxs-lookup"><span data-stu-id="5d655-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="5d655-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="5d655-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="5d655-112">Atualizar o objeto educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="5d655-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5d655-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5d655-113">Properties</span></span>

| <span data-ttu-id="5d655-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5d655-114">Property</span></span>     | <span data-ttu-id="5d655-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="5d655-115">Type</span></span>        | <span data-ttu-id="5d655-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d655-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5d655-117">points</span><span class="sxs-lookup"><span data-stu-id="5d655-117">points</span></span>|[<span data-ttu-id="5d655-118">educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="5d655-118">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="5d655-119">A nota numérica que o professor deu ao aluno para essa atribuição.</span><span class="sxs-lookup"><span data-stu-id="5d655-119">The numeric grade the teacher has given the student for this assignment.</span></span>|
|<span data-ttu-id="5d655-120">publishedPoints</span><span class="sxs-lookup"><span data-stu-id="5d655-120">publishedPoints</span></span>|[<span data-ttu-id="5d655-121">educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="5d655-121">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="5d655-122">Uma cópia da propriedade points que é feita quando a nota é liberada para o aluno.</span><span class="sxs-lookup"><span data-stu-id="5d655-122">A copy of the points property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d655-123">Relações</span><span class="sxs-lookup"><span data-stu-id="5d655-123">Relationships</span></span>

<span data-ttu-id="5d655-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5d655-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d655-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5d655-125">JSON representation</span></span>

<span data-ttu-id="5d655-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5d655-126">The following is a JSON representation of the resource.</span></span>

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

