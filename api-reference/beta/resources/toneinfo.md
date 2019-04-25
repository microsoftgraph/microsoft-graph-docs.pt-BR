---
title: tipo de recurso toneInfo
description: Um único evento DTMF.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: f58548f8f075494c6601db2962d88fb6cabb59ce
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522647"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="e2d20-103">tipo de recurso toneInfo</span><span class="sxs-lookup"><span data-stu-id="e2d20-103">toneInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2d20-104">Um único evento DTMF.</span><span class="sxs-lookup"><span data-stu-id="e2d20-104">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="e2d20-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e2d20-105">Properties</span></span>

| <span data-ttu-id="e2d20-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2d20-106">Property</span></span>       | <span data-ttu-id="e2d20-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2d20-107">Type</span></span>    | <span data-ttu-id="e2d20-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2d20-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e2d20-109">SequenceId</span><span class="sxs-lookup"><span data-stu-id="e2d20-109">sequenceId</span></span> | <span data-ttu-id="e2d20-110">Int64</span><span class="sxs-lookup"><span data-stu-id="e2d20-110">Int64</span></span> | <span data-ttu-id="e2d20-111">Um identificador incremental usado para ordenar eventos de DTMF.</span><span class="sxs-lookup"><span data-stu-id="e2d20-111">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="e2d20-112">bipe</span><span class="sxs-lookup"><span data-stu-id="e2d20-112">tone</span></span> | <span data-ttu-id="e2d20-113">String</span><span class="sxs-lookup"><span data-stu-id="e2d20-113">String</span></span> | <span data-ttu-id="e2d20-114">Os valores possíveis são `tone0`: `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`,,,,,,,,,.</span><span class="sxs-lookup"><span data-stu-id="e2d20-114">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e2d20-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e2d20-115">JSON representation</span></span>

<span data-ttu-id="e2d20-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e2d20-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/toneinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
