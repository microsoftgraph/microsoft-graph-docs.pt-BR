---
title: Tipo de recurso bookingWorkTimeSlot
description: Define os horários de início e término do trabalho.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 119062c301844f297a57c47829ffab4465ea4ec4
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525019"
---
# <a name="bookingworktimeslot-resource-type"></a>Tipo de recurso bookingWorkTimeSlot

Namespace: microsoft.graph

Define os horários de início e término do trabalho.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|endTime|TimeOfDay|A hora do dia em que o trabalho é interrompido. Por exemplo, 17:00:00.0000000.|
|startTime|TimeOfDay|A hora do dia em que o trabalho é iniciado. Por exemplo, 08:00:00.0000000.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingWorkTimeSlot"
}-->

```json
{
  "endTime": "String (timestamp)",
  "startTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingWorkTimeSlot resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


