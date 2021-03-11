---
title: Tipo de recurso educationRubric
description: Uma rubrica de classificação que pode ser anexada a uma atribuição
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2e5c9713de4da614c8bfb0f6332930edb8ad775b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721576"
---
# <a name="educationrubric-resource-type"></a><span data-ttu-id="99981-103">Tipo de recurso educationRubric</span><span class="sxs-lookup"><span data-stu-id="99981-103">educationRubric resource type</span></span>

<span data-ttu-id="99981-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99981-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99981-105">Uma rubrica de classificação que pode ser anexada a uma atribuição.</span><span class="sxs-lookup"><span data-stu-id="99981-105">A grading rubric that can be attached to an assignment.</span></span> <span data-ttu-id="99981-106">Uma rubrica é associada a um **educationUser** (professor) e anexada a um ou mais recursos **educationAssignment.**</span><span class="sxs-lookup"><span data-stu-id="99981-106">A rubric is associated with an **educationUser** (teacher), and attached to one or more **educationAssignment** resources.</span></span> 

<span data-ttu-id="99981-107">Consulte [Education rubric overview para](/graph/education-rubric-overview) obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="99981-107">See [Education rubric overview](/graph/education-rubric-overview) for more information.</span></span>

## <a name="methods"></a><span data-ttu-id="99981-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="99981-108">Methods</span></span>

