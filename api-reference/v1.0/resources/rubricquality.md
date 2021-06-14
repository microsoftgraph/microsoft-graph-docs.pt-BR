---
title: Tipo de recurso rubricQuality
description: Uma qualidade de uma rubrica.
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 82fdb8fa226ab6eb2c38b1e49e12904ff26b6491
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911375"
---
# <a name="rubricquality-resource-type"></a><span data-ttu-id="7aa60-103">Tipo de recurso rubricQuality</span><span class="sxs-lookup"><span data-stu-id="7aa60-103">rubricQuality resource type</span></span>

<span data-ttu-id="7aa60-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7aa60-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7aa60-105">Uma qualidade de uma rubrica.</span><span class="sxs-lookup"><span data-stu-id="7aa60-105">A quality of a rubric.</span></span> 

<span data-ttu-id="7aa60-106">Consulte [educationRubric](educationrubric.md) para ver uma descrição da relação entre as qualidades *rubricas,* níveis e *critérios.*</span><span class="sxs-lookup"><span data-stu-id="7aa60-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="7aa60-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7aa60-107">Properties</span></span>

| <span data-ttu-id="7aa60-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7aa60-108">Property</span></span>     | <span data-ttu-id="7aa60-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7aa60-109">Type</span></span>        | <span data-ttu-id="7aa60-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aa60-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7aa60-111">criteria</span><span class="sxs-lookup"><span data-stu-id="7aa60-111">criteria</span></span>|<span data-ttu-id="7aa60-112">[Coleção rubricCriterion](rubriccriterion.md)</span><span class="sxs-lookup"><span data-stu-id="7aa60-112">[rubricCriterion](rubriccriterion.md) collection</span></span>|<span data-ttu-id="7aa60-113">A coleção de critérios para essa qualidade rubrica.</span><span class="sxs-lookup"><span data-stu-id="7aa60-113">The collection of criteria for this rubric quality.</span></span>|
|<span data-ttu-id="7aa60-114">descrição</span><span class="sxs-lookup"><span data-stu-id="7aa60-114">description</span></span>|[<span data-ttu-id="7aa60-115">itemBody</span><span class="sxs-lookup"><span data-stu-id="7aa60-115">itemBody</span></span>](itembody.md)|<span data-ttu-id="7aa60-116">A descrição dessa qualidade rubrica.</span><span class="sxs-lookup"><span data-stu-id="7aa60-116">The description of this rubric quality.</span></span>|
|<span data-ttu-id="7aa60-117">displayName</span><span class="sxs-lookup"><span data-stu-id="7aa60-117">displayName</span></span>|<span data-ttu-id="7aa60-118">String</span><span class="sxs-lookup"><span data-stu-id="7aa60-118">String</span></span>|<span data-ttu-id="7aa60-119">O nome dessa qualidade rubrica.</span><span class="sxs-lookup"><span data-stu-id="7aa60-119">The name of this rubric quality.</span></span>|
|<span data-ttu-id="7aa60-120">qualityId</span><span class="sxs-lookup"><span data-stu-id="7aa60-120">qualityId</span></span>|<span data-ttu-id="7aa60-121">String</span><span class="sxs-lookup"><span data-stu-id="7aa60-121">String</span></span>|<span data-ttu-id="7aa60-122">A ID desse recurso.</span><span class="sxs-lookup"><span data-stu-id="7aa60-122">The ID of this resource.</span></span>|
|<span data-ttu-id="7aa60-123">weight</span><span class="sxs-lookup"><span data-stu-id="7aa60-123">weight</span></span>|<span data-ttu-id="7aa60-124">Único</span><span class="sxs-lookup"><span data-stu-id="7aa60-124">Single</span></span>|<span data-ttu-id="7aa60-125">Se presente, um peso numérico para essa qualidade.</span><span class="sxs-lookup"><span data-stu-id="7aa60-125">If present, a numerical weight for this quality.</span></span>  <span data-ttu-id="7aa60-126">Os pesos devem adicionar até 100.</span><span class="sxs-lookup"><span data-stu-id="7aa60-126">Weights must add up to 100.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7aa60-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7aa60-127">JSON representation</span></span>

<span data-ttu-id="7aa60-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7aa60-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQuality",
  "baseType": null
}-->

```json
{
  "criteria": [{"@odata.type": "microsoft.graph.rubricCriterion"}],
  "description": {"@odata.type": "microsoft.graph.itemBody"},
  "displayName": "String",
  "qualityId": "String",
  "weight": "Double"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

