---
title: Tipo de recurso daylightTimeZoneOffset
description: Especifica quando um fuso horário muda do horário padrão para o horário de verão.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: calendar
author: abheek-das
ms.openlocfilehash: 06d816085d13a6e921ebbdd98a9a18d72ecf289f
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65898053"
---
# <a name="daylighttimezoneoffset-resource-type"></a>Tipo de recurso daylightTimeZoneOffset

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica quando um fuso horário muda do horário padrão para o horário de verão.

Por exemplo, se um fuso horário estiver especificado com as seguintes propriedades:

- **bias** como 300
- **daylightBias** como -100
- **dayOccurrence** como 4
- **dayOfWeek** como "domingo"
- **month** como 5
- **time** como 02:00:00 _ **year** como 0, significa que a hora durante o horário de verão é +300-100=200 minutos adiantada ao UTC. A transição do fuso horário de horário de verão para o horário padrão ocorre às 2 da manhã no quarto domingo de maio, todos os anos.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| daylightBias | Edm.Int32 | A diferença de horário em relação ao UTC (Tempo Universal Coordenado) para o horário de verão. Este valor está em minutos.  |
| dayOccurrence | Edm.Int32 | Representa a enésima ocorrência do dia da semana em que a transição do horário padrão para o horário de verão acontece. |
| dayOfWeek | string | Representa o dia da semana em que a transição do horário padrão para o horário de verão acontece. |
| month | Edm.Int32 | Representa o mês do ano em que a transição do horário padrão para o horário de verão acontece. |
| time | Edm.TimeOfDay | Representa a hora do dia em que a transição do horário padrão para o horário de verão acontece. |
| year | Edm.Int32 | Representa com que frequência, em anos, a transição do horário padrão para o horário de verão acontece. Por exemplo, um valor 0 significa todos os anos.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.daylightTimeZoneOffset"
}-->

```json
{
  "daylightBias": "Int32",
  "dayOccurrence": "Int32",
  "dayOfWeek": "string",
  "month": "Int32",
  "time": "TimeOfDay",
  "year": "Int32"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "daylightTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