| <span data-ttu-id="99981-109">Método</span><span class="sxs-lookup"><span data-stu-id="99981-109">Method</span></span>       | <span data-ttu-id="99981-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="99981-110">Return Type</span></span> | <span data-ttu-id="99981-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="99981-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="99981-112">Criar educationRubric</span><span class="sxs-lookup"><span data-stu-id="99981-112">Create educationRubric</span></span>](../api/educationuser-post-rubrics.md) | [<span data-ttu-id="99981-113">educationRubric</span><span class="sxs-lookup"><span data-stu-id="99981-113">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="99981-114">Crie um novo objeto educationRubric.</span><span class="sxs-lookup"><span data-stu-id="99981-114">Create a new educationRubric object.</span></span> |
| [<span data-ttu-id="99981-115">Obter educationRubric</span><span class="sxs-lookup"><span data-stu-id="99981-115">Get educationRubric</span></span>](../api/educationrubric-get.md) | [<span data-ttu-id="99981-116">educationRubric</span><span class="sxs-lookup"><span data-stu-id="99981-116">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="99981-117">Ler propriedades e relações do objeto educationRubric.</span><span class="sxs-lookup"><span data-stu-id="99981-117">Read properties and relationships of educationRubric object.</span></span> |
| [<span data-ttu-id="99981-118">Atualizar educationRubric</span><span class="sxs-lookup"><span data-stu-id="99981-118">Update educationRubric</span></span>](../api/educationrubric-update.md) | [<span data-ttu-id="99981-119">educationRubric</span><span class="sxs-lookup"><span data-stu-id="99981-119">educationRubric</span></span>](educationrubric.md) | <span data-ttu-id="99981-120">Atualize o objeto educationRubric.</span><span class="sxs-lookup"><span data-stu-id="99981-120">Update educationRubric object.</span></span> |
| [<span data-ttu-id="99981-121">Excluir educationRubric</span><span class="sxs-lookup"><span data-stu-id="99981-121">Delete educationRubric</span></span>](../api/educationrubric-delete.md) | <span data-ttu-id="99981-122">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="99981-122">None</span></span> | <span data-ttu-id="99981-123">Exclua o objeto educationRubric.</span><span class="sxs-lookup"><span data-stu-id="99981-123">Delete educationRubric object.</span></span> |

## <a name="properties"></a><span data-ttu-id="99981-124">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99981-124">Properties</span></span>

| <span data-ttu-id="99981-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99981-125">Property</span></span>     | <span data-ttu-id="99981-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="99981-126">Type</span></span>        | <span data-ttu-id="99981-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="99981-127">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="99981-128">createdBy</span><span class="sxs-lookup"><span data-stu-id="99981-128">createdBy</span></span>|[<span data-ttu-id="99981-129">identitySet</span><span class="sxs-lookup"><span data-stu-id="99981-129">identitySet</span></span>](identityset.md)|<span data-ttu-id="99981-130">O usuário que criou esse recurso.</span><span class="sxs-lookup"><span data-stu-id="99981-130">The user who created this resource.</span></span>|
|<span data-ttu-id="99981-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99981-131">createdDateTime</span></span>|<span data-ttu-id="99981-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99981-132">DateTimeOffset</span></span>|<span data-ttu-id="99981-133">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="99981-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="99981-134">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="99981-134">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="99981-135">description</span><span class="sxs-lookup"><span data-stu-id="99981-135">description</span></span>|[<span data-ttu-id="99981-136">itemBody</span><span class="sxs-lookup"><span data-stu-id="99981-136">itemBody</span></span>](itembody.md)|<span data-ttu-id="99981-137">A descrição dessa rubrica.</span><span class="sxs-lookup"><span data-stu-id="99981-137">The description of this rubric.</span></span>|
|<span data-ttu-id="99981-138">displayName</span><span class="sxs-lookup"><span data-stu-id="99981-138">displayName</span></span>|<span data-ttu-id="99981-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99981-139">String</span></span>|<span data-ttu-id="99981-140">O nome dessa rubrica.</span><span class="sxs-lookup"><span data-stu-id="99981-140">The name of this rubric.</span></span>|
|<span data-ttu-id="99981-141">grading</span><span class="sxs-lookup"><span data-stu-id="99981-141">grading</span></span>|[<span data-ttu-id="99981-142">educationAssignmentGradeType</span><span class="sxs-lookup"><span data-stu-id="99981-142">educationAssignmentGradeType</span></span>](educationassignmentgradetype.md)|<span data-ttu-id="99981-143">O tipo de classificação dessa rubrica -- nulo para uma rubrica sem pontos ou [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) para um rubric de pontos.</span><span class="sxs-lookup"><span data-stu-id="99981-143">The grading type of this rubric -- null for a no-points rubric, or [educationAssignmentPointsGradeType](educationassignmentpointsgradetype.md) for a points rubric.</span></span>|
|<span data-ttu-id="99981-144">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="99981-144">lastModifiedBy</span></span>|[<span data-ttu-id="99981-145">identitySet</span><span class="sxs-lookup"><span data-stu-id="99981-145">identitySet</span></span>](identityset.md)|<span data-ttu-id="99981-146">O último usuário a modificar o recurso.</span><span class="sxs-lookup"><span data-stu-id="99981-146">The last user to modify the resource.</span></span>|
|<span data-ttu-id="99981-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99981-147">lastModifiedDateTime</span></span>|<span data-ttu-id="99981-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99981-148">DateTimeOffset</span></span>|<span data-ttu-id="99981-149">Momento no tempo em que o recurso foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="99981-149">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="99981-150">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="99981-150">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="99981-151">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="99981-151">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="99981-152">levels</span><span class="sxs-lookup"><span data-stu-id="99981-152">levels</span></span>|<span data-ttu-id="99981-153">[Coleção rubricLevel](rubriclevel.md)</span><span class="sxs-lookup"><span data-stu-id="99981-153">[rubricLevel](rubriclevel.md) collection</span></span>|<span data-ttu-id="99981-154">A coleção de níveis que comem essa rubrica.</span><span class="sxs-lookup"><span data-stu-id="99981-154">The collection of levels making up this rubric.</span></span>|
|<span data-ttu-id="99981-155">qualidades</span><span class="sxs-lookup"><span data-stu-id="99981-155">qualities</span></span>|<span data-ttu-id="99981-156">[Coleção rubricQuality](rubricquality.md)</span><span class="sxs-lookup"><span data-stu-id="99981-156">[rubricQuality](rubricquality.md) collection</span></span>|<span data-ttu-id="99981-157">A coleção de qualidades que com isso é rubrica.</span><span class="sxs-lookup"><span data-stu-id="99981-157">The collection of qualities making up this rubric.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99981-158">Relações</span><span class="sxs-lookup"><span data-stu-id="99981-158">Relationships</span></span>

<span data-ttu-id="99981-159">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99981-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99981-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99981-160">JSON representation</span></span>

<span data-ttu-id="99981-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99981-161">The following is a JSON representation of the resource.</span></span>

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