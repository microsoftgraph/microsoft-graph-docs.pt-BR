---
title: Tipo de recurso customTimeZone
description: Representa um fuso horário em que a transição do horário padrão para o horário de verão, ou vice-versa, não é padrão.
localization_priority: Normal
author: abheek-das
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a4d05d000b2491fcc9d02b3e39bb012e6e5f023e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130512"
---
# <a name="customtimezone-resource-type"></a>Tipo de recurso customTimeZone

Namespace: microsoft.graph

Representa um fuso horário em que a transição do horário padrão para o horário de verão, ou vice-versa, não é padrão.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| bias | Edm.Int32 | A diferença de tempo em relação ao fuso horário UTC (Tempo Universal Coordenado). Este valor está em minutos. Os fusos horários que estão adiantados em relação ao UTC têm uma diferença de tempo positiva, enquanto os atrasados têm uma diferença de tempo negativa.|
| daylightOffset | [daylightTimeZoneOffset](daylighttimezoneoffset.md) | Especifica quando o fuso horário muda do horário padrão para o horário de verão. |
| nome | string | O nome do fuso horário personalizado. |
| standardOffset | [standardTimeZoneOffset](standardtimezoneoffset.md) | Especifica quando o fuso horário muda do horário de verão para o horário padrão. |


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.timeZoneBase",
  "@odata.type": "microsoft.graph.customTimeZone"
}-->

```json
{
  "bias": "Int32",
  "daylightOffset": {"@odata.type": "microsoft.graph.daylightTimeZoneOffset"},
  "name": "string",
  "standardOffset": {"@odata.type": "microsoft.graph.standardTimeZoneOffset"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "customTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

