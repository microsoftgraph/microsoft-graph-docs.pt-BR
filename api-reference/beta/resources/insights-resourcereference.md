---
title: tipo de recurso resourceReference
description: Tipo complexo contendo propriedades de insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: accd2b0b12f8068ea990fbd611b46053f66d6de4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339980"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="c6bcd-103">tipo de recurso resourceReference</span><span class="sxs-lookup"><span data-stu-id="c6bcd-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6bcd-104">Tipo complexo contendo propriedades de [](officegraphinsights.md)insights.</span><span class="sxs-lookup"><span data-stu-id="c6bcd-104">Complex type containing properties of [insights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6bcd-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c6bcd-105">JSON representation</span></span>

<span data-ttu-id="c6bcd-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="c6bcd-106">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.resourceReference"
}-->
```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="c6bcd-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c6bcd-107">Properties</span></span>

| <span data-ttu-id="c6bcd-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c6bcd-108">Property</span></span>      | <span data-ttu-id="c6bcd-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c6bcd-109">Type</span></span>      | <span data-ttu-id="c6bcd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6bcd-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="c6bcd-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="c6bcd-111">webUrl</span></span>        | <span data-ttu-id="c6bcd-112">String</span><span class="sxs-lookup"><span data-stu-id="c6bcd-112">String</span></span>    | <span data-ttu-id="c6bcd-113">Uma URL que conduz ao item referenciado.</span><span class="sxs-lookup"><span data-stu-id="c6bcd-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="c6bcd-114">id</span><span class="sxs-lookup"><span data-stu-id="c6bcd-114">id</span></span>            | <span data-ttu-id="c6bcd-115">String</span><span class="sxs-lookup"><span data-stu-id="c6bcd-115">String</span></span>    | <span data-ttu-id="c6bcd-116">O identificador exclusivo do item.</span><span class="sxs-lookup"><span data-stu-id="c6bcd-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="c6bcd-117">type</span><span class="sxs-lookup"><span data-stu-id="c6bcd-117">type</span></span>          | <span data-ttu-id="c6bcd-118">String</span><span class="sxs-lookup"><span data-stu-id="c6bcd-118">String</span></span>    | <span data-ttu-id="c6bcd-119">Um valor String que pode ser usado para classificar o item, como "Microsoft. Graph. driveItem"</span><span class="sxs-lookup"><span data-stu-id="c6bcd-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
