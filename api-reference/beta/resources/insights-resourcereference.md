---
title: tipo de recurso resourceReference
description: Tipo complexo contendo propriedades de insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a353eb07c1aeb2fd904b9f97c8307ed0b5190470
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021851"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="926d8-103">tipo de recurso resourceReference</span><span class="sxs-lookup"><span data-stu-id="926d8-103">resourceReference resource type</span></span>

<span data-ttu-id="926d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="926d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="926d8-105">Tipo complexo contendo propriedades de item de [informações](iteminsights.md)</span><span class="sxs-lookup"><span data-stu-id="926d8-105">Complex type containing properties of [itemInsights](iteminsights.md)</span></span>

## <a name="json-representation"></a><span data-ttu-id="926d8-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="926d8-106">JSON representation</span></span>

<span data-ttu-id="926d8-107">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="926d8-107">Here is a JSON representation of the resource</span></span>
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

## <a name="properties"></a><span data-ttu-id="926d8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="926d8-108">Properties</span></span>

| <span data-ttu-id="926d8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="926d8-109">Property</span></span>      | <span data-ttu-id="926d8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="926d8-110">Type</span></span>      | <span data-ttu-id="926d8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="926d8-111">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="926d8-112">webUrl</span><span class="sxs-lookup"><span data-stu-id="926d8-112">webUrl</span></span>        | <span data-ttu-id="926d8-113">String</span><span class="sxs-lookup"><span data-stu-id="926d8-113">String</span></span>    | <span data-ttu-id="926d8-114">Uma URL que conduz ao item referenciado.</span><span class="sxs-lookup"><span data-stu-id="926d8-114">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="926d8-115">id</span><span class="sxs-lookup"><span data-stu-id="926d8-115">id</span></span>            | <span data-ttu-id="926d8-116">String</span><span class="sxs-lookup"><span data-stu-id="926d8-116">String</span></span>    | <span data-ttu-id="926d8-117">O identificador exclusivo do item.</span><span class="sxs-lookup"><span data-stu-id="926d8-117">The item's unique identifier.</span></span>           |
| <span data-ttu-id="926d8-118">tipo</span><span class="sxs-lookup"><span data-stu-id="926d8-118">type</span></span>          | <span data-ttu-id="926d8-119">String</span><span class="sxs-lookup"><span data-stu-id="926d8-119">String</span></span>    | <span data-ttu-id="926d8-120">Um valor String que pode ser usado para classificar o item, como "Microsoft. Graph. driveItem"</span><span class="sxs-lookup"><span data-stu-id="926d8-120">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |


