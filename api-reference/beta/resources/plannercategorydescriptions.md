---
title: Tipo de recurso plannerCategoryDescriptions
description: 'O recurso **plannerCategoryDescriptions** representa os rótulos descritivos das categorias que foram definidas para um plano. Ele pertence ao objeto plan details. Pode haver até 6 categorias definidas. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 4175692182d115e884642ef8f9956cc4db5dae2e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930940"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="8676c-105">Tipo de recurso plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="8676c-105">plannerCategoryDescriptions resource type</span></span>

> <span data-ttu-id="8676c-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8676c-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8676c-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8676c-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8676c-p103">O recurso **plannerCategoryDescriptions** representa os rótulos descritivos das categorias que foram definidas para um plano. Ele pertence ao objeto [plan details](plannerplandetails.md). Pode haver até 6 categorias definidas.</span><span class="sxs-lookup"><span data-stu-id="8676c-p103">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan. It belongs to the [plan details](plannerplandetails.md) object. There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="8676c-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8676c-111">Properties</span></span>
| <span data-ttu-id="8676c-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8676c-112">Property</span></span>     | <span data-ttu-id="8676c-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="8676c-113">Type</span></span>   |<span data-ttu-id="8676c-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="8676c-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8676c-115">categoria1</span><span class="sxs-lookup"><span data-stu-id="8676c-115">category1</span></span>|<span data-ttu-id="8676c-116">String</span><span class="sxs-lookup"><span data-stu-id="8676c-116">String</span></span>|<span data-ttu-id="8676c-117">O rótulo associado à Categoria 1.</span><span class="sxs-lookup"><span data-stu-id="8676c-117">The label associated with Category 1</span></span>|
|<span data-ttu-id="8676c-118">categoria2</span><span class="sxs-lookup"><span data-stu-id="8676c-118">category2</span></span>|<span data-ttu-id="8676c-119">String</span><span class="sxs-lookup"><span data-stu-id="8676c-119">String</span></span>|<span data-ttu-id="8676c-120">O rótulo associado à Categoria 2.</span><span class="sxs-lookup"><span data-stu-id="8676c-120">The label associated with Category 2</span></span>|
|<span data-ttu-id="8676c-121">categoria3</span><span class="sxs-lookup"><span data-stu-id="8676c-121">category3</span></span>|<span data-ttu-id="8676c-122">String</span><span class="sxs-lookup"><span data-stu-id="8676c-122">String</span></span>|<span data-ttu-id="8676c-123">O rótulo associado à Categoria 3.</span><span class="sxs-lookup"><span data-stu-id="8676c-123">The label associated with Category 3</span></span>|
|<span data-ttu-id="8676c-124">categoria4</span><span class="sxs-lookup"><span data-stu-id="8676c-124">category4</span></span>|<span data-ttu-id="8676c-125">String</span><span class="sxs-lookup"><span data-stu-id="8676c-125">String</span></span>|<span data-ttu-id="8676c-126">O rótulo associado à Categoria 4.</span><span class="sxs-lookup"><span data-stu-id="8676c-126">The label associated with Category 4</span></span>|
|<span data-ttu-id="8676c-127">categoria5</span><span class="sxs-lookup"><span data-stu-id="8676c-127">category5</span></span>|<span data-ttu-id="8676c-128">String</span><span class="sxs-lookup"><span data-stu-id="8676c-128">String</span></span>|<span data-ttu-id="8676c-129">O rótulo associado à Categoria 5.</span><span class="sxs-lookup"><span data-stu-id="8676c-129">The label associated with Category 5</span></span>|
|<span data-ttu-id="8676c-130">categoria6</span><span class="sxs-lookup"><span data-stu-id="8676c-130">category6</span></span>|<span data-ttu-id="8676c-131">String</span><span class="sxs-lookup"><span data-stu-id="8676c-131">String</span></span>|<span data-ttu-id="8676c-132">O rótulo associado à Categoria 6.</span><span class="sxs-lookup"><span data-stu-id="8676c-132">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8676c-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8676c-133">JSON representation</span></span>
<span data-ttu-id="8676c-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8676c-134">Here is a JSON representation of the resource.</span></span>

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
