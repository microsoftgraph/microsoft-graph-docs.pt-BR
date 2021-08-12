---
title: Tipo de recurso toneInfo
description: Um único evento DTMF.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: eba7ef5b7251712da0c91ecc9f006bbf3e1c5e80eaa86c1ea53942e815c9df4b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124000"
---
# <a name="toneinfo-resource-type"></a>Tipo de recurso toneInfo

Namespace: microsoft.graph

Um único evento DTMF.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    | Descrição|
|:---------------|:--------|:----------|
| sequenceId | Int64 | Um identificador incremental usado para ordenar eventos DTMF. |
| tone | tone | Os valores possíveis são: `tone0` , , , , , , , , `tone1` , , , `tone2` , , `tone3` , , , `tone4` `tone5` `tone6` , `tone7` `tone8` `tone9` `star` `pound` `a` `b` `c` `d` `flash` . |

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

