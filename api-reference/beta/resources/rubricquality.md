---
title: tipo de recurso rubricQuality
description: Uma qualidade de um amostra rubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6f900056db140719ff5bc7902a6a7a9531cebe9b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521002"
---
# <a name="rubricquality-resource-type"></a><span data-ttu-id="bafd1-103">tipo de recurso rubricQuality</span><span class="sxs-lookup"><span data-stu-id="bafd1-103">rubricQuality resource type</span></span>

<span data-ttu-id="bafd1-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="bafd1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bafd1-105">Uma qualidade de um amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="bafd1-105">A quality of a rubric.</span></span> <span data-ttu-id="bafd1-106">Consulte [educationRubric](educationrubric.md) para obter uma descrição da relação entre as *qualidades*, *níveis*e *critérios*do amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="bafd1-106">See [educationRubric](educationrubric.md) for a description of the relationship between rubric *qualities*, *levels*, and *criteria*.</span></span>

## <a name="properties"></a><span data-ttu-id="bafd1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bafd1-107">Properties</span></span>

| <span data-ttu-id="bafd1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bafd1-108">Property</span></span>     | <span data-ttu-id="bafd1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bafd1-109">Type</span></span>        | <span data-ttu-id="bafd1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bafd1-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bafd1-111">criteria</span><span class="sxs-lookup"><span data-stu-id="bafd1-111">criteria</span></span>|<span data-ttu-id="bafd1-112">coleção [rubricCriterion](rubriccriterion.md)</span><span class="sxs-lookup"><span data-stu-id="bafd1-112">[rubricCriterion](rubriccriterion.md) collection</span></span>|<span data-ttu-id="bafd1-113">O conjunto de critérios para esta qualidade de amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="bafd1-113">The collection of criteria for this rubric quality.</span></span>|
|<span data-ttu-id="bafd1-114">description</span><span class="sxs-lookup"><span data-stu-id="bafd1-114">description</span></span>|[<span data-ttu-id="bafd1-115">itemBody</span><span class="sxs-lookup"><span data-stu-id="bafd1-115">itemBody</span></span>](itembody.md)|<span data-ttu-id="bafd1-116">A descrição dessa qualidade de amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="bafd1-116">The description of this rubric quality.</span></span>|
|<span data-ttu-id="bafd1-117">displayName</span><span class="sxs-lookup"><span data-stu-id="bafd1-117">displayName</span></span>|<span data-ttu-id="bafd1-118">String</span><span class="sxs-lookup"><span data-stu-id="bafd1-118">String</span></span>|<span data-ttu-id="bafd1-119">O nome dessa qualidade de amostra rubric.</span><span class="sxs-lookup"><span data-stu-id="bafd1-119">The name of this rubric quality.</span></span>|
|<span data-ttu-id="bafd1-120">qualityid</span><span class="sxs-lookup"><span data-stu-id="bafd1-120">qualityId</span></span>|<span data-ttu-id="bafd1-121">String</span><span class="sxs-lookup"><span data-stu-id="bafd1-121">String</span></span>|<span data-ttu-id="bafd1-122">A ID desse recurso.</span><span class="sxs-lookup"><span data-stu-id="bafd1-122">The ID of this resource.</span></span>|
|<span data-ttu-id="bafd1-123">weight</span><span class="sxs-lookup"><span data-stu-id="bafd1-123">weight</span></span>|<span data-ttu-id="bafd1-124">Único</span><span class="sxs-lookup"><span data-stu-id="bafd1-124">Single</span></span>|<span data-ttu-id="bafd1-125">Se presente, um peso numérico para essa qualidade.</span><span class="sxs-lookup"><span data-stu-id="bafd1-125">If present, a numerical weight for this quality.</span></span>  <span data-ttu-id="bafd1-126">Os pesos devem adicionar até 100.</span><span class="sxs-lookup"><span data-stu-id="bafd1-126">Weights must add up to 100.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bafd1-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bafd1-127">JSON representation</span></span>

<span data-ttu-id="bafd1-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bafd1-128">The following is a JSON representation of the resource.</span></span>

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