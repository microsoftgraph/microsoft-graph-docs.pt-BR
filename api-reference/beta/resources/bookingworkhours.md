---
title: Tipo de recurso bookingWorkHours
description: Representa o conjunto de horários de trabalho em um único dia da semana, para um bookingBusiness ou bookingStaffMember.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: d503d23cd8f6652e4e25c4f03e73a348baecd310
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526174"
---
# <a name="bookingworkhours-resource-type"></a>Tipo de recurso bookingWorkHours

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa o conjunto de horários de trabalho em um único dia da semana, para [um bookingBusiness](bookingbusiness.md) ou [bookingStaffMember](bookingstaffmember.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|dia|Cadeia de caracteres| O dia da semana representado por essa instância. Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|timeSlots|[Coleção bookingWorkTimeSlot](bookingworktimeslot.md)|Uma lista de horários de início/término durante um dia.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingWorkHours"
}-->

```json
{
  "day": "String",
  "timeSlots": [{"@odata.type": "microsoft.graph.bookingWorkTimeSlot"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingWorkHours resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


