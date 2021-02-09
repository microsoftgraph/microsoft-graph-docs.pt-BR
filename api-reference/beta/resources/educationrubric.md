---
title: Tipo de recurso educationRubric
description: Um rubric de gradação que pode ser anexado a uma atribuição
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 37e1d4a6267f1f1292a72cc7f34b8135483091ec
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161933"
---
# <a name="educationrubric-resource-type"></a><span data-ttu-id="4db99-103">Tipo de recurso educationRubric</span><span class="sxs-lookup"><span data-stu-id="4db99-103">educationRubric resource type</span></span>

<span data-ttu-id="4db99-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4db99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4db99-105">Um rubric de gradação que pode ser anexado a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="4db99-105">A grading rubric that can be attached to an assignment.</span></span> <span data-ttu-id="4db99-106">Um rubric é associado a **um educationUser** (professor) e anexado a um ou mais **recursos educationAssignment.**</span><span class="sxs-lookup"><span data-stu-id="4db99-106">A rubric is associated with an **educationUser** (teacher), and attached to one or more **educationAssignment** resources.</span></span> 

<span data-ttu-id="4db99-107">Confira [a visão geral do rubric educacional](/graph/education-rubric-overview) para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="4db99-107">See [Education rubric overview](/graph/education-rubric-overview) for more information.</span></span>

## <a name="methods"></a><span data-ttu-id="4db99-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="4db99-108">Methods</span></span>

