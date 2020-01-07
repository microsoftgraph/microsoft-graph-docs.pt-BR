---
title: tipo de recurso onlineMeeting
description: Contém informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 7b82170b606334c6db8fa07c3f9b2f95f16c0082
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40951962"
---
# <a name="onlinemeeting-resource-type"></a>tipo de recurso onlineMeeting

Contém informações sobre a reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.

## <a name="methods"></a>Methods

| Método         | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
| [Criar ReuniãoOnline](../api/application-post-onlineMeetings.md) | [onlineMeeting](onlinemeeting.md) | Criar uma reunião online. |
| [Obter onlineMeeting](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | Leia as propriedades e os relacionamentos de um objeto **onlineMeeting** . |
| [Excluir onlineMeeting](../api/onlinemeeting-delete.md) | Nenhum | Excluir uma reunião online |

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo                                                   | Descrição                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| audioConferencing         | [audioConferencing](audioconferencing.md)              | As informações de acesso de telefone (discagem) para uma reunião online. Somente leitura. |
| chatInfo                  | [chatInfo](chatinfo.md)                                | As informações de chat associadas a esta reunião online. |
| creationDatetime          | DateTime                                               | O horário de criação da reunião em UTC. Somente leitura. |
| startDateTime             | DateTime                                               | A hora de início da reunião em UTC. |
| endDateTime               | DateTime                                               | A hora de término da reunião em UTC. |
| id                        | String                                                 | A ID padrão associada à reunião online. Somente leitura. |
| joinWebUrl                | String                                                 | A URL de ingresso da reunião online. Somente leitura.|
| participants              | [meetingParticipants](meetingparticipants.md)          | Os participantes associados à reunião online.  Isso inclui o organizador e os participantes. |
| assunto                   | Cadeia de caracteres                                                 | O assunto da reunião online. |
| videoTeleconferenceId     | String                                                 | A ID de teleconferência de vídeo. Somente leitura. |


## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "videoTeleconferenceId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
