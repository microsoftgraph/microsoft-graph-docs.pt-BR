---
title: tipo de recurso educationRubricOutcome
description: Um educationOutcome que fornece uma amostra rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 93e6585a6963a6f31c2613e2f2e12cce7246b7d8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501007"
---
# <a name="educationrubricoutcome-resource-type"></a><span data-ttu-id="dfb40-103">tipo de recurso educationRubricOutcome</span><span class="sxs-lookup"><span data-stu-id="dfb40-103">educationRubricOutcome resource type</span></span>

<span data-ttu-id="dfb40-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dfb40-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfb40-105">Um [educationOutcome](educationoutcome.md) que fornece um amostra rubric com a classificação.</span><span class="sxs-lookup"><span data-stu-id="dfb40-105">An [educationOutcome](educationoutcome.md) that provides a graded rubric.</span></span>

## <a name="methods"></a><span data-ttu-id="dfb40-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="dfb40-106">Methods</span></span>

| <span data-ttu-id="dfb40-107">Método</span><span class="sxs-lookup"><span data-stu-id="dfb40-107">Method</span></span>       | <span data-ttu-id="dfb40-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dfb40-108">Return Type</span></span> | <span data-ttu-id="dfb40-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfb40-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="dfb40-110">Atualizar educationOutcome</span><span class="sxs-lookup"><span data-stu-id="dfb40-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="dfb40-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="dfb40-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="dfb40-112">Atualize o objeto educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="dfb40-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="dfb40-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dfb40-113">Properties</span></span>

| <span data-ttu-id="dfb40-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dfb40-114">Property</span></span>     | <span data-ttu-id="dfb40-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="dfb40-115">Type</span></span>        | <span data-ttu-id="dfb40-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="dfb40-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dfb40-117">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="dfb40-117">lastModifiedBy</span></span>|[<span data-ttu-id="dfb40-118">identitySet</span><span class="sxs-lookup"><span data-stu-id="dfb40-118">identitySet</span></span>](identityset.md)|<span data-ttu-id="dfb40-119">O último usuário a modificar o recurso.</span><span class="sxs-lookup"><span data-stu-id="dfb40-119">The last user to modify the resource.</span></span>|
|<span data-ttu-id="dfb40-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dfb40-120">lastModifiedDateTime</span></span>|<span data-ttu-id="dfb40-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfb40-121">DateTimeOffset</span></span>|<span data-ttu-id="dfb40-122">Momento no momento em que o recurso foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="dfb40-122">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="dfb40-123">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="dfb40-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="dfb40-124">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="dfb40-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="dfb40-125">publishedRubricQualityFeedback</span><span class="sxs-lookup"><span data-stu-id="dfb40-125">publishedRubricQualityFeedback</span></span>|<span data-ttu-id="dfb40-126">coleção [rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)</span><span class="sxs-lookup"><span data-stu-id="dfb40-126">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="dfb40-127">Uma cópia da propriedade rubricQualityFeedback que é feita quando a nota é liberada para o aluno.</span><span class="sxs-lookup"><span data-stu-id="dfb40-127">A copy of the rubricQualityFeedback property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="dfb40-128">publishedRubricQualitySelectedLevels</span><span class="sxs-lookup"><span data-stu-id="dfb40-128">publishedRubricQualitySelectedLevels</span></span>|<span data-ttu-id="dfb40-129">coleção [rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)</span><span class="sxs-lookup"><span data-stu-id="dfb40-129">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="dfb40-130">Uma cópia da propriedade rubricQualitySelectedLevels que é feita quando a nota é liberada para o aluno.</span><span class="sxs-lookup"><span data-stu-id="dfb40-130">A copy of the rubricQualitySelectedLevels property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="dfb40-131">rubricQualityFeedback</span><span class="sxs-lookup"><span data-stu-id="dfb40-131">rubricQualityFeedback</span></span>|<span data-ttu-id="dfb40-132">coleção [rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)</span><span class="sxs-lookup"><span data-stu-id="dfb40-132">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="dfb40-133">Uma coleção de comentários específicos para cada qualidade desse amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="dfb40-133">A collection of specific feedback for each quality of this rubric.</span></span>|
|<span data-ttu-id="dfb40-134">rubricQualitySelectedLevels</span><span class="sxs-lookup"><span data-stu-id="dfb40-134">rubricQualitySelectedLevels</span></span>|<span data-ttu-id="dfb40-135">coleção [rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)</span><span class="sxs-lookup"><span data-stu-id="dfb40-135">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="dfb40-136">O nível que o professor selecionou para cada qualidade e, ao mesmo tempo, grada esta atribuição.</span><span class="sxs-lookup"><span data-stu-id="dfb40-136">The level that the teacher has selected for each quality while grading this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfb40-137">Relações</span><span class="sxs-lookup"><span data-stu-id="dfb40-137">Relationships</span></span>

<span data-ttu-id="dfb40-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dfb40-138">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfb40-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dfb40-139">JSON representation</span></span>

<span data-ttu-id="dfb40-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dfb40-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationRubricOutcome",
  "baseType": "",
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