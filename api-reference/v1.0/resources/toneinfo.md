---
title: tipo de recurso toneInfo
description: Um único evento DTMF.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 80ffc67fcba25fabb1da3ee1c21ee805c334fa3c
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40912962"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="b15c0-103">tipo de recurso toneInfo</span><span class="sxs-lookup"><span data-stu-id="b15c0-103">toneInfo resource type</span></span>

<span data-ttu-id="b15c0-104">Um único evento DTMF.</span><span class="sxs-lookup"><span data-stu-id="b15c0-104">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="b15c0-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b15c0-105">Properties</span></span>

| <span data-ttu-id="b15c0-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b15c0-106">Property</span></span>       | <span data-ttu-id="b15c0-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b15c0-107">Type</span></span>    | <span data-ttu-id="b15c0-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b15c0-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b15c0-109">SequenceId</span><span class="sxs-lookup"><span data-stu-id="b15c0-109">sequenceId</span></span> | <span data-ttu-id="b15c0-110">Int64</span><span class="sxs-lookup"><span data-stu-id="b15c0-110">Int64</span></span> | <span data-ttu-id="b15c0-111">Um identificador incremental usado para ordenar eventos de DTMF.</span><span class="sxs-lookup"><span data-stu-id="b15c0-111">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="b15c0-112">bipe</span><span class="sxs-lookup"><span data-stu-id="b15c0-112">tone</span></span> | <span data-ttu-id="b15c0-113">String</span><span class="sxs-lookup"><span data-stu-id="b15c0-113">String</span></span> | <span data-ttu-id="b15c0-114">Os valores possíveis são `tone0`: `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`,`pound`</span><span class="sxs-lookup"><span data-stu-id="b15c0-114">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b15c0-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b15c0-115">JSON representation</span></span>

<span data-ttu-id="b15c0-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b15c0-116">The following is a JSON representation of the resource.</span></span>

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
