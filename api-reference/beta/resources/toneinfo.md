---
title: tipo de recurso toneInfo
description: Um único evento DTMF.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0eaa4b4159ffd5e7455b1155a7f3cd82c89b19aa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964246"
---
# <a name="toneinfo-resource-type"></a>tipo de recurso toneInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um único evento DTMF.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    | Descrição|
|:---------------|:--------|:----------|
| SequenceId | Int64 | Um identificador incremental usado para ordenar eventos de DTMF. |
| bipe | String | Os valores possíveis são `tone0`: `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`,,,,,,,,,. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

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
