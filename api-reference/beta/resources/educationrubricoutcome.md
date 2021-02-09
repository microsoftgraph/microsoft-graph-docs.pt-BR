---
title: Tipo de recurso educationRubricOutcome
description: Um educationOutcome que fornece um rubric de notas
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c8132159fa70c175a46a43a13ebce981299f2431
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161905"
---
# <a name="educationrubricoutcome-resource-type"></a><span data-ttu-id="1d533-103">Tipo de recurso educationRubricOutcome</span><span class="sxs-lookup"><span data-stu-id="1d533-103">educationRubricOutcome resource type</span></span>

<span data-ttu-id="1d533-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d533-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d533-105">Um [educationOutcome](educationoutcome.md) que fornece um rubric de notas.</span><span class="sxs-lookup"><span data-stu-id="1d533-105">An [educationOutcome](educationoutcome.md) that provides a graded rubric.</span></span>

## <a name="methods"></a><span data-ttu-id="1d533-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="1d533-106">Methods</span></span>

| <span data-ttu-id="1d533-107">Método</span><span class="sxs-lookup"><span data-stu-id="1d533-107">Method</span></span>       | <span data-ttu-id="1d533-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1d533-108">Return Type</span></span> | <span data-ttu-id="1d533-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d533-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1d533-110">Atualizar educationOutcome</span><span class="sxs-lookup"><span data-stu-id="1d533-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="1d533-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="1d533-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="1d533-112">Atualize o objeto educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="1d533-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1d533-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d533-113">Properties</span></span>

| <span data-ttu-id="1d533-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d533-114">Property</span></span>     | <span data-ttu-id="1d533-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d533-115">Type</span></span>        | <span data-ttu-id="1d533-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d533-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1d533-117">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="1d533-117">lastModifiedBy</span></span>|[<span data-ttu-id="1d533-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="1d533-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="1d533-119">O último usuário a modificar o recurso.</span><span class="sxs-lookup"><span data-stu-id="1d533-119">The last user to modify the resource.</span></span>|
|<span data-ttu-id="1d533-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1d533-120">lastModifiedDateTime</span></span>|<span data-ttu-id="1d533-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1d533-121">DateTimeOffset</span></span>|<span data-ttu-id="1d533-122">Momento no tempo em que o recurso foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="1d533-122">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="1d533-123">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1d533-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1d533-124">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1d533-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1d533-125">publishedRubricQualityFeedback</span><span class="sxs-lookup"><span data-stu-id="1d533-125">publishedRubricQualityFeedback</span></span>|<span data-ttu-id="1d533-126">[Coleção rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)</span><span class="sxs-lookup"><span data-stu-id="1d533-126">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="1d533-127">Uma cópia da propriedade rubricQualityFeedback que é feita quando a nota é liberada para o aluno.</span><span class="sxs-lookup"><span data-stu-id="1d533-127">A copy of the rubricQualityFeedback property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="1d533-128">publishedRubricQualitySelectedLevels</span><span class="sxs-lookup"><span data-stu-id="1d533-128">publishedRubricQualitySelectedLevels</span></span>|<span data-ttu-id="1d533-129">[Coleção rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)</span><span class="sxs-lookup"><span data-stu-id="1d533-129">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="1d533-130">Uma cópia da propriedade rubricQualitySelectedLevels que é feita quando a nota é liberada para o aluno.</span><span class="sxs-lookup"><span data-stu-id="1d533-130">A copy of the rubricQualitySelectedLevels property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="1d533-131">rubricQualityFeedback</span><span class="sxs-lookup"><span data-stu-id="1d533-131">rubricQualityFeedback</span></span>|<span data-ttu-id="1d533-132">[Coleção rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)</span><span class="sxs-lookup"><span data-stu-id="1d533-132">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="1d533-133">Uma coleção de comentários específicos para cada qualidade dessa rubric.</span><span class="sxs-lookup"><span data-stu-id="1d533-133">A collection of specific feedback for each quality of this rubric.</span></span>|
|<span data-ttu-id="1d533-134">rubricQualitySelectedLevels</span><span class="sxs-lookup"><span data-stu-id="1d533-134">rubricQualitySelectedLevels</span></span>|<span data-ttu-id="1d533-135">[Coleção rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)</span><span class="sxs-lookup"><span data-stu-id="1d533-135">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="1d533-136">O nível que o professor selecionou para cada qualidade durante a gradação dessa atribuição.</span><span class="sxs-lookup"><span data-stu-id="1d533-136">The level that the teacher has selected for each quality while grading this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d533-137">Relações</span><span class="sxs-lookup"><span data-stu-id="1d533-137">Relationships</span></span>

<span data-ttu-id="1d533-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d533-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d533-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d533-139">JSON representation</span></span>

<span data-ttu-id="1d533-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d533-140">The following is a JSON representation of the resource.</span></span>

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

