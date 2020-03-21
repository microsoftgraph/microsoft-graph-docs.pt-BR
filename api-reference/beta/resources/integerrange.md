---
title: tipo de recurso integerRange
description: Representa um intervalo inclusivo de inteiros descritos por dois limites Int64.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: c7c3a14e8b8772a0bc319d8415046f3e10871f52
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895489"
---
# <a name="integerrange-resource-type"></a><span data-ttu-id="c508f-103">tipo de recurso integerRange</span><span class="sxs-lookup"><span data-stu-id="c508f-103">integerRange resource type</span></span>

<span data-ttu-id="c508f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c508f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c508f-105">Representa um intervalo inclusivo de inteiros descritos por dois limites Int64.</span><span class="sxs-lookup"><span data-stu-id="c508f-105">Represents an inclusive range of integers described by two Int64 boundaries.</span></span>

## <a name="properties"></a><span data-ttu-id="c508f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c508f-106">Properties</span></span>
| <span data-ttu-id="c508f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c508f-107">Property</span></span>     | <span data-ttu-id="c508f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c508f-108">Type</span></span>        | <span data-ttu-id="c508f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c508f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c508f-110">minimum</span><span class="sxs-lookup"><span data-stu-id="c508f-110">minimum</span></span>|<span data-ttu-id="c508f-111">Int64</span><span class="sxs-lookup"><span data-stu-id="c508f-111">Int64</span></span>|<span data-ttu-id="c508f-112">O limite inferior inclusivo do intervalo de inteiros.</span><span class="sxs-lookup"><span data-stu-id="c508f-112">The inclusive lower bound of the integer range.</span></span>|
|<span data-ttu-id="c508f-113">maximum</span><span class="sxs-lookup"><span data-stu-id="c508f-113">maximum</span></span>|<span data-ttu-id="c508f-114">Int64</span><span class="sxs-lookup"><span data-stu-id="c508f-114">Int64</span></span>|<span data-ttu-id="c508f-115">O limite superior inclusivo do intervalo de inteiros.</span><span class="sxs-lookup"><span data-stu-id="c508f-115">The inclusive upper bound of the integer range.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c508f-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c508f-116">JSON representation</span></span>

<span data-ttu-id="c508f-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c508f-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.integerRange"
}-->

```json
{
    "minimum": 12345,
    "maximum": 12345
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "integerRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->