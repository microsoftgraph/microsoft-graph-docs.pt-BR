---
title: tipo de recurso integerRange
description: Representa um intervalo inclusivo de inteiros descritos por dois limites Int64.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: ee879104878189ddcaf51f65e4e127a61798c811
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986053"
---
# <a name="integerrange-resource-type"></a><span data-ttu-id="6540c-103">tipo de recurso integerRange</span><span class="sxs-lookup"><span data-stu-id="6540c-103">integerRange resource type</span></span>

<span data-ttu-id="6540c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6540c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6540c-105">Representa um intervalo inclusivo de inteiros descritos por dois limites Int64.</span><span class="sxs-lookup"><span data-stu-id="6540c-105">Represents an inclusive range of integers described by two Int64 boundaries.</span></span>

## <a name="properties"></a><span data-ttu-id="6540c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6540c-106">Properties</span></span>
| <span data-ttu-id="6540c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6540c-107">Property</span></span>     | <span data-ttu-id="6540c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6540c-108">Type</span></span>        | <span data-ttu-id="6540c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6540c-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6540c-110">iniciar</span><span class="sxs-lookup"><span data-stu-id="6540c-110">start</span></span>|<span data-ttu-id="6540c-111">Int64</span><span class="sxs-lookup"><span data-stu-id="6540c-111">Int64</span></span>|<span data-ttu-id="6540c-112">O limite inferior inclusivo do intervalo de inteiros.</span><span class="sxs-lookup"><span data-stu-id="6540c-112">The inclusive lower bound of the integer range.</span></span>|
|<span data-ttu-id="6540c-113">end</span><span class="sxs-lookup"><span data-stu-id="6540c-113">end</span></span>|<span data-ttu-id="6540c-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6540c-114">Int64</span></span>|<span data-ttu-id="6540c-115">O limite superior inclusivo do intervalo de inteiros.</span><span class="sxs-lookup"><span data-stu-id="6540c-115">The inclusive upper bound of the integer range.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6540c-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6540c-116">JSON representation</span></span>

<span data-ttu-id="6540c-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6540c-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.integerRange"
}-->

```json
{
    "start": 12345,
    "end": 12345
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

