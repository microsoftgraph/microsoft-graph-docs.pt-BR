---
title: tipo de recurso meetingParticipants
description: Participantes de uma reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 171d24629c8a219f788ad17cdf97874bbf299a62
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006624"
---
# <a name="meetingparticipants-resource-type"></a>tipo de recurso meetingParticipants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Participantes de uma reunião.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    | Descrição|
|:---------------|:--------|:----------|
| attendees | coleção [meetingParticipantInfo](meetingparticipantinfo.md) |  |
| organizer | [meetingParticipantInfo](meetingparticipantinfo.md) |  |
| produtores | coleção [meetingParticipantInfo](meetingparticipantinfo.md) | Somente para reunião de transmissão. |
| colaboradores | coleção [meetingParticipantInfo](meetingparticipantinfo.md) | Somente para reunião de transmissão. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipants"
}-->
```json
{
  "attendees": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"},
  "producers": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "contributors": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipants resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
