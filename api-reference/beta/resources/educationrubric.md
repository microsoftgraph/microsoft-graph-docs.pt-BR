---
title: tipo de recurso educationRubric
description: Uma amostra rubric de gradação que pode ser anexada a uma atribuição
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b43b611465af4dabb62d9dd741eb9a8670f241b9
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173234"
---
# <a name="educationrubric-resource-type"></a><span data-ttu-id="de171-103">tipo de recurso educationRubric</span><span class="sxs-lookup"><span data-stu-id="de171-103">educationRubric resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de171-104">Um amostra rubric de gradação que pode ser anexado a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="de171-104">A grading rubric that can be attached to an assignment.</span></span> <span data-ttu-id="de171-105">Um amostra rubric é associado a um **educationUser** (professor) e anexado a um ou mais recursos do **educationAssignment** .</span><span class="sxs-lookup"><span data-stu-id="de171-105">A rubric is associated with an **educationUser** (teacher), and attached to one or more **educationAssignment** resources.</span></span> 

<span data-ttu-id="de171-106">Consulte [Education amostra rubric Overview](https://developer.microsoft.com/graph/docs/concepts/education-rubric-overview) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="de171-106">See [Education rubric overview](https://developer.microsoft.com/graph/docs/concepts/education-rubric-overview) for more information.</span></span>

## <a name="methods"></a><span data-ttu-id="de171-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="de171-107">Methods</span></span>

| <span data-ttu-id="de171-108">Método</span><span class="sxs-lookup"><span data-stu-id="de171-108">Method</span></span>       | <span data-ttu-id="de171-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="de171-109">Return Type</span></span> | <span data-ttu-id="de171-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="de171-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="de171-111">Obter educationRubric</span><span class="sxs-lookup"><span data-stu-id="de171-111">Get educationRubric</span></span>](../api/educationrubric-get.md) | [<span data-ttu-id="de171-112">educationRubric</span><span class="sxs-lookup"><span data-stu-id="de171-112">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="de171-113">Leia as propriedades e os relacionamentos do objeto educationRubric.</span><span class="sxs-lookup"><span data-stu-id="de171-113">Read properties and relationships of educationRubric object.</span></span> |
| [<span data-ttu-id="de171-114">Atualizar educationRubric</span><span class="sxs-lookup"><span data-stu-id="de171-114">Update educationRubric</span></span>](../api/educationrubric-update.md) | [<span data-ttu-id="de171-115">educationRubric</span><span class="sxs-lookup"><span data-stu-id="de171-115">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="de171-116">Atualize o objeto educationRubric.</span><span class="sxs-lookup"><span data-stu-id="de171-116">Update educationRubric object.</span></span> |
| [<span data-ttu-id="de171-117">Excluir educationRubric</span><span class="sxs-lookup"><span data-stu-id="de171-117">Delete educationRubric</span></span>](../api/educationrubric-delete.md) | <span data-ttu-id="de171-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de171-118">None</span></span> | <span data-ttu-id="de171-119">Exclua o objeto educationRubric.</span><span class="sxs-lookup"><span data-stu-id="de171-119">Delete educationRubric object.</span></span> |

## <a name="properties"></a><span data-ttu-id="de171-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de171-120">Properties</span></span>

| <span data-ttu-id="de171-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de171-121">Property</span></span>     | <span data-ttu-id="de171-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="de171-122">Type</span></span>        | <span data-ttu-id="de171-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="de171-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="de171-124">createdBy</span><span class="sxs-lookup"><span data-stu-id="de171-124">createdBy</span></span>|[<span data-ttu-id="de171-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="de171-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="de171-126">O usuário que criou este recurso.</span><span class="sxs-lookup"><span data-stu-id="de171-126">The user who created this resource.</span></span>|
|<span data-ttu-id="de171-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="de171-127">createdDateTime</span></span>|<span data-ttu-id="de171-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de171-128">DateTimeOffset</span></span>|<span data-ttu-id="de171-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="de171-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="de171-131">descrição</span><span class="sxs-lookup"><span data-stu-id="de171-131">description</span></span>|[<span data-ttu-id="de171-132">itemBody</span><span class="sxs-lookup"><span data-stu-id="de171-132">itemBody</span></span>](itembody.md)|<span data-ttu-id="de171-133">A descrição desse amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="de171-133">The description of this rubric.</span></span>|
|<span data-ttu-id="de171-134">displayName</span><span class="sxs-lookup"><span data-stu-id="de171-134">displayName</span></span>|<span data-ttu-id="de171-135">String</span><span class="sxs-lookup"><span data-stu-id="de171-135">String</span></span>|<span data-ttu-id="de171-136">O nome deste amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="de171-136">The name of this rubric.</span></span>|
|<span data-ttu-id="de171-137">notas</span><span class="sxs-lookup"><span data-stu-id="de171-137">grading</span></span>|[<span data-ttu-id="de171-138">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="de171-138">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="de171-139">O tipo de gradação desse amostra rubric-NULL para um amostra rubric sem pontos, ou [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) para um ponto amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="de171-139">The grading type of this rubric -- null for a no-points rubric, or [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) for a points rubric.</span></span>|
|<span data-ttu-id="de171-140">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="de171-140">lastModifiedBy</span></span>|[<span data-ttu-id="de171-141">identitySet</span><span class="sxs-lookup"><span data-stu-id="de171-141">identitySet</span></span>](identityset.md)|<span data-ttu-id="de171-142">O último usuário a modificar o recurso.</span><span class="sxs-lookup"><span data-stu-id="de171-142">The last user to modify the resource.</span></span>|
|<span data-ttu-id="de171-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de171-143">lastModifiedDateTime</span></span>|<span data-ttu-id="de171-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de171-144">DateTimeOffset</span></span>|<span data-ttu-id="de171-145">Momento no momento em que o recurso foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="de171-145">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="de171-146">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="de171-146">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="de171-147">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="de171-147">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="de171-148">alcançar</span><span class="sxs-lookup"><span data-stu-id="de171-148">levels</span></span>|<span data-ttu-id="de171-149">coleção [rubricLevel](rubriclevel.md)</span><span class="sxs-lookup"><span data-stu-id="de171-149">[rubricLevel](rubriclevel.md) collection</span></span>|<span data-ttu-id="de171-150">A coleção de níveis que compõem este amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="de171-150">The collection of levels making up this rubric.</span></span>|
|<span data-ttu-id="de171-151">qualidades</span><span class="sxs-lookup"><span data-stu-id="de171-151">qualities</span></span>|<span data-ttu-id="de171-152">coleção [rubricQuality](rubricquality.md)</span><span class="sxs-lookup"><span data-stu-id="de171-152">[rubricQuality](rubricquality.md) collection</span></span>|<span data-ttu-id="de171-153">O conjunto de qualidades que compõem este amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="de171-153">The collection of qualities making up this rubric.</span></span>|

## <a name="relationships"></a><span data-ttu-id="de171-154">Relações</span><span class="sxs-lookup"><span data-stu-id="de171-154">Relationships</span></span>

<span data-ttu-id="de171-155">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de171-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de171-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de171-156">JSON representation</span></span>

<span data-ttu-id="de171-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de171-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubric",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "grading": {"@odata.type": "microsoft.graph.educationAssignmentGradeType"},
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "levels": [{"@odata.type": "microsoft.graph.rubricLevel"}],
  "qualities": [{"@odata.type": "microsoft.graph.rubricQuality"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRubric resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->