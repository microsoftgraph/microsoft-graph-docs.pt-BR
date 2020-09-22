---
title: tipo de recurso plannerCategoryDescriptions
description: 'O recurso **plannerCategoryDescriptions** representa os rótulos descritivos das categorias que foram definidas para um plano. Ele pertence ao objeto Plan details. Pode haver até 6 categorias definidas. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: ab0fd1b58da0fd3e0b21212897c3f7a3e2d185b5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026528"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="dc6af-105">tipo de recurso plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="dc6af-105">plannerCategoryDescriptions resource type</span></span>

<span data-ttu-id="dc6af-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc6af-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc6af-107">O recurso **plannerCategoryDescriptions** representa os rótulos descritivos das categorias que foram definidas para um plano.</span><span class="sxs-lookup"><span data-stu-id="dc6af-107">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan.</span></span> <span data-ttu-id="dc6af-108">Ele pertence ao objeto [Plan Details](plannerplandetails.md) .</span><span class="sxs-lookup"><span data-stu-id="dc6af-108">It belongs to the [plan details](plannerplandetails.md) object.</span></span> <span data-ttu-id="dc6af-109">Pode haver até 6 categorias definidas.</span><span class="sxs-lookup"><span data-stu-id="dc6af-109">There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="dc6af-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc6af-110">Properties</span></span>
| <span data-ttu-id="dc6af-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc6af-111">Property</span></span>     | <span data-ttu-id="dc6af-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc6af-112">Type</span></span>   |<span data-ttu-id="dc6af-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc6af-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc6af-114">category1</span><span class="sxs-lookup"><span data-stu-id="dc6af-114">category1</span></span>|<span data-ttu-id="dc6af-115">String</span><span class="sxs-lookup"><span data-stu-id="dc6af-115">String</span></span>|<span data-ttu-id="dc6af-116">O rótulo associado à categoria 1</span><span class="sxs-lookup"><span data-stu-id="dc6af-116">The label associated with Category 1</span></span>|
|<span data-ttu-id="dc6af-117">category2</span><span class="sxs-lookup"><span data-stu-id="dc6af-117">category2</span></span>|<span data-ttu-id="dc6af-118">String</span><span class="sxs-lookup"><span data-stu-id="dc6af-118">String</span></span>|<span data-ttu-id="dc6af-119">O rótulo associado à categoria 2</span><span class="sxs-lookup"><span data-stu-id="dc6af-119">The label associated with Category 2</span></span>|
|<span data-ttu-id="dc6af-120">category3</span><span class="sxs-lookup"><span data-stu-id="dc6af-120">category3</span></span>|<span data-ttu-id="dc6af-121">String</span><span class="sxs-lookup"><span data-stu-id="dc6af-121">String</span></span>|<span data-ttu-id="dc6af-122">O rótulo associado à categoria 3</span><span class="sxs-lookup"><span data-stu-id="dc6af-122">The label associated with Category 3</span></span>|
|<span data-ttu-id="dc6af-123">category4</span><span class="sxs-lookup"><span data-stu-id="dc6af-123">category4</span></span>|<span data-ttu-id="dc6af-124">String</span><span class="sxs-lookup"><span data-stu-id="dc6af-124">String</span></span>|<span data-ttu-id="dc6af-125">O rótulo associado à categoria 4</span><span class="sxs-lookup"><span data-stu-id="dc6af-125">The label associated with Category 4</span></span>|
|<span data-ttu-id="dc6af-126">category5</span><span class="sxs-lookup"><span data-stu-id="dc6af-126">category5</span></span>|<span data-ttu-id="dc6af-127">String</span><span class="sxs-lookup"><span data-stu-id="dc6af-127">String</span></span>|<span data-ttu-id="dc6af-128">O rótulo associado à categoria 5</span><span class="sxs-lookup"><span data-stu-id="dc6af-128">The label associated with Category 5</span></span>|
|<span data-ttu-id="dc6af-129">category6</span><span class="sxs-lookup"><span data-stu-id="dc6af-129">category6</span></span>|<span data-ttu-id="dc6af-130">String</span><span class="sxs-lookup"><span data-stu-id="dc6af-130">String</span></span>|<span data-ttu-id="dc6af-131">O rótulo associado à categoria 6</span><span class="sxs-lookup"><span data-stu-id="dc6af-131">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc6af-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc6af-132">JSON representation</span></span>
<span data-ttu-id="dc6af-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dc6af-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


