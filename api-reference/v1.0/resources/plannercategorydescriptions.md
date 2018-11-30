---
title: Tipo de recurso plannerCategoryDescriptions
description: 'O recurso **plannerCategoryDescriptions** representa os rótulos descritivos das categorias que foram definidas para um plano. Ele pertence ao objeto plan details. Pode haver até 6 categorias definidas. '
ms.openlocfilehash: e71cbd1f41d23747691b3738b5a46ff302a72168
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004443"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="c4115-105">Tipo de recurso plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="c4115-105">plannerCategoryDescriptions resource type</span></span>

<span data-ttu-id="c4115-p102">O recurso **plannerCategoryDescriptions** representa os rótulos descritivos das categorias que foram definidas para um plano. Ele pertence ao objeto [plan details](plannerplandetails.md). Pode haver até 6 categorias definidas.</span><span class="sxs-lookup"><span data-stu-id="c4115-p102">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="c4115-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c4115-109">Properties</span></span>
| <span data-ttu-id="c4115-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c4115-110">Property</span></span>     | <span data-ttu-id="c4115-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="c4115-111">Type</span></span>   |<span data-ttu-id="c4115-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4115-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4115-113">categoria1</span><span class="sxs-lookup"><span data-stu-id="c4115-113">category1</span></span>|<span data-ttu-id="c4115-114">String</span><span class="sxs-lookup"><span data-stu-id="c4115-114">String</span></span>|<span data-ttu-id="c4115-115">O rótulo associado à Categoria 1.</span><span class="sxs-lookup"><span data-stu-id="c4115-115">The label associated with Category 1</span></span>|
|<span data-ttu-id="c4115-116">categoria2</span><span class="sxs-lookup"><span data-stu-id="c4115-116">category2</span></span>|<span data-ttu-id="c4115-117">String</span><span class="sxs-lookup"><span data-stu-id="c4115-117">String</span></span>|<span data-ttu-id="c4115-118">O rótulo associado à Categoria 2.</span><span class="sxs-lookup"><span data-stu-id="c4115-118">The label associated with Category 2</span></span>|
|<span data-ttu-id="c4115-119">categoria3</span><span class="sxs-lookup"><span data-stu-id="c4115-119">category3</span></span>|<span data-ttu-id="c4115-120">String</span><span class="sxs-lookup"><span data-stu-id="c4115-120">String</span></span>|<span data-ttu-id="c4115-121">O rótulo associado à Categoria 3.</span><span class="sxs-lookup"><span data-stu-id="c4115-121">The label associated with Category 3</span></span>|
|<span data-ttu-id="c4115-122">categoria4</span><span class="sxs-lookup"><span data-stu-id="c4115-122">category4</span></span>|<span data-ttu-id="c4115-123">String</span><span class="sxs-lookup"><span data-stu-id="c4115-123">String</span></span>|<span data-ttu-id="c4115-124">O rótulo associado à Categoria 4.</span><span class="sxs-lookup"><span data-stu-id="c4115-124">The label associated with Category 4</span></span>|
|<span data-ttu-id="c4115-125">categoria5</span><span class="sxs-lookup"><span data-stu-id="c4115-125">category5</span></span>|<span data-ttu-id="c4115-126">String</span><span class="sxs-lookup"><span data-stu-id="c4115-126">String</span></span>|<span data-ttu-id="c4115-127">O rótulo associado à Categoria 5.</span><span class="sxs-lookup"><span data-stu-id="c4115-127">The label associated with Category 5</span></span>|
|<span data-ttu-id="c4115-128">categoria6</span><span class="sxs-lookup"><span data-stu-id="c4115-128">category6</span></span>|<span data-ttu-id="c4115-129">String</span><span class="sxs-lookup"><span data-stu-id="c4115-129">String</span></span>|<span data-ttu-id="c4115-130">O rótulo associado à Categoria 6.</span><span class="sxs-lookup"><span data-stu-id="c4115-130">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c4115-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c4115-131">JSON representation</span></span>
<span data-ttu-id="c4115-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c4115-132">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->