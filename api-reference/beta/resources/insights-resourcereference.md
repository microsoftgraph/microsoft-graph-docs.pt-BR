---
title: tipo de recurso resourceReference
description: Tipo complexo contendo propriedades de insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 06a8d99ba01a8a3fd3d171b800345f81b0819de0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005720"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="2d7a6-103">tipo de recurso resourceReference</span><span class="sxs-lookup"><span data-stu-id="2d7a6-103">resourceReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d7a6-104">Tipo complexo contendo propriedades de [](officegraphinsights.md)insights.</span><span class="sxs-lookup"><span data-stu-id="2d7a6-104">Complex type containing properties of [insights](officegraphinsights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d7a6-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d7a6-105">JSON representation</span></span>

<span data-ttu-id="2d7a6-106">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="2d7a6-106">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="2d7a6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d7a6-107">Properties</span></span>

| <span data-ttu-id="2d7a6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d7a6-108">Property</span></span>      | <span data-ttu-id="2d7a6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d7a6-109">Type</span></span>      | <span data-ttu-id="2d7a6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d7a6-110">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="2d7a6-111">webUrl</span><span class="sxs-lookup"><span data-stu-id="2d7a6-111">webUrl</span></span>        | <span data-ttu-id="2d7a6-112">String</span><span class="sxs-lookup"><span data-stu-id="2d7a6-112">String</span></span>    | <span data-ttu-id="2d7a6-113">Uma URL que conduz ao item referenciado.</span><span class="sxs-lookup"><span data-stu-id="2d7a6-113">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="2d7a6-114">id</span><span class="sxs-lookup"><span data-stu-id="2d7a6-114">id</span></span>            | <span data-ttu-id="2d7a6-115">String</span><span class="sxs-lookup"><span data-stu-id="2d7a6-115">String</span></span>    | <span data-ttu-id="2d7a6-116">O identificador exclusivo do item.</span><span class="sxs-lookup"><span data-stu-id="2d7a6-116">The item's unique identifier.</span></span>           |
| <span data-ttu-id="2d7a6-117">type</span><span class="sxs-lookup"><span data-stu-id="2d7a6-117">type</span></span>          | <span data-ttu-id="2d7a6-118">String</span><span class="sxs-lookup"><span data-stu-id="2d7a6-118">String</span></span>    | <span data-ttu-id="2d7a6-119">Um valor String que pode ser usado para classificar o item, como "Microsoft. Graph. driveItem"</span><span class="sxs-lookup"><span data-stu-id="2d7a6-119">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
