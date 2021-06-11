---
title: Tipo de recurso meetingParticipants
description: Participantes em uma reunião.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8ee5cf115a80c642f5442230d7111dfaeffca930
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896617"
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


