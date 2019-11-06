---
title: tipo de recurso onlineMeeting
description: Contém informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: VinodRavichandran
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 64b2c1880edafe1241367ac91889440a513964d9
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006610"
---
# <a name="onlinemeeting-resource-type"></a>tipo de recurso onlineMeeting

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre a reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.

## <a name="methods"></a>Métodos

| Método         | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
| [Criar onlineMeeting](../api/application-post-onlineMeetings.md) | [onlineMeeting](onlinemeeting.md) | Criar uma reunião online. |
| [Obter onlineMeeting](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | Leia as propriedades e os relacionamentos de um objeto **onlineMeeting** . |

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo                                                   | Descrição                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| autoAdmittedUsers         | String                                                 | A configuração que especifica o tipo de participantes que será automaticamente permitido na reunião online. Somente leitura. Os valores possíveis são `everyone`: `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`,,`organizer`|
| audioConferencing         | [audioConferencing](audioconferencing.md)              | As informações de acesso de telefone (discagem) para uma reunião online. Somente leitura. |
| canceledDateTime          | DateTime                                               | A hora em UTC quando a reunião foi cancelada. Somente leitura. |
| chatInfo                  | [chatInfo](chatinfo.md)                                | As informações de chat associadas a esta reunião online. |
| creationDatetime          | DateTime                                               | O horário de criação da reunião em UTC. Somente leitura. |
| startDateTime             | DateTime                                               | A hora de início da reunião em UTC. |
| endDateTime               | DateTime                                               | A hora de término da reunião em UTC. |
| id                        | String                                                 | A ID padrão associada à reunião online. Somente leitura. |
| IsCanceled                | Booliano                                                | Indica se a reunião foi cancelada. Somente leitura. |
| joinUrl                   | String                                                 | A URL de ingresso da reunião online. Somente leitura.|
| isbroadcast               | Booliano                                                | Indica se a reunião é uma reunião de transmissão. |
| participants              | [meetingParticipants](meetingparticipants.md)          | Os participantes associados à reunião online.  Isso inclui o organizador e os participantes. |
| assunto                   | Cadeia de caracteres                                                 | O assunto da reunião online. |
| capabilities              | String collection                                      | A lista de recursos de reunião. Os valores possíveis são `questionAndAnswer`:. |
| videoTeleconferenceId     | String                                                 | A ID de teleconferência do videio. Somente leitura. |

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
  "canceledDateTime": "String (timestamp)",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "isCanceled": false,
  "joinUrl": "String",
  "isBroadcast": false,
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
