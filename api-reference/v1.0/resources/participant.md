---
title: tipo de recurso participante
description: Representa o tipo de participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0c5004ea45cf44818c30ffe02dc48a1f6851e64a
ms.sourcegitcommit: d12bd5435c198bcd096e1f7f6a2716f4a04631cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/19/2020
ms.locfileid: "48137110"
---
# <a name="participant-resource-type"></a>tipo de recurso participante

Namespace: microsoft.graph

Representa um participante em uma chamada.

## <a name="methods"></a>Métodos

| Método                                                 | Tipo de retorno                                                 | Descrição                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [Lista de participantes](../api/participant-get.md)          | [participante](participant.md)                               | Recupere uma lista de objetos **participantes** na chamada. |
| [Obter participante](../api/participant-get.md)           | [participante](participant.md)                               | Leia as propriedades do objeto **participante** . |
| [Excluir participante](../api/participant-delete.md)         | Nenhum   | Excluir um participante de uma chamada.                  |
| [Convidar](../api/participant-invite.md)                 | [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md)                        | Convidar um participante para a chamada.              |
| [Ativar mudo para participante](../api/participant-mute.md)         | [muteParticipantOperation](muteparticipantoperation.md)     | Tirar o áudio de um participante em uma chamada.                  |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                                     | Descrição                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| id                   | Cadeia de caracteres                                   | A ID do participante.                                          |
| informações                  | [participantInfo](participantinfo.md)    | O participante do participante.                          |
| isInLobby            | Booliano                                  | `true` Se o participante estiver no lobby.                          |
| IsMuted              | Booliano                                  | `true` Se o participante estiver com mudo ativado (cliente ou servidor sem som).    |
| mediaStreams         | coleção [mediaStream](mediastream.md) | A lista de fluxos de mídia.                                   |
| recordingInfo        | [recordingInfo](recordinginfo.md)        | Informação que especifica se o participante tem capacidade de gravação. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.participant"
}-->
```json
{
  "id": "String (identifier)",
  "info": {"@odata.type": "#microsoft.graph.participantInfo"},
  "isInLobby": true,
  "isMuted": true,
  "mediaStreams": [ { "@odata.type": "#microsoft.graph.mediaStream" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

