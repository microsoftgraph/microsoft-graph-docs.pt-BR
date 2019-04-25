---
title: tipo de recurso plannerCategoryDescriptions
description: 'O recurso **plannerCategoryDescriptions** representa os rótulos descritivos das categorias que foram definidas para um plano. Ele pertence ao objeto Plan details. Pode haver até 6 categorias definidas. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 33031dc3c688e1fefb34109cb0a4a303dbe1c183
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579027"
---
# <a name="plannercategorydescriptions-resource-type"></a><span data-ttu-id="21ea9-105">tipo de recurso plannerCategoryDescriptions</span><span class="sxs-lookup"><span data-stu-id="21ea9-105">plannerCategoryDescriptions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21ea9-106">O recurso **plannerCategoryDescriptions** representa os rótulos descritivos das categorias que foram definidas para um plano.</span><span class="sxs-lookup"><span data-stu-id="21ea9-106">The **plannerCategoryDescriptions** resource represents the descriptive labels for the categories that have been defined for a plan.</span></span> <span data-ttu-id="21ea9-107">Ele pertence ao objeto [Plan Details](plannerplandetails.md) .</span><span class="sxs-lookup"><span data-stu-id="21ea9-107">It belongs to the [plan details](plannerplandetails.md) object.</span></span> <span data-ttu-id="21ea9-108">Pode haver até 6 categorias definidas.</span><span class="sxs-lookup"><span data-stu-id="21ea9-108">There can be up to 6 categories defined.</span></span> 


## <a name="properties"></a><span data-ttu-id="21ea9-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="21ea9-109">Properties</span></span>
| <span data-ttu-id="21ea9-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="21ea9-110">Property</span></span>     | <span data-ttu-id="21ea9-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="21ea9-111">Type</span></span>   |<span data-ttu-id="21ea9-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="21ea9-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21ea9-113">category1</span><span class="sxs-lookup"><span data-stu-id="21ea9-113">category1</span></span>|<span data-ttu-id="21ea9-114">String</span><span class="sxs-lookup"><span data-stu-id="21ea9-114">String</span></span>|<span data-ttu-id="21ea9-115">O rótulo associado à categoria 1</span><span class="sxs-lookup"><span data-stu-id="21ea9-115">The label associated with Category 1</span></span>|
|<span data-ttu-id="21ea9-116">category2</span><span class="sxs-lookup"><span data-stu-id="21ea9-116">category2</span></span>|<span data-ttu-id="21ea9-117">String</span><span class="sxs-lookup"><span data-stu-id="21ea9-117">String</span></span>|<span data-ttu-id="21ea9-118">O rótulo associado à categoria 2</span><span class="sxs-lookup"><span data-stu-id="21ea9-118">The label associated with Category 2</span></span>|
|<span data-ttu-id="21ea9-119">category3</span><span class="sxs-lookup"><span data-stu-id="21ea9-119">category3</span></span>|<span data-ttu-id="21ea9-120">String</span><span class="sxs-lookup"><span data-stu-id="21ea9-120">String</span></span>|<span data-ttu-id="21ea9-121">O rótulo associado à categoria 3</span><span class="sxs-lookup"><span data-stu-id="21ea9-121">The label associated with Category 3</span></span>|
|<span data-ttu-id="21ea9-122">category4</span><span class="sxs-lookup"><span data-stu-id="21ea9-122">category4</span></span>|<span data-ttu-id="21ea9-123">String</span><span class="sxs-lookup"><span data-stu-id="21ea9-123">String</span></span>|<span data-ttu-id="21ea9-124">O rótulo associado à categoria 4</span><span class="sxs-lookup"><span data-stu-id="21ea9-124">The label associated with Category 4</span></span>|
|<span data-ttu-id="21ea9-125">category5</span><span class="sxs-lookup"><span data-stu-id="21ea9-125">category5</span></span>|<span data-ttu-id="21ea9-126">String</span><span class="sxs-lookup"><span data-stu-id="21ea9-126">String</span></span>|<span data-ttu-id="21ea9-127">O rótulo associado à categoria 5</span><span class="sxs-lookup"><span data-stu-id="21ea9-127">The label associated with Category 5</span></span>|
|<span data-ttu-id="21ea9-128">category6</span><span class="sxs-lookup"><span data-stu-id="21ea9-128">category6</span></span>|<span data-ttu-id="21ea9-129">String</span><span class="sxs-lookup"><span data-stu-id="21ea9-129">String</span></span>|<span data-ttu-id="21ea9-130">O rótulo associado à categoria 6</span><span class="sxs-lookup"><span data-stu-id="21ea9-130">The label associated with Category 6</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21ea9-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="21ea9-131">JSON representation</span></span>
<span data-ttu-id="21ea9-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="21ea9-132">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannercategorydescriptions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
