---
title: tipo de recurso toneInfo
description: Um único evento DTMF.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a370fe4b6375cecd563c797a21096d02d741e52e
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865633"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="ab780-103">tipo de recurso toneInfo</span><span class="sxs-lookup"><span data-stu-id="ab780-103">toneInfo resource type</span></span>

<span data-ttu-id="ab780-104">Um único evento DTMF.</span><span class="sxs-lookup"><span data-stu-id="ab780-104">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="ab780-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ab780-105">Properties</span></span>

| <span data-ttu-id="ab780-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ab780-106">Property</span></span>       | <span data-ttu-id="ab780-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="ab780-107">Type</span></span>    | <span data-ttu-id="ab780-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab780-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ab780-109">SequenceId</span><span class="sxs-lookup"><span data-stu-id="ab780-109">sequenceId</span></span> | <span data-ttu-id="ab780-110">Int64</span><span class="sxs-lookup"><span data-stu-id="ab780-110">Int64</span></span> | <span data-ttu-id="ab780-111">Um identificador incremental usado para ordenar eventos de DTMF.</span><span class="sxs-lookup"><span data-stu-id="ab780-111">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="ab780-112">bipe</span><span class="sxs-lookup"><span data-stu-id="ab780-112">tone</span></span> | <span data-ttu-id="ab780-113">String</span><span class="sxs-lookup"><span data-stu-id="ab780-113">String</span></span> | <span data-ttu-id="ab780-114">Os valores possíveis são `tone0`: `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`,`pound`</span><span class="sxs-lookup"><span data-stu-id="ab780-114">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ab780-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ab780-115">JSON representation</span></span>

<span data-ttu-id="ab780-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ab780-116">The following is a JSON representation of the resource.</span></span>

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
