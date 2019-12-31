---
title: tipo de recurso onlineMeeting
description: Contém informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 5d86df3bde56e242559e224cc27921d162be7bf4
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913412"
---
# <a name="onlinemeeting-resource-type"></a>tipo de recurso onlineMeeting

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre a reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.

## <a name="methods"></a>Methods

| Método         | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
| [Criar ReuniãoOnline](../api/application-post-onlineMeetings.md) | [onlineMeeting](onlinemeeting.md) | Criar uma reunião online. |
| [Obter onlineMeeting](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | Leia as propriedades e os relacionamentos de um objeto **onlineMeeting** . |

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo                                                   | Descrição                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| autoAdmittedUsers         | String                                                 | A configuração que especifica o tipo de participantes que será automaticamente permitido na reunião online. Os valores possíveis são: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`. Somente leitura.|
| audioConferencing         | [audioConferencing](audioconferencing.md)              | As informações de acesso de telefone (discagem) para uma reunião online. Somente leitura. |
| chatInfo                  | [chatInfo](chatinfo.md)                                | As informações de chat associadas a esta reunião online. |
| creationDatetime          | DateTime                                               | O horário de criação da reunião em UTC. Somente leitura. |
| startDateTime             | DateTime                                               | A hora de início da reunião em UTC. |
| endDateTime               | DateTime                                               | A hora de término da reunião em UTC. |
| id                        | String                                                 | A ID padrão associada à reunião online. Somente leitura. |
| joinWebUrl                   | String                                                 | A URL de ingresso da reunião online. Somente leitura.|
| participants              | [meetingParticipants](meetingparticipants.md)          | Os participantes associados à reunião online.  Isso inclui o organizador e os participantes. |
| assunto                   | Cadeia de caracteres                                                 | O assunto da reunião online. |
| capabilities              | Coleção de cadeias de caracteres                                      | A lista de recursos de reunião. Os valores possíveis são `questionAndAnswer`:. |
| videoTeleconferenceId     | String                                                 | A ID de teleconferência de vídeo. Somente leitura. |

### <a name="autoadmittedusers-values"></a>valores de autoAdmittedUsers
| Valor | Descrição  |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| organizer | Somente o organizador da reunião é admitido diretamente.  Todos os outros esperam no lobby, até que seja admitido pelo organizador  |
| invitedUsersInCompany | O organizador da reunião e os usuários na mesma empresa convidados pelo Organizador participam diretamente da reunião.  Todos os outros esperam no lobby até que seja admitido.  |
| everyoneInCompany | Todos na mesma empresa que o Organizador participam diretamente da reunião.  Usuários federados e anônimos esperam no lobby até serem admitidos.  |
| everyoneInSameAndFederatedCompany |  Todos na mesma empresa que o organizador e as empresas federadas ingressam na reunião diretamente.  Usuários anônimos esperam no lobby até serem admitidos.  |
| têm | Qualquer usuário é permitido, o que significa que todos (incluindo usuários anônimos) podem participar da reunião diretamente, sem esperar no lobby.  |


## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "autoAdmittedUsers": "everyone | everyoneInSameAndFederatedCompany | everyoneInCompany | invitedUsersInCompany | organizer",
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "capabilities": [ "questionAndAnswer" ],
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
