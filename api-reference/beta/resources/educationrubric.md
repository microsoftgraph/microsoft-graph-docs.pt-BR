---
title: tipo de recurso educationRubric
description: Uma amostra rubric de gradação que pode ser anexada a uma atribuição
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 154e153166c45a0eb671ab554d1b8ed337fb9830
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406069"
---
# <a name="educationrubric-resource-type"></a><span data-ttu-id="6d0a0-103">tipo de recurso educationRubric</span><span class="sxs-lookup"><span data-stu-id="6d0a0-103">educationRubric resource type</span></span>

<span data-ttu-id="6d0a0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d0a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d0a0-105">Um amostra rubric de gradação que pode ser anexado a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="6d0a0-105">A grading rubric that can be attached to an assignment.</span></span> <span data-ttu-id="6d0a0-106">Um amostra rubric é associado a um **educationUser** (professor) e anexado a um ou mais recursos do **educationAssignment** .</span><span class="sxs-lookup"><span data-stu-id="6d0a0-106">A rubric is associated with an **educationUser** (teacher), and attached to one or more **educationAssignment** resources.</span></span> 

<span data-ttu-id="6d0a0-107">Consulte [Education amostra rubric Overview](/graph/education-rubric-overview) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="6d0a0-107">See [Education rubric overview](/graph/education-rubric-overview) for more information.</span></span>

## <a name="methods"></a><span data-ttu-id="6d0a0-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="6d0a0-108">Methods</span></span>

