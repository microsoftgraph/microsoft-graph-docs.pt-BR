---
title: Tipo de recurso standardTimeZoneOffset
description: Especifica quando um fuso horário muda do horário de verão para o horário padrão.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: mail
author: abheek-das
ms.openlocfilehash: f9c8375431ce859df2670b457b21b2e996b25168
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66734232"
---
# <a name="standardtimezoneoffset-resource-type"></a>Tipo de recurso standardTimeZoneOffset

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica quando um fuso horário muda do horário de verão para o horário padrão.

Por exemplo, se um fuso horário estiver especificado com as seguintes propriedades:

- **dayOccurrence** como 3
- **dayOfWeek** como "Domingo"
- **month** como 10
- **time** como 02:00:00 _ **year** como 0. Isso significa que a transição do fuso horário do horário de verão para o horário padrão ocorre às 02:00:00 da manhã no quarto domingo de maio, todos os anos.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| dayOccurrence | Edm.Int32 | Representa a enésima ocorrência do dia da semana em que ocorre a transição do horário de verão para o horário padrão. |
| dayOfWeek | string | Representa o dia da semana em que ocorre a transição do horário de verão para o horário padrão. |
| month | Edm.Int32 | Representa o mês do ano em que ocorre a transição do horário de verão para o horário padrão. |
| time | Edm.TimeOfDay | Representa a hora do dia em que ocorre a transição do horário de verão para o horário padrão. |
| year | Edm.Int32 | Representa com que frequência, em anos, ocorre a mudança do horário de verão para o horário padrão. Por exemplo, um valor 0 significa todos os anos.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.standardTimeZoneOffset"
}-->

```json
{
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
  "description": "standardTimeZoneOffset resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


