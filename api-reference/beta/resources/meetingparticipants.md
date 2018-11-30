---
title: tipo de recurso de meetingParticipants
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 4f91c9198018e903eccff7e8fe07d6668d9fd2c9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040712"
---
# <a name="meetingparticipants-resource-type"></a>tipo de recurso de meetingParticipants

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    | Descrição|
|:---------------|:--------|:----------|
| attendees | coleção [meetingParticipantInfo](meetingparticipantinfo.md) |  |
| organizer | [meetingParticipantInfo](meetingparticipantinfo.md) |  |

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
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingParticipants resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
