---
title: tipo de recurso de multimargem
description: Especifica as larguras de margem a serem usadas ao imprimir.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 4d7399f45138d6ab7d82f33e6577e7d08967ad15
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863695"
---
# <a name="printmargin-complex-type"></a><span data-ttu-id="ee79c-103">tipo complexo de transmargem</span><span class="sxs-lookup"><span data-stu-id="ee79c-103">printMargin complex type</span></span>

<span data-ttu-id="ee79c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee79c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee79c-105">Especifica as larguras de margem a serem usadas ao imprimir.</span><span class="sxs-lookup"><span data-stu-id="ee79c-105">Specifies the margin widths to use when printing.</span></span>

## <a name="properties"></a><span data-ttu-id="ee79c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee79c-106">Properties</span></span>
| <span data-ttu-id="ee79c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee79c-107">Property</span></span>     | <span data-ttu-id="ee79c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee79c-108">Type</span></span>        | <span data-ttu-id="ee79c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee79c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ee79c-110">top</span><span class="sxs-lookup"><span data-stu-id="ee79c-110">top</span></span>|<span data-ttu-id="ee79c-111">Int32</span><span class="sxs-lookup"><span data-stu-id="ee79c-111">Int32</span></span>|<span data-ttu-id="ee79c-112">A margem em mícrons da borda superior.</span><span class="sxs-lookup"><span data-stu-id="ee79c-112">The margin in microns from the top edge.</span></span>|
|<span data-ttu-id="ee79c-113">bottom</span><span class="sxs-lookup"><span data-stu-id="ee79c-113">bottom</span></span>|<span data-ttu-id="ee79c-114">Int32</span><span class="sxs-lookup"><span data-stu-id="ee79c-114">Int32</span></span>|<span data-ttu-id="ee79c-115">A margem em mícrons da borda inferior.</span><span class="sxs-lookup"><span data-stu-id="ee79c-115">The margin in microns from the bottom edge.</span></span>|
|<span data-ttu-id="ee79c-116">Certo</span><span class="sxs-lookup"><span data-stu-id="ee79c-116">right</span></span>|<span data-ttu-id="ee79c-117">Int32</span><span class="sxs-lookup"><span data-stu-id="ee79c-117">Int32</span></span>|<span data-ttu-id="ee79c-118">A margem em mícrons da borda direita.</span><span class="sxs-lookup"><span data-stu-id="ee79c-118">The margin in microns from the right edge.</span></span>|
|<span data-ttu-id="ee79c-119">left</span><span class="sxs-lookup"><span data-stu-id="ee79c-119">left</span></span>|<span data-ttu-id="ee79c-120">Int32</span><span class="sxs-lookup"><span data-stu-id="ee79c-120">Int32</span></span>|<span data-ttu-id="ee79c-121">A margem em mícrons da borda esquerda.</span><span class="sxs-lookup"><span data-stu-id="ee79c-121">The margin in microns from the left edge.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee79c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee79c-122">JSON representation</span></span>

<span data-ttu-id="ee79c-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee79c-123">The following is a JSON representation of the resource.</span></span>

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
