---
title: tipo de recurso de multimargem
description: Especifica as larguras de margem a serem usadas ao imprimir.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 8f89d2d4daa45d1043e3412852cdaa480223129b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048726"
---
# <a name="printmargin-complex-type"></a><span data-ttu-id="52cc5-103">tipo complexo de transmargem</span><span class="sxs-lookup"><span data-stu-id="52cc5-103">printMargin complex type</span></span>

<span data-ttu-id="52cc5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52cc5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52cc5-105">Especifica as larguras de margem a serem usadas ao imprimir.</span><span class="sxs-lookup"><span data-stu-id="52cc5-105">Specifies the margin widths to use when printing.</span></span>

## <a name="properties"></a><span data-ttu-id="52cc5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52cc5-106">Properties</span></span>
| <span data-ttu-id="52cc5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52cc5-107">Property</span></span>     | <span data-ttu-id="52cc5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="52cc5-108">Type</span></span>        | <span data-ttu-id="52cc5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="52cc5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52cc5-110">top</span><span class="sxs-lookup"><span data-stu-id="52cc5-110">top</span></span>|<span data-ttu-id="52cc5-111">Int32</span><span class="sxs-lookup"><span data-stu-id="52cc5-111">Int32</span></span>|<span data-ttu-id="52cc5-112">A margem em mícrons da borda superior.</span><span class="sxs-lookup"><span data-stu-id="52cc5-112">The margin in microns from the top edge.</span></span>|
|<span data-ttu-id="52cc5-113">bottom</span><span class="sxs-lookup"><span data-stu-id="52cc5-113">bottom</span></span>|<span data-ttu-id="52cc5-114">Int32</span><span class="sxs-lookup"><span data-stu-id="52cc5-114">Int32</span></span>|<span data-ttu-id="52cc5-115">A margem em mícrons da borda inferior.</span><span class="sxs-lookup"><span data-stu-id="52cc5-115">The margin in microns from the bottom edge.</span></span>|
|<span data-ttu-id="52cc5-116">Certo</span><span class="sxs-lookup"><span data-stu-id="52cc5-116">right</span></span>|<span data-ttu-id="52cc5-117">Int32</span><span class="sxs-lookup"><span data-stu-id="52cc5-117">Int32</span></span>|<span data-ttu-id="52cc5-118">A margem em mícrons da borda direita.</span><span class="sxs-lookup"><span data-stu-id="52cc5-118">The margin in microns from the right edge.</span></span>|
|<span data-ttu-id="52cc5-119">left</span><span class="sxs-lookup"><span data-stu-id="52cc5-119">left</span></span>|<span data-ttu-id="52cc5-120">Int32</span><span class="sxs-lookup"><span data-stu-id="52cc5-120">Int32</span></span>|<span data-ttu-id="52cc5-121">A margem em mícrons da borda esquerda.</span><span class="sxs-lookup"><span data-stu-id="52cc5-121">The margin in microns from the left edge.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52cc5-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52cc5-122">JSON representation</span></span>

<span data-ttu-id="52cc5-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52cc5-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printMargin"
}-->

```json
{
  "top": 123456,
  "bottom": 123456,
  "right": 123456,
  "left": 123456
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printMargin resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


