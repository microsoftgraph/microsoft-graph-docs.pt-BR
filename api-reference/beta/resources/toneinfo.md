---
title: tipo de recurso toneInfo
description: Um único evento DTMF.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5555ae61920751d63a70fdb86199ffa572dcb9be
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083936"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="e734f-103">tipo de recurso toneInfo</span><span class="sxs-lookup"><span data-stu-id="e734f-103">toneInfo resource type</span></span>

<span data-ttu-id="e734f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e734f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e734f-105">Um único evento DTMF.</span><span class="sxs-lookup"><span data-stu-id="e734f-105">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="e734f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e734f-106">Properties</span></span>

| <span data-ttu-id="e734f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e734f-107">Property</span></span>       | <span data-ttu-id="e734f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e734f-108">Type</span></span>    | <span data-ttu-id="e734f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e734f-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e734f-110">SequenceId</span><span class="sxs-lookup"><span data-stu-id="e734f-110">sequenceId</span></span> | <span data-ttu-id="e734f-111">Int64</span><span class="sxs-lookup"><span data-stu-id="e734f-111">Int64</span></span> | <span data-ttu-id="e734f-112">Um identificador incremental usado para ordenar eventos de DTMF.</span><span class="sxs-lookup"><span data-stu-id="e734f-112">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="e734f-113">bipe</span><span class="sxs-lookup"><span data-stu-id="e734f-113">tone</span></span> | <span data-ttu-id="e734f-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e734f-114">String</span></span> | <span data-ttu-id="e734f-115">Os valores possíveis são:, `tone0` `tone1` , `tone2` , `tone3` , `tone4` , `tone5` ,,,,,,,,,,,,,,, `tone6` `tone7` `tone8` `tone9` `star` `pound` `a` , `b` , `c` , `d` , `flash` .</span><span class="sxs-lookup"><span data-stu-id="e734f-115">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e734f-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e734f-116">JSON representation</span></span>

<span data-ttu-id="e734f-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e734f-117">The following is a JSON representation of the resource.</span></span>

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


