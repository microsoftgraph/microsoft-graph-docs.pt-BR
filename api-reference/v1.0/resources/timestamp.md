---
title: tipo de recurso da carimbo de hora
description: Data e hora informações para um ponto no tempo.
localization_priority: Normal
ms.openlocfilehash: c63b3bba93f4b108a8eb9943d3fc2a1b2961f06c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888799"
---
# <a name="timestamp-resource-type"></a>tipo de recurso da carimbo de hora

Data e hora informações para um ponto no tempo.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|data|Data|A parte da data do carimbo de hora.|
|time|TimeOfDay|A parte do tempo do carimbo de hora.|
|timeZone|Cadeia de caracteres|A porção de fuso horário da carimbo de hora, o que é uma das áreas longitudinal 24 no mundo.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
