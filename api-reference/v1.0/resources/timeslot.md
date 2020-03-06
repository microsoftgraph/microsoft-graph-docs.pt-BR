---
title: Tipo de recurso timeSlot
description: Um período de tempo.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: f106b81acf827c2e99b5ea22afe81afd3d4c7313
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533454"
---
# <a name="timeslot-resource-type"></a>Tipo de recurso timeSlot

Namespace: microsoft.graph

Representa um intervalo de tempo para uma reunião.

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
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|end|[dateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário em que um período começa. |
|iniciar|[dateTimeTimeZone](datetimetimezone.md)|A data, a hora e o fuso horário que um período termina.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
