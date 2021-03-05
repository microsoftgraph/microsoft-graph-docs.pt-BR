---
title: Tipo de recurso timeSlot
description: Um período de tempo.
localization_priority: Normal
doc_type: resourcePageType
author: vrod9429
ms.prod: outlook
ms.openlocfilehash: f531add7d16fc5d1922a40e7341894b7fedd6535
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472040"
---
# <a name="timeslot-resource-type"></a>Tipo de recurso timeSlot

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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
|end|[dateTimeTimeZone](datetimetimezone.md)|A data, hora e fuso horário que um período começa. |
|iniciar|[dateTimeTimeZone](datetimetimezone.md)|A data, hora e fuso horário que um período termina.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


