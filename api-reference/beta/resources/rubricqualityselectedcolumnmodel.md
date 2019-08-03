---
title: tipo de recurso rubricQualitySelectedColumnModel
description: Indica o rubricLevel selecionado pelo professor ao gradar um educationRubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6fd6ff5d9def23a6a6fb180c8d12398437e5dce0
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173290"
---
# <a name="rubricqualityselectedcolumnmodel-resource-type"></a><span data-ttu-id="0e485-103">tipo de recurso rubricQualitySelectedColumnModel</span><span class="sxs-lookup"><span data-stu-id="0e485-103">rubricQualitySelectedColumnModel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e485-104">Indica o [rubricLevel](rubriclevel.md) selecionado pelo professor ao gradar um [educationRubric](educationrubric.md).</span><span class="sxs-lookup"><span data-stu-id="0e485-104">Indicates the [rubricLevel](rubriclevel.md) selected by the teacher when grading an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0e485-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e485-105">Properties</span></span>

| <span data-ttu-id="0e485-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e485-106">Property</span></span>     | <span data-ttu-id="0e485-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e485-107">Type</span></span>        | <span data-ttu-id="0e485-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e485-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0e485-109">columnId</span><span class="sxs-lookup"><span data-stu-id="0e485-109">columnId</span></span>|<span data-ttu-id="0e485-110">String</span><span class="sxs-lookup"><span data-stu-id="0e485-110">String</span></span>|<span data-ttu-id="0e485-111">ID do nível selecionado para essa qualidade.</span><span class="sxs-lookup"><span data-stu-id="0e485-111">ID of the selected level for this quality.</span></span>|
|<span data-ttu-id="0e485-112">qualityid</span><span class="sxs-lookup"><span data-stu-id="0e485-112">qualityId</span></span>|<span data-ttu-id="0e485-113">String</span><span class="sxs-lookup"><span data-stu-id="0e485-113">String</span></span>|<span data-ttu-id="0e485-114">ID da qualidade associada.</span><span class="sxs-lookup"><span data-stu-id="0e485-114">ID of the associated quality.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0e485-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e485-115">JSON representation</span></span>

<span data-ttu-id="0e485-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e485-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel",
  "baseType": null
}-->

```json
{
  "columnId": "String",
  "qualityId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQualitySelectedColumnModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->