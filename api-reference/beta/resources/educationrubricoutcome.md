---
title: tipo de recurso educationRubricOutcome
description: Um educationOutcome que fornece uma amostra rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4640daa1bb93945463cffc9dcf54d4db23b84da1
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173255"
---
# <a name="educationrubricoutcome-resource-type"></a><span data-ttu-id="79666-103">tipo de recurso educationRubricOutcome</span><span class="sxs-lookup"><span data-stu-id="79666-103">educationRubricOutcome resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79666-104">Um [educationOutcome](educationoutcome.md) que fornece um amostra rubric com a classificação.</span><span class="sxs-lookup"><span data-stu-id="79666-104">An [educationOutcome](educationoutcome.md) that provides a graded rubric.</span></span>

## <a name="methods"></a><span data-ttu-id="79666-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="79666-105">Methods</span></span>

| <span data-ttu-id="79666-106">Método</span><span class="sxs-lookup"><span data-stu-id="79666-106">Method</span></span>       | <span data-ttu-id="79666-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="79666-107">Return Type</span></span> | <span data-ttu-id="79666-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="79666-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="79666-109">Atualizar educationOutcome</span><span class="sxs-lookup"><span data-stu-id="79666-109">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="79666-110">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="79666-110">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="79666-111">Atualize o objeto educationOutcome.</span><span class="sxs-lookup"><span data-stu-id="79666-111">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="79666-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79666-112">Properties</span></span>

| <span data-ttu-id="79666-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79666-113">Property</span></span>     | <span data-ttu-id="79666-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="79666-114">Type</span></span>        | <span data-ttu-id="79666-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="79666-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="79666-116">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="79666-116">lastModifiedBy</span></span>|[<span data-ttu-id="79666-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="79666-117">identitySet</span></span>](identityset.md)|<span data-ttu-id="79666-118">O último usuário a modificar o recurso.</span><span class="sxs-lookup"><span data-stu-id="79666-118">The last user to modify the resource.</span></span>|
|<span data-ttu-id="79666-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="79666-119">lastModifiedDateTime</span></span>|<span data-ttu-id="79666-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79666-120">DateTimeOffset</span></span>|<span data-ttu-id="79666-121">Momento no momento em que o recurso foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="79666-121">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="79666-122">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="79666-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="79666-123">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="79666-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="79666-124">publishedRubricQualityFeedback</span><span class="sxs-lookup"><span data-stu-id="79666-124">publishedRubricQualityFeedback</span></span>|<span data-ttu-id="79666-125">coleção [rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)</span><span class="sxs-lookup"><span data-stu-id="79666-125">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="79666-126">Uma cópia da propriedade rubricQualityFeedback que é feita quando a nota é liberada para o aluno.</span><span class="sxs-lookup"><span data-stu-id="79666-126">A copy of the rubricQualityFeedback property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="79666-127">publishedRubricQualitySelectedLevels</span><span class="sxs-lookup"><span data-stu-id="79666-127">publishedRubricQualitySelectedLevels</span></span>|<span data-ttu-id="79666-128">coleção [rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)</span><span class="sxs-lookup"><span data-stu-id="79666-128">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="79666-129">Uma cópia da propriedade rubricQualitySelectedLevels que é feita quando a nota é liberada para o aluno.</span><span class="sxs-lookup"><span data-stu-id="79666-129">A copy of the rubricQualitySelectedLevels property that is made when the grade is released to the student.</span></span>|
|<span data-ttu-id="79666-130">rubricQualityFeedback</span><span class="sxs-lookup"><span data-stu-id="79666-130">rubricQualityFeedback</span></span>|<span data-ttu-id="79666-131">coleção [rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md)</span><span class="sxs-lookup"><span data-stu-id="79666-131">[rubricQualityFeedbackModel](rubricqualityfeedbackmodel.md) collection</span></span>|<span data-ttu-id="79666-132">Uma coleção de comentários específicos para cada qualidade desse amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="79666-132">A collection of specific feedback for each quality of this rubric.</span></span>|
|<span data-ttu-id="79666-133">rubricQualitySelectedLevels</span><span class="sxs-lookup"><span data-stu-id="79666-133">rubricQualitySelectedLevels</span></span>|<span data-ttu-id="79666-134">coleção [rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md)</span><span class="sxs-lookup"><span data-stu-id="79666-134">[rubricQualitySelectedColumnModel](rubricqualityselectedcolumnmodel.md) collection</span></span>|<span data-ttu-id="79666-135">O nível que o professor selecionou para cada qualidade e, ao mesmo tempo, grada esta atribuição.</span><span class="sxs-lookup"><span data-stu-id="79666-135">The level that the teacher has selected for each quality while grading this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79666-136">Relações</span><span class="sxs-lookup"><span data-stu-id="79666-136">Relationships</span></span>

<span data-ttu-id="79666-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79666-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79666-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79666-138">JSON representation</span></span>

<span data-ttu-id="79666-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79666-139">The following is a JSON representation of the resource.</span></span>

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