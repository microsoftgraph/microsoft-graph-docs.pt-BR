---
title: tipo de recurso resourceReference
description: Tipo complexo contendo propriedades de insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: fac5ec3b40467034a583933a6e09399e91badfe0
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427393"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="ba9a7-103">tipo de recurso resourceReference</span><span class="sxs-lookup"><span data-stu-id="ba9a7-103">resourceReference resource type</span></span>

<span data-ttu-id="ba9a7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba9a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba9a7-105">Tipo complexo contendo propriedades de item de [informações](iteminsights.md)</span><span class="sxs-lookup"><span data-stu-id="ba9a7-105">Complex type containing properties of [itemInsights](iteminsights.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba9a7-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba9a7-106">JSON representation</span></span>

<span data-ttu-id="ba9a7-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ba9a7-107">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="ba9a7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba9a7-108">Properties</span></span>

| <span data-ttu-id="ba9a7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba9a7-109">Property</span></span>      | <span data-ttu-id="ba9a7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba9a7-110">Type</span></span>      | <span data-ttu-id="ba9a7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba9a7-111">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="ba9a7-112">webUrl</span><span class="sxs-lookup"><span data-stu-id="ba9a7-112">webUrl</span></span>        | <span data-ttu-id="ba9a7-113">String</span><span class="sxs-lookup"><span data-stu-id="ba9a7-113">String</span></span>    | <span data-ttu-id="ba9a7-114">Uma URL que conduz ao item referenciado.</span><span class="sxs-lookup"><span data-stu-id="ba9a7-114">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="ba9a7-115">id</span><span class="sxs-lookup"><span data-stu-id="ba9a7-115">id</span></span>            | <span data-ttu-id="ba9a7-116">String</span><span class="sxs-lookup"><span data-stu-id="ba9a7-116">String</span></span>    | <span data-ttu-id="ba9a7-117">O identificador exclusivo do item.</span><span class="sxs-lookup"><span data-stu-id="ba9a7-117">The item's unique identifier.</span></span>           |
| <span data-ttu-id="ba9a7-118">tipo</span><span class="sxs-lookup"><span data-stu-id="ba9a7-118">type</span></span>          | <span data-ttu-id="ba9a7-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ba9a7-119">String</span></span>    | <span data-ttu-id="ba9a7-120">Um valor String que pode ser usado para classificar o item, como "Microsoft. Graph. driveItem"</span><span class="sxs-lookup"><span data-stu-id="ba9a7-120">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
