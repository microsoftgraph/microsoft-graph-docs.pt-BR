---
title: tipo de recurso participant
description: Representa o tipo de participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 99f165f2f3e99ab424a318b053a060ccda8fdc1c
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49943714"
---
# <a name="participant-resource-type"></a>tipo de recurso participant

Namespace: microsoft.graph

Representa um participante em uma chamada.

## <a name="methods"></a>Métodos

| Método                                                 | Tipo de retorno                                                 | Descrição                                    |
|:-------------------------------------------------------|:------------------------------------------------------------|:-----------------------------------------------|
| [Listar participantes](../api/participant-get.md)          | [participante](participant.md)                               | Recupere uma lista de **objetos** de participante na chamada. |
| [Obter participante](../api/participant-get.md)           | [participante](participant.md)                               | Leia as propriedades do **objeto participante.** |
| [Excluir participante](../api/participant-delete.md)         | Nenhum   | Exclua um participante de uma chamada.                  |
| [Convidar](../api/participant-invite.md)                 | [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md)                        | Convide um participante para a chamada.              |
| [Ativar mudo para participante](../api/participant-mute.md)         | [muteParticipantOperation](muteparticipantoperation.md)     | Silenciar um participante em uma chamada.                  |

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo                                     | Descrição                                                  |
| :------------------- | :--------------------------------------- | :------------------------------------------------------------|
| id                   | String                                   | A ID do participante.                                          |
| informações                  | [participantInfo](participantinfo.md)    | Informações sobre o participante.                          |
| isInLobby            | Booliano                                  | `true` se o participante estiver no lobby.                          |
| isMuted              | Booliano                                  | `true` se o participante estiver sem som (cliente ou servidor mudo).    |
| mediaStreams         | [Coleção mediaStream](mediastream.md) | A lista de fluxos de mídia.                                   |
| recordingInfo        | [recordingInfo](recordinginfo.md)        | Informações sobre se o participante tem capacidade de gravação. |

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

