---
title: Tipo de recurso educationRubricOutcome
description: Um educationOutcome que fornece uma rubrica de notas.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2f71fb170eaa6259a4b478aa5ffbbc340a306bde
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912178"
---
# <a name="educationrubricoutcome-resource-type"></a><span data-ttu-id="664ae-103">Tipo de recurso educationRubricOutcome</span><span class="sxs-lookup"><span data-stu-id="664ae-103">educationRubricOutcome resource type</span></span>

<span data-ttu-id="664ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="664ae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="664ae-105">Um [educationOutcome](educationoutcome.md) que fornece uma rubrica de notas.</span><span class="sxs-lookup"><span data-stu-id="664ae-105">An [educationOutcome](educationoutcome.md) that provides a graded rubric.</span></span>

## <a name="methods"></a><span data-ttu-id="664ae-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="664ae-106">Methods</span></span>

| <span data-ttu-id="664ae-107">Método</span><span class="sxs-lookup"><span data-stu-id="664ae-107">Method</span></span>       | <span data-ttu-id="664ae-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="664ae-108">Return Type</span></span> | <span data-ttu-id="664ae-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="664ae-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="664ae-110">Atualizar educationOutcome</span><span class="sxs-lookup"><span data-stu-id="664ae-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="664ae-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="664ae-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="664ae-112">Atualizar o objeto educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="664ae-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="664ae-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="664ae-113">Properties</span></span>

| <span data-ttu-id="664ae-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="664ae-114">Property</span></span>     | <span data-ttu-id="664ae-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="664ae-115">Type</span></span>        | <span data-ttu-id="664ae-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="664ae-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="664ae-117">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="664ae-117">lastModifiedBy</span></span>|[<span data-ttu-id="664ae-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="664ae-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="664ae-119">O último usuário a modificar o recurso.</span><span class="sxs-lookup"><span data-stu-id="664ae-119">The last user to modify the resource.</span></span>|
|<span data-ttu-id="664ae-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="664ae-120">lastModifiedDateTime</span></span>|<span data-ttu-id="664ae-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="664ae-121">DateTimeOffset</span></span>|<span data-ttu-id="664ae-122">Momento no tempo em que o recurso foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="664ae-122">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="664ae-123">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="664ae-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="664ae-124">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="664ae-124">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="664ae-125">publishedRubricQualityFeedback</span><span class="sxs-lookup"><span data-stu-id="664ae-125">publishedRubricQualityFeedback</span></span>|<span data-ttu-id="664ae-126">[Coleção rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)</span><span class="sxs-lookup"><span data-stu-id="664ae-126">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="664ae-127">Uma cópia da propriedade rubricQualityFeedback que é feita quando a nota é liberada para o aluno.</span><span class="sxs-lookup"><span data-stu-id="664ae-127">A copy of the rubricQualityFeedback property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="664ae-128">publishedRubricQualitySelectedLevels</span><span class="sxs-lookup"><span data-stu-id="664ae-128">publishedRubricQualitySelectedLevels</span></span>|<span data-ttu-id="664ae-129">[Coleção rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)</span><span class="sxs-lookup"><span data-stu-id="664ae-129">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="664ae-130">Uma cópia da propriedade rubricQualitySelectedLevels que é feita quando a nota é liberada para o aluno.</span><span class="sxs-lookup"><span data-stu-id="664ae-130">A copy of the rubricQualitySelectedLevels property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="664ae-131">rubricQualityFeedback</span><span class="sxs-lookup"><span data-stu-id="664ae-131">rubricQualityFeedback</span></span>|<span data-ttu-id="664ae-132">[Coleção rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)</span><span class="sxs-lookup"><span data-stu-id="664ae-132">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="664ae-133">Uma coleção de comentários específicos para cada qualidade desse rubric.</span><span class="sxs-lookup"><span data-stu-id="664ae-133">A collection of specific feedback for each quality of this rubric.</span></span>|
|<span data-ttu-id="664ae-134">rubricQualitySelectedLevels</span><span class="sxs-lookup"><span data-stu-id="664ae-134">rubricQualitySelectedLevels</span></span>|<span data-ttu-id="664ae-135">[Coleção rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)</span><span class="sxs-lookup"><span data-stu-id="664ae-135">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="664ae-136">O nível que o professor selecionou para cada qualidade durante a classificação dessa atribuição.</span><span class="sxs-lookup"><span data-stu-id="664ae-136">The level that the teacher has selected for each quality while grading this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="664ae-137">Relações</span><span class="sxs-lookup"><span data-stu-id="664ae-137">Relationships</span></span>

<span data-ttu-id="664ae-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="664ae-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="664ae-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="664ae-139">JSON representation</span></span>

<span data-ttu-id="664ae-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="664ae-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubricOutcome",
  "keyProperty": "id"
}-->

```json
{
  "publishedRubricQualityFeedback": [{"@odata.type": "microsoft.graph.rubricQualityFeedbackModel"}],
  "publishedRubricQualitySelectedLevels": [{"@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel"}],
  "rubricQualityFeedback": [{"@odata.type": "microsoft.graph.rubricQualityFeedbackModel"}],
  "rubricQualitySelectedLevels": [{"@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationRubricOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