| <span data-ttu-id="6d0a0-109">Método</span><span class="sxs-lookup"><span data-stu-id="6d0a0-109">Method</span></span>       | <span data-ttu-id="6d0a0-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6d0a0-110">Return Type</span></span> | <span data-ttu-id="6d0a0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d0a0-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="6d0a0-112">Criar educationRubric</span><span class="sxs-lookup"><span data-stu-id="6d0a0-112">Create educationRubric</span></span>](../api/educationuser-post-rubrics.md) | [<span data-ttu-id="6d0a0-113">educationRubric</span><span class="sxs-lookup"><span data-stu-id="6d0a0-113">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="6d0a0-114">Criar um novo objeto educationRubric.</span><span class="sxs-lookup"><span data-stu-id="6d0a0-114">Create a new educationRubric object.</span></span> |
| [<span data-ttu-id="6d0a0-115">Obter educationRubric</span><span class="sxs-lookup"><span data-stu-id="6d0a0-115">Get educationRubric</span></span>](../api/educationrubric-get.md) | [<span data-ttu-id="6d0a0-116">educationRubric</span><span class="sxs-lookup"><span data-stu-id="6d0a0-116">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="6d0a0-117">Leia as propriedades e os relacionamentos do objeto educationRubric.</span><span class="sxs-lookup"><span data-stu-id="6d0a0-117">Read properties and relationships of educationRubric object.</span></span> |
| [<span data-ttu-id="6d0a0-118">Atualizar educationRubric</span><span class="sxs-lookup"><span data-stu-id="6d0a0-118">Update educationRubric</span></span>](../api/educationrubric-update.md) | [<span data-ttu-id="6d0a0-119">educationRubric</span><span class="sxs-lookup"><span data-stu-id="6d0a0-119">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="6d0a0-120">Atualize o objeto educationRubric.</span><span class="sxs-lookup"><span data-stu-id="6d0a0-120">Update educationRubric object.</span></span> |
| [<span data-ttu-id="6d0a0-121">Excluir educationRubric</span><span class="sxs-lookup"><span data-stu-id="6d0a0-121">Delete educationRubric</span></span>](../api/educationrubric-delete.md) | <span data-ttu-id="6d0a0-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6d0a0-122">None</span></span> | <span data-ttu-id="6d0a0-123">Exclua o objeto educationRubric.</span><span class="sxs-lookup"><span data-stu-id="6d0a0-123">Delete educationRubric object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6d0a0-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6d0a0-124">Properties</span></span>

| <span data-ttu-id="6d0a0-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6d0a0-125">Property</span></span>     | <span data-ttu-id="6d0a0-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="6d0a0-126">Type</span></span>        | <span data-ttu-id="6d0a0-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="6d0a0-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6d0a0-128">createdBy</span><span class="sxs-lookup"><span data-stu-id="6d0a0-128">createdBy</span></span>|[<span data-ttu-id="6d0a0-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="6d0a0-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="6d0a0-130">O usuário que criou este recurso.</span><span class="sxs-lookup"><span data-stu-id="6d0a0-130">The user who created this resource.</span></span>|
|<span data-ttu-id="6d0a0-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6d0a0-131">createdDateTime</span></span>|<span data-ttu-id="6d0a0-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d0a0-132">DateTimeOffset</span></span>|<span data-ttu-id="6d0a0-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6d0a0-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6d0a0-135">description</span><span class="sxs-lookup"><span data-stu-id="6d0a0-135">description</span></span>|[<span data-ttu-id="6d0a0-136">itemBody</span><span class="sxs-lookup"><span data-stu-id="6d0a0-136">itemBody</span></span>](itembody.md)|<span data-ttu-id="6d0a0-137">A descrição desse amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="6d0a0-137">The description of this rubric.</span></span>|
|<span data-ttu-id="6d0a0-138">displayName</span><span class="sxs-lookup"><span data-stu-id="6d0a0-138">displayName</span></span>|<span data-ttu-id="6d0a0-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6d0a0-139">String</span></span>|<span data-ttu-id="6d0a0-140">O nome deste amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="6d0a0-140">The name of this rubric.</span></span>|
|<span data-ttu-id="6d0a0-141">notas</span><span class="sxs-lookup"><span data-stu-id="6d0a0-141">grading</span></span>|[<span data-ttu-id="6d0a0-142">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="6d0a0-142">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="6d0a0-143">O tipo de gradação desse amostra rubric-NULL para um amostra rubric sem pontos, ou [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) para um ponto amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="6d0a0-143">The grading type of this rubric -- null for a no-points rubric, or [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) for a points rubric.</span></span>|
|<span data-ttu-id="6d0a0-144">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6d0a0-144">lastModifiedBy</span></span>|[<span data-ttu-id="6d0a0-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="6d0a0-145">identitySet</span></span>](identityset.md)|<span data-ttu-id="6d0a0-146">O último usuário a modificar o recurso.</span><span class="sxs-lookup"><span data-stu-id="6d0a0-146">The last user to modify the resource.</span></span>|
|<span data-ttu-id="6d0a0-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6d0a0-147">lastModifiedDateTime</span></span>|<span data-ttu-id="6d0a0-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6d0a0-148">DateTimeOffset</span></span>|<span data-ttu-id="6d0a0-149">Momento no momento em que o recurso foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="6d0a0-149">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="6d0a0-150">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="6d0a0-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6d0a0-151">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6d0a0-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6d0a0-152">alcançar</span><span class="sxs-lookup"><span data-stu-id="6d0a0-152">levels</span></span>|<span data-ttu-id="6d0a0-153">coleção [rubricLevel](rubriclevel.md)</span><span class="sxs-lookup"><span data-stu-id="6d0a0-153">[rubricLevel](rubriclevel.md) collection</span></span>|<span data-ttu-id="6d0a0-154">A coleção de níveis que compõem este amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="6d0a0-154">The collection of levels making up this rubric.</span></span>|
|<span data-ttu-id="6d0a0-155">qualidades</span><span class="sxs-lookup"><span data-stu-id="6d0a0-155">qualities</span></span>|<span data-ttu-id="6d0a0-156">coleção [rubricQuality](rubricquality.md)</span><span class="sxs-lookup"><span data-stu-id="6d0a0-156">[rubricQuality](rubricquality.md) collection</span></span>|<span data-ttu-id="6d0a0-157">O conjunto de qualidades que compõem este amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="6d0a0-157">The collection of qualities making up this rubric.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d0a0-158">Relações</span><span class="sxs-lookup"><span data-stu-id="6d0a0-158">Relationships</span></span>

<span data-ttu-id="6d0a0-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6d0a0-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d0a0-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6d0a0-160">JSON representation</span></span>

<span data-ttu-id="6d0a0-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6d0a0-161">The following is a JSON representation of the resource.</span></span>

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