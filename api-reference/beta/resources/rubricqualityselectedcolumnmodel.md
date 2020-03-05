---
title: tipo de recurso rubricQualitySelectedColumnModel
description: Indica o rubricLevel selecionado pelo professor ao gradar um educationRubric
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9c8b6264a0373fb5b388cd95771d9360b867feb9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520988"
---
# <a name="rubricqualityselectedcolumnmodel-resource-type"></a><span data-ttu-id="fc28e-103">tipo de recurso rubricQualitySelectedColumnModel</span><span class="sxs-lookup"><span data-stu-id="fc28e-103">rubricQualitySelectedColumnModel resource type</span></span>

<span data-ttu-id="fc28e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fc28e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc28e-105">Indica o [rubricLevel](rubriclevel.md) selecionado pelo professor ao gradar um [educationRubric](educationrubric.md).</span><span class="sxs-lookup"><span data-stu-id="fc28e-105">Indicates the [rubricLevel](rubriclevel.md) selected by the teacher when grading an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fc28e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fc28e-106">Properties</span></span>

| <span data-ttu-id="fc28e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fc28e-107">Property</span></span>     | <span data-ttu-id="fc28e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc28e-108">Type</span></span>        | <span data-ttu-id="fc28e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc28e-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fc28e-110">columnId</span><span class="sxs-lookup"><span data-stu-id="fc28e-110">columnId</span></span>|<span data-ttu-id="fc28e-111">String</span><span class="sxs-lookup"><span data-stu-id="fc28e-111">String</span></span>|<span data-ttu-id="fc28e-112">ID do nível selecionado para essa qualidade.</span><span class="sxs-lookup"><span data-stu-id="fc28e-112">ID of the selected level for this quality.</span></span>|
|<span data-ttu-id="fc28e-113">qualityid</span><span class="sxs-lookup"><span data-stu-id="fc28e-113">qualityId</span></span>|<span data-ttu-id="fc28e-114">String</span><span class="sxs-lookup"><span data-stu-id="fc28e-114">String</span></span>|<span data-ttu-id="fc28e-115">ID da qualidade associada.</span><span class="sxs-lookup"><span data-stu-id="fc28e-115">ID of the associated quality.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc28e-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fc28e-116">JSON representation</span></span>

<span data-ttu-id="fc28e-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fc28e-117">The following is a JSON representation of the resource.</span></span>

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