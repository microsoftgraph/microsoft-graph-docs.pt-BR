---
title: tipo de recurso addIn
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 777b9e2eac1ec4052fae30b13d09aaf91a808375
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339120"
---
# <a name="addin-resource-type"></a><span data-ttu-id="72333-103">tipo de recurso addIn</span><span class="sxs-lookup"><span data-stu-id="72333-103">addIn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


## <a name="properties"></a><span data-ttu-id="72333-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="72333-104">Properties</span></span>
| <span data-ttu-id="72333-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72333-105">Property</span></span>     | <span data-ttu-id="72333-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="72333-106">Type</span></span>   |<span data-ttu-id="72333-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="72333-107">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="72333-108">id</span><span class="sxs-lookup"><span data-stu-id="72333-108">id</span></span>|<span data-ttu-id="72333-109">#c0</span><span class="sxs-lookup"><span data-stu-id="72333-109">guid</span></span>||
|<span data-ttu-id="72333-110">properties</span><span class="sxs-lookup"><span data-stu-id="72333-110">properties</span></span>|<span data-ttu-id="72333-111">Coleção [KeyValue](keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="72333-111">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="72333-112">type</span><span class="sxs-lookup"><span data-stu-id="72333-112">type</span></span>|<span data-ttu-id="72333-113">string</span><span class="sxs-lookup"><span data-stu-id="72333-113">string</span></span>||

## <a name="json-representation"></a><span data-ttu-id="72333-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="72333-114">JSON representation</span></span>

<span data-ttu-id="72333-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="72333-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addIn"
}-->

```json
{
  "id": "guid",
  "properties": [{"@odata.type": "microsoft.graph.keyValue"}],
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
