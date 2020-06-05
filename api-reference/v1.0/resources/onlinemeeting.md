---
title: tipo de recurso onlineMeeting
description: Contém informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 812f094667b217d167509be324843227e552e0a5
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556223"
---
# <a name="onlinemeeting-resource-type"></a>tipo de recurso onlineMeeting

Namespace: microsoft.graph

Contém informações sobre a reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.

## <a name="methods"></a>Methods

| Método         | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
| [Criar ReuniãoOnline](../api/application-post-onlineMeetings.md) | [onlineMeeting](onlinemeeting.md) | Criar uma reunião online. |
| [Obter onlineMeeting](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | Leia as propriedades e os relacionamentos de um objeto **onlineMeeting** . |
| [Excluir onlineMeeting](../api/onlinemeeting-delete.md) | Nenhuma | Excluir uma reunião online. |
| [Criar ou obter onlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Criar uma reunião online com uma ID externa personalizada. Se a reunião já existir, recupere suas propriedades. |

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo                                                   | Descrição                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| audioConferencing         | [audioConferencing](audioconferencing.md)              | As informações de acesso de telefone (discagem) para uma reunião online. Apenas leitura. |
| chatInfo                  | [chatInfo](chatinfo.md)                                | As informações de chat associadas a esta reunião online. |
| creationDatetime          | DateTime                                               | O horário de criação da reunião em UTC. Somente leitura. |
| startDateTime             | DateTime                                               | A hora de início da reunião em UTC. |
| endDateTime               | DateTime                                               | A hora de término da reunião em UTC. |
| id                        | String                                                 | A ID padrão associada à reunião online. Somente leitura. |
| joinWebUrl                | String                                                 | A URL de ingresso da reunião online. Somente leitura.|
| participants              | [meetingParticipants](meetingparticipants.md)          | Os participantes associados à reunião online.  Isso inclui o organizador e os participantes. |
| subject                   | Cadeia de caracteres                                                 | O assunto da reunião online. |
| videoTeleconferenceId     | String                                                 | A ID de teleconferência de vídeo. Somente leitura. |
| joinInformation | [itemBody](itembody.md) | As informações de ingresso no idioma e na variante de localidade especificados no `Accept-Language` cabeçalho HTTP da solicitação. Somente leitura. |

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
