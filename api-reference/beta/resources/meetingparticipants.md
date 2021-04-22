---
title: Tipo de recurso meetingParticipants
description: Participantes em uma reunião.
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 93ca3d73518f9739cc3115c80efd2aec551629b5
ms.sourcegitcommit: 6e7d9987a255f1bee04f196a4a7e37f56621bfb8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2021
ms.locfileid: "51944160"
---
# <a name="meetingparticipants-resource-type"></a>Tipo de recurso meetingParticipants

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Participantes em uma reunião.

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo                                                           | Descrição                           |
| :------------------------ | :------------------------------------------------------------- | :------------------------------------ |
| attendees                 | [coleção meetingParticipantInfo](meetingparticipantinfo.md) | Informações dos participantes da reunião. |
| organizer                 | [meetingParticipantInfo](meetingparticipantinfo.md)            | Informações do organizador da reunião. |
| produtores (preterido)    | [coleção meetingParticipantInfo](meetingparticipantinfo.md) | Somente para a reunião de transmissão.           |
| colaboradores (preterido) | [coleção meetingParticipantInfo](meetingparticipantinfo.md) | Somente para a reunião de transmissão.           |

> [!CAUTION]
> As **propriedades de produtores** **e** colaboradores são preteridas. Todos os participantes da reunião são retornados **na coleção de participantes.** Use a **propriedade role** de [meetingParticipantInfo](meetingparticipantinfo.md) para identificar a função de reunião do participante.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingParticipants"
}-->
```json
{
  "attendees": [{"@odata.type": "#microsoft.graph.meetingParticipantInfo"}],
  "organizer": {"@odata.type": "#microsoft.graph.meetingParticipantInfo"},
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