| <span data-ttu-id="4db99-109">Método</span><span class="sxs-lookup"><span data-stu-id="4db99-109">Method</span></span>       | <span data-ttu-id="4db99-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4db99-110">Return Type</span></span> | <span data-ttu-id="4db99-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4db99-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4db99-112">Criar educationRubric</span><span class="sxs-lookup"><span data-stu-id="4db99-112">Create educationRubric</span></span>](../api/educationuser-post-rubrics.md) | [<span data-ttu-id="4db99-113">educationRubric</span><span class="sxs-lookup"><span data-stu-id="4db99-113">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="4db99-114">Crie um novo objeto educationRubric.</span><span class="sxs-lookup"><span data-stu-id="4db99-114">Create a new educationRubric object.</span></span> |
| [<span data-ttu-id="4db99-115">Obter educationRubric</span><span class="sxs-lookup"><span data-stu-id="4db99-115">Get educationRubric</span></span>](../api/educationrubric-get.md) | [<span data-ttu-id="4db99-116">educationRubric</span><span class="sxs-lookup"><span data-stu-id="4db99-116">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="4db99-117">Leia as propriedades e os relacionamentos do objeto educationRubric.</span><span class="sxs-lookup"><span data-stu-id="4db99-117">Read properties and relationships of educationRubric object.</span></span> |
| [<span data-ttu-id="4db99-118">Atualizar educationRubric</span><span class="sxs-lookup"><span data-stu-id="4db99-118">Update educationRubric</span></span>](../api/educationrubric-update.md) | [<span data-ttu-id="4db99-119">educationRubric</span><span class="sxs-lookup"><span data-stu-id="4db99-119">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="4db99-120">Atualize o objeto educationRubric.</span><span class="sxs-lookup"><span data-stu-id="4db99-120">Update educationRubric object.</span></span> |
| [<span data-ttu-id="4db99-121">Excluir educationRubric</span><span class="sxs-lookup"><span data-stu-id="4db99-121">Delete educationRubric</span></span>](../api/educationrubric-delete.md) | <span data-ttu-id="4db99-122">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="4db99-122">None</span></span> | <span data-ttu-id="4db99-123">Exclua o objeto educationRubric.</span><span class="sxs-lookup"><span data-stu-id="4db99-123">Delete educationRubric object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4db99-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4db99-124">Properties</span></span>

| <span data-ttu-id="4db99-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4db99-125">Property</span></span>     | <span data-ttu-id="4db99-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="4db99-126">Type</span></span>        | <span data-ttu-id="4db99-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="4db99-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4db99-128">createdBy</span><span class="sxs-lookup"><span data-stu-id="4db99-128">createdBy</span></span>|[<span data-ttu-id="4db99-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="4db99-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="4db99-130">O usuário que criou esse recurso.</span><span class="sxs-lookup"><span data-stu-id="4db99-130">The user who created this resource.</span></span>|
|<span data-ttu-id="4db99-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4db99-131">createdDateTime</span></span>|<span data-ttu-id="4db99-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4db99-132">DateTimeOffset</span></span>|<span data-ttu-id="4db99-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4db99-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4db99-135">description</span><span class="sxs-lookup"><span data-stu-id="4db99-135">description</span></span>|[<span data-ttu-id="4db99-136">itemBody</span><span class="sxs-lookup"><span data-stu-id="4db99-136">itemBody</span></span>](itembody.md)|<span data-ttu-id="4db99-137">A descrição desse rubric.</span><span class="sxs-lookup"><span data-stu-id="4db99-137">The description of this rubric.</span></span>|
|<span data-ttu-id="4db99-138">displayName</span><span class="sxs-lookup"><span data-stu-id="4db99-138">displayName</span></span>|<span data-ttu-id="4db99-139">String</span><span class="sxs-lookup"><span data-stu-id="4db99-139">String</span></span>|<span data-ttu-id="4db99-140">O nome dessa rubric.</span><span class="sxs-lookup"><span data-stu-id="4db99-140">The name of this rubric.</span></span>|
|<span data-ttu-id="4db99-141">grading</span><span class="sxs-lookup"><span data-stu-id="4db99-141">grading</span></span>|[<span data-ttu-id="4db99-142">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="4db99-142">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="4db99-143">O tipo de gradação desse rubric – nulo para um rubric sem pontos ou [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) para um rubric de pontos.</span><span class="sxs-lookup"><span data-stu-id="4db99-143">The grading type of this rubric -- null for a no-points rubric, or [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) for a points rubric.</span></span>|
|<span data-ttu-id="4db99-144">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="4db99-144">lastModifiedBy</span></span>|[<span data-ttu-id="4db99-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="4db99-145">identitySet</span></span>](identityset.md)|<span data-ttu-id="4db99-146">O último usuário a modificar o recurso.</span><span class="sxs-lookup"><span data-stu-id="4db99-146">The last user to modify the resource.</span></span>|
|<span data-ttu-id="4db99-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4db99-147">lastModifiedDateTime</span></span>|<span data-ttu-id="4db99-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4db99-148">DateTimeOffset</span></span>|<span data-ttu-id="4db99-149">Momento no tempo em que o recurso foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="4db99-149">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="4db99-150">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4db99-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4db99-151">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4db99-151">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4db99-152">níveis</span><span class="sxs-lookup"><span data-stu-id="4db99-152">levels</span></span>|<span data-ttu-id="4db99-153">[Coleção rubricLevel](rubriclevel.md)</span><span class="sxs-lookup"><span data-stu-id="4db99-153">[rubricLevel](rubriclevel.md) collection</span></span>|<span data-ttu-id="4db99-154">A coleção de níveis que comem esse rubric.</span><span class="sxs-lookup"><span data-stu-id="4db99-154">The collection of levels making up this rubric.</span></span>|
|<span data-ttu-id="4db99-155">qualities</span><span class="sxs-lookup"><span data-stu-id="4db99-155">qualities</span></span>|<span data-ttu-id="4db99-156">[coleção rubricQuality](rubricquality.md)</span><span class="sxs-lookup"><span data-stu-id="4db99-156">[rubricQuality](rubricquality.md) collection</span></span>|<span data-ttu-id="4db99-157">A coleção de qualidades que com o mesmo rubric.</span><span class="sxs-lookup"><span data-stu-id="4db99-157">The collection of qualities making up this rubric.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4db99-158">Relações</span><span class="sxs-lookup"><span data-stu-id="4db99-158">Relationships</span></span>

<span data-ttu-id="4db99-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4db99-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4db99-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4db99-160">JSON representation</span></span>

<span data-ttu-id="4db99-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4db99-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubric",
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