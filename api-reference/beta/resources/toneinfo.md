---
title: Tipo de recurso toneInfo
description: Um único evento DTMF.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2b79a0227273339d61a975c5df80b1a07b2d124f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954962"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="6b7ae-103">Tipo de recurso toneInfo</span><span class="sxs-lookup"><span data-stu-id="6b7ae-103">toneInfo resource type</span></span>

<span data-ttu-id="6b7ae-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b7ae-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b7ae-105">Um único evento DTMF.</span><span class="sxs-lookup"><span data-stu-id="6b7ae-105">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="6b7ae-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b7ae-106">Properties</span></span>

| <span data-ttu-id="6b7ae-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b7ae-107">Property</span></span>       | <span data-ttu-id="6b7ae-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b7ae-108">Type</span></span>    | <span data-ttu-id="6b7ae-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b7ae-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6b7ae-110">sequenceId</span><span class="sxs-lookup"><span data-stu-id="6b7ae-110">sequenceId</span></span> | <span data-ttu-id="6b7ae-111">Int64</span><span class="sxs-lookup"><span data-stu-id="6b7ae-111">Int64</span></span> | <span data-ttu-id="6b7ae-112">Um identificador incremental usado para ordenar eventos DTMF.</span><span class="sxs-lookup"><span data-stu-id="6b7ae-112">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="6b7ae-113">tone</span><span class="sxs-lookup"><span data-stu-id="6b7ae-113">tone</span></span> | <span data-ttu-id="6b7ae-114">tone</span><span class="sxs-lookup"><span data-stu-id="6b7ae-114">tone</span></span> | <span data-ttu-id="6b7ae-115">Os valores possíveis são: `tone0` , , , , , , , , `tone1` , , , `tone2` , , `tone3` , , , `tone4` `tone5` `tone6` , `tone7` `tone8` `tone9` `star` `pound` `a` `b` `c` `d` `flash` .</span><span class="sxs-lookup"><span data-stu-id="6b7ae-115">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6b7ae-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b7ae-116">JSON representation</span></span>

<span data-ttu-id="6b7ae-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b7ae-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.toneInfo"
}-->
```json
{
  "sequenceId": 1024,
  "tone": "tone0 | tone1 | tone2 | tone3 | tone4 | tone5 | tone6 | tone7 | tone8 | tone9 | star | pound | a | b | c | d | flash"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "toneInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


