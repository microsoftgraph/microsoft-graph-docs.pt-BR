---
title: tipo de recurso educationPointsOutcome
description: Um educationOutcome que fornece uma classificação numérica
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: eb8c95fa7d13f57cca2c2fe19d7b992e6e2cab98
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049741"
---
# <a name="educationpointsoutcome-resource-type"></a><span data-ttu-id="10f41-103">tipo de recurso educationPointsOutcome</span><span class="sxs-lookup"><span data-stu-id="10f41-103">educationPointsOutcome resource type</span></span>

<span data-ttu-id="10f41-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10f41-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10f41-105">Um [educationOutcome](educationoutcome.md) que fornece uma classificação numérica.</span><span class="sxs-lookup"><span data-stu-id="10f41-105">An [educationOutcome](educationoutcome.md) that gives a numerical grade.</span></span>

## <a name="methods"></a><span data-ttu-id="10f41-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="10f41-106">Methods</span></span>

| <span data-ttu-id="10f41-107">Método</span><span class="sxs-lookup"><span data-stu-id="10f41-107">Method</span></span>       | <span data-ttu-id="10f41-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="10f41-108">Return Type</span></span> | <span data-ttu-id="10f41-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="10f41-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="10f41-110">Atualizar educationOutcome</span><span class="sxs-lookup"><span data-stu-id="10f41-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="10f41-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="10f41-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="10f41-112">Atualize o objeto educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="10f41-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="10f41-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="10f41-113">Properties</span></span>

| <span data-ttu-id="10f41-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="10f41-114">Property</span></span>     | <span data-ttu-id="10f41-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="10f41-115">Type</span></span>        | <span data-ttu-id="10f41-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="10f41-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="10f41-117">points</span><span class="sxs-lookup"><span data-stu-id="10f41-117">points</span></span>|[<span data-ttu-id="10f41-118">educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="10f41-118">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="10f41-119">A série de números que o professor forneceu ao aluno para esta atribuição.</span><span class="sxs-lookup"><span data-stu-id="10f41-119">The numeric grade the teacher has given the student for this assignment.</span></span>|
|<span data-ttu-id="10f41-120">publishedPoints</span><span class="sxs-lookup"><span data-stu-id="10f41-120">publishedPoints</span></span>|[<span data-ttu-id="10f41-121">educationAssignmentPointsGrade</span><span class="sxs-lookup"><span data-stu-id="10f41-121">educationAssignmentPointsGrade</span></span>](educationassignmentpointsgrade.md)|<span data-ttu-id="10f41-122">Uma cópia da propriedade Points que é feita quando a nota é liberada para o aluno.</span><span class="sxs-lookup"><span data-stu-id="10f41-122">A copy of the points property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10f41-123">Relações</span><span class="sxs-lookup"><span data-stu-id="10f41-123">Relationships</span></span>

<span data-ttu-id="10f41-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="10f41-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="10f41-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="10f41-125">JSON representation</span></span>

<span data-ttu-id="10f41-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="10f41-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPointsOutcome",
  "baseType": "",
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

