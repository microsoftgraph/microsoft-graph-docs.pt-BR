---
title: tipo de recurso rubricQualitySelectedColumnModel
description: Indica o rubricLevel selecionado pelo professor ao gradar um educationRubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a381ad878f16dab6197c72bd19d6f5aeee86f4a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016055"
---
# <a name="rubricqualityselectedcolumnmodel-resource-type"></a><span data-ttu-id="5caa1-103">tipo de recurso rubricQualitySelectedColumnModel</span><span class="sxs-lookup"><span data-stu-id="5caa1-103">rubricQualitySelectedColumnModel resource type</span></span>

<span data-ttu-id="5caa1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5caa1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5caa1-105">Indica o [rubricLevel](rubriclevel.md) selecionado pelo professor ao gradar um [educationRubric](educationrubric.md).</span><span class="sxs-lookup"><span data-stu-id="5caa1-105">Indicates the [rubricLevel](rubriclevel.md) selected by the teacher when grading an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="5caa1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5caa1-106">Properties</span></span>

| <span data-ttu-id="5caa1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5caa1-107">Property</span></span>     | <span data-ttu-id="5caa1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5caa1-108">Type</span></span>        | <span data-ttu-id="5caa1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5caa1-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5caa1-110">columnId</span><span class="sxs-lookup"><span data-stu-id="5caa1-110">columnId</span></span>|<span data-ttu-id="5caa1-111">String</span><span class="sxs-lookup"><span data-stu-id="5caa1-111">String</span></span>|<span data-ttu-id="5caa1-112">ID do nível selecionado para essa qualidade.</span><span class="sxs-lookup"><span data-stu-id="5caa1-112">ID of the selected level for this quality.</span></span>|
|<span data-ttu-id="5caa1-113">qualityid</span><span class="sxs-lookup"><span data-stu-id="5caa1-113">qualityId</span></span>|<span data-ttu-id="5caa1-114">String</span><span class="sxs-lookup"><span data-stu-id="5caa1-114">String</span></span>|<span data-ttu-id="5caa1-115">ID da qualidade associada.</span><span class="sxs-lookup"><span data-stu-id="5caa1-115">ID of the associated quality.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5caa1-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5caa1-116">JSON representation</span></span>

<span data-ttu-id="5caa1-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5caa1-117">The following is a JSON representation of the resource.</span></span>

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

