---
title: Tipo de recurso meetingTimeSuggestion
description: 'Uma sugestão de reunião que inclui informações como o horário da reunião, a probabilidade de presença, individual '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 4c5a4cb4d094e7fd7fe9b0e56227a556c6e5b5d1
ms.sourcegitcommit: a90abf5b89dbbdfefb1b7794d1f12c6e2bfb0cda
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936259"
---
# <a name="meetingtimesuggestion-resource-type"></a>Tipo de recurso meetingTimeSuggestion

Uma sugestão de reunião que inclui informações como o horário da reunião, a probabilidade de presença, a disponibilidade individual e os locais de reunião disponíveis.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestion"
}-->

```json
{
  "attendeeAvailability": [{"@odata.type": "microsoft.graph.attendeeAvailability"}],
  "confidence": 100.0,
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "meetingTimeSlot": {"@odata.type": "microsoft.graph.timeSlot"},
  "order": 1024,
  "organizerAvailability": "String",
  "suggestionReason": "String"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|attendeeAvailability|Coleção [attendeeAvailability](attendeeavailability.md)|Uma matriz que mostra o status de disponibilidade de cada participante para essa sugestão da reunião.|
|confidence|Double|Uma porcentagem que representa a probabilidade de todos os participantes comparecerem.|
|locations|Coleção [location](location.md)|Uma matriz que especifica o nome e a localização geográfica de cada local da reunião para esta sugestão de reunião.|
|meetingTimeSlot|[timeSlot](timeslot.md)|Um período de tempo sugerido para a reunião.|
|Ordene|Int32|Ordem das sugestões de horário de reunião classificadas pelo valor de confiança computado de alto para baixo e, em seguida, por cronologia, se houver sugestões com a mesma confiança. |
|organizerAvailability|freeBusyStatus| Disponibilidade do organizador da reunião para essa sugestão de reunião. Os valores possíveis são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|
|suggestionReason|Cadeia de caracteres|Razão da sugestão de horário da reunião.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestion resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
