---
title: Tipo de recurso timeSlot
description: Um período de tempo.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 08ba0c696c511e5a80c25262ba9d1d4cab6d2231aabea01cec0f573d70cd6ec1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189195"
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
|end|[dateTimeTimeZone](datetimetimezone.md)|A data, hora e fuso horário que um período começa. |
|iniciar|[dateTimeTimeZone](datetimetimezone.md)|A data, hora e fuso horário que um período termina.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

