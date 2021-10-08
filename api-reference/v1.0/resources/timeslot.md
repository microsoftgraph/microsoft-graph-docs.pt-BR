---
title: Tipo de recurso timeSlot
description: Um período de tempo.
ms.localizationpriority: medium
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 055797d4dccb4d74f8fe55ce8c0a75c9ab27e417
ms.sourcegitcommit: 6cea9bc17d3859e475a74c4a6f661f848e837e89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/08/2021
ms.locfileid: "60240744"
---
# <a name="timeslot-resource-type"></a>Tipo de recurso timeSlot

Namespace: microsoft.graph

Representa um intervalo de tempo para uma reunião.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|end|[dateTimeTimeZone](datetimetimezone.md)|A data, hora e fuso horário que um período termina. |
|iniciar|[dateTimeTimeZone](datetimetimezone.md)|A data, hora e fuso horário que um período começa.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeSlot"
}-->

```json
{
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

