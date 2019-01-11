---
title: Tipo de recurso customTimeZone
description: Representa um fuso horário em que a transição do horário padrão para o horário de verão, ou vice-versa, não é padrão.
localization_priority: Normal
ms.openlocfilehash: bad1a190581592d2d9465284bf8ab1c41fe2370a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818268"
---
# <a name="customtimezone-resource-type"></a>Tipo de recurso customTimeZone

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um fuso horário em que a transição do horário padrão para o horário de verão, ou vice-versa, não é padrão.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| bias | Edm.Int32 | A diferença de tempo em relação ao fuso horário UTC (Tempo Universal Coordenado). Este valor está em minutos.Os fusos horários que estão adiantados em relação ao UTC têm uma diferença de tempo positiva, enquanto os atrasados têm uma diferença de tempo negativa.|
| daylightOffset | [daylightTimeZoneOffset](daylighttimezoneoffset.md) | Especifica quando o fuso horário muda do horário padrão para o horário de verão. |
| name | string | O nome do fuso horário personalizado. |
| standardOffset | [standardTimeZoneOffset](standardtimezoneoffset.md) | Especifica quando o fuso horário muda do horário de verão para o horário padrão. |


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
