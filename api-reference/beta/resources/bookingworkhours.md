---
title: tipo de recurso bookingWorkHours
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: cfc15d65e840d7634c5c9134c5fc36a244f73286
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507884"
---
# <a name="bookingworkhours-resource-type"></a>tipo de recurso bookingWorkHours

Namespace: Microsoft. Graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa o conjunto de horas de trabalho em um único dia da semana, para um [bookingBusiness](bookingbusiness.md) ou [bookingStaffMember](bookingstaffmember.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|dia|String| O dia da semana representado por esta instância. Os valores possíveis são: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|Intervalos|coleção [bookingWorkTimeSlot](bookingworktimeslot.md)|Uma lista de horários de início/término durante um dia.|

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
