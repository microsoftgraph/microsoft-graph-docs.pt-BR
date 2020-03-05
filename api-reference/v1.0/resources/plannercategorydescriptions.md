---
title: tipo de recurso plannerCategoryDescriptions
description: 'O recurso **plannerCategoryDescriptions** representa os rótulos descritivos das categorias que foram definidas para um plano. Ele pertence ao objeto Plan details. Pode haver até 6 categorias definidas. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d0ef4c4f91c4b2f8017a7b7555785c9dd10d082a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447133"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="4cd04-105">tipo de recurso plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="4cd04-105">plannerCategoryDescriptions resource type</span></span>

<span data-ttu-id="4cd04-106">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4cd04-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4cd04-107">O recurso **plannerCategoryDescriptions** representa os rótulos descritivos das categorias que foram definidas para um plano.</span><span class="sxs-lookup"><span data-stu-id="4cd04-107">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan.</span></span> <span data-ttu-id="4cd04-108">Ele pertence ao objeto [Plan Details](plannerplandetails.md) .</span><span class="sxs-lookup"><span data-stu-id="4cd04-108">It belongs to the [plan details](plannerplandetails.md) object.</span></span> <span data-ttu-id="4cd04-109">Pode haver até 6 categorias definidas.</span><span class="sxs-lookup"><span data-stu-id="4cd04-109">There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="4cd04-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4cd04-110">Properties</span></span>
| <span data-ttu-id="4cd04-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4cd04-111">Property</span></span>     | <span data-ttu-id="4cd04-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="4cd04-112">Type</span></span>   |<span data-ttu-id="4cd04-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cd04-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4cd04-114">category1</span><span class="sxs-lookup"><span data-stu-id="4cd04-114">category1</span></span>|<span data-ttu-id="4cd04-115">String</span><span class="sxs-lookup"><span data-stu-id="4cd04-115">String</span></span>|<span data-ttu-id="4cd04-116">O rótulo associado à categoria 1</span><span class="sxs-lookup"><span data-stu-id="4cd04-116">The label associated with Category 1</span></span>|
|<span data-ttu-id="4cd04-117">category2</span><span class="sxs-lookup"><span data-stu-id="4cd04-117">category2</span></span>|<span data-ttu-id="4cd04-118">String</span><span class="sxs-lookup"><span data-stu-id="4cd04-118">String</span></span>|<span data-ttu-id="4cd04-119">O rótulo associado à categoria 2</span><span class="sxs-lookup"><span data-stu-id="4cd04-119">The label associated with Category 2</span></span>|
|<span data-ttu-id="4cd04-120">category3</span><span class="sxs-lookup"><span data-stu-id="4cd04-120">category3</span></span>|<span data-ttu-id="4cd04-121">String</span><span class="sxs-lookup"><span data-stu-id="4cd04-121">String</span></span>|<span data-ttu-id="4cd04-122">O rótulo associado à categoria 3</span><span class="sxs-lookup"><span data-stu-id="4cd04-122">The label associated with Category 3</span></span>|
|<span data-ttu-id="4cd04-123">category4</span><span class="sxs-lookup"><span data-stu-id="4cd04-123">category4</span></span>|<span data-ttu-id="4cd04-124">String</span><span class="sxs-lookup"><span data-stu-id="4cd04-124">String</span></span>|<span data-ttu-id="4cd04-125">O rótulo associado à categoria 4</span><span class="sxs-lookup"><span data-stu-id="4cd04-125">The label associated with Category 4</span></span>|
|<span data-ttu-id="4cd04-126">category5</span><span class="sxs-lookup"><span data-stu-id="4cd04-126">category5</span></span>|<span data-ttu-id="4cd04-127">String</span><span class="sxs-lookup"><span data-stu-id="4cd04-127">String</span></span>|<span data-ttu-id="4cd04-128">O rótulo associado à categoria 5</span><span class="sxs-lookup"><span data-stu-id="4cd04-128">The label associated with Category 5</span></span>|
|<span data-ttu-id="4cd04-129">category6</span><span class="sxs-lookup"><span data-stu-id="4cd04-129">category6</span></span>|<span data-ttu-id="4cd04-130">String</span><span class="sxs-lookup"><span data-stu-id="4cd04-130">String</span></span>|<span data-ttu-id="4cd04-131">O rótulo associado à categoria 6</span><span class="sxs-lookup"><span data-stu-id="4cd04-131">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4cd04-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4cd04-132">JSON representation</span></span>
<span data-ttu-id="4cd04-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4cd04-133">Here is a JSON representation of the resource.</span></span>

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
