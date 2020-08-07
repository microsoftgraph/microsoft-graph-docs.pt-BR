---
title: tipo de recurso onlineMeeting
description: Contém informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: bfc1055b3e700b951957ffd1bce0fe7a541846b0
ms.sourcegitcommit: 93b6781adf2c889235022d34ab50e2a4d62760c5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/07/2020
ms.locfileid: "46589248"
---
# <a name="onlinemeeting-resource-type"></a>tipo de recurso onlineMeeting

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre a reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.

## <a name="methods"></a>Métodos

| Método         | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
| [Criar](../api/application-post-onlineMeetings.md) | [onlineMeeting](onlinemeeting.md) | Criar uma reunião online. |
| [Get](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | Leia as propriedades e os relacionamentos de um objeto **onlineMeeting** . |
| [Criar ou obter onlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Criar uma reunião online com uma ID externa personalizada. Se a reunião já existir, recupere suas propriedades. |
| [Atualizar](../api/onlinemeeting-update.md) | [onlineMeeting](onlinemeeting.md) | Atualizar as propriedades **StartDateTime**, **EndDateTime**, **Subject**e **participantes** de uma reunião online. |
| [Excluir](../api/onlinemeeting-delete.md) | Nenhuma | Excluir um recurso **onlineMeeting** . |

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo                                                   | Descrição                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| autoAdmittedUsers         | String                                                 | A configuração que especifica o tipo de participantes que será automaticamente permitido na reunião online. Os valores possíveis são: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`. Somente leitura.|
| audioConferencing         | [audioConferencing](audioconferencing.md)              | As informações de acesso de telefone (discagem) para uma reunião online. Apenas leitura. |
| chatInfo                  | [chatInfo](chatinfo.md)                                | As informações de chat associadas a esta reunião online. |
| creationDatetime          | DateTime                                               | O horário de criação da reunião em UTC. Somente leitura. |
| startDateTime             | DateTime                                               | A hora de início da reunião em UTC. |
| endDateTime               | DateTime                                               | A hora de término da reunião em UTC. |
| id                        | String                                                 | A ID padrão associada à reunião online. Somente leitura. |
| joinWebUrl                   | String                                                 | A URL de ingresso da reunião online. Somente leitura.|
| participants              | [meetingParticipants](meetingparticipants.md)          | Os participantes associados à reunião online.  Isso inclui o organizador e os participantes. |
| assunto                   | String                                                 | O assunto da reunião online. |
| capabilities              | Coleção de cadeias de caracteres                                      | A lista de recursos de reunião. Os valores possíveis são: `questionAndAnswer` . |
| videoTeleconferenceId     | String                                                 | A ID de teleconferência de vídeo. Somente leitura. |
| joinInformation | [itemBody](itembody.md) | As informações de ingresso no idioma e na variante de localidade especificados no cabeçalho HTTP da solicitação ' Accept-Language '. Somente leitura |
| externalId                | Cadeia de caracteres                                                 | A ID externa. Uma ID personalizada. Opcional. |

### <a name="autoadmittedusers-values"></a>valores de autoAdmittedUsers
| Valor | Descrição  |
| :------------------------ | :----------------------------------------------------- |
| organizer | Somente o organizador da reunião é admitido diretamente.  Todos os outros esperam no lobby, até que seja admitido pelo organizador  |
| invitedUsersInCompany | O organizador da reunião e os usuários na mesma empresa convidados pelo Organizador participam diretamente da reunião.  Todos os outros esperam no lobby até que seja admitido.  |
| everyoneInCompany | Todos na mesma empresa que o Organizador participam diretamente da reunião.  Usuários federados e anônimos esperam no lobby até serem admitidos.  |
| everyoneInSameAndFederatedCompany |  Todos na mesma empresa que o organizador e as empresas federadas ingressam na reunião diretamente.  Usuários anônimos esperam no lobby até serem admitidos.  |
| têm | Qualquer usuário é permitido, o que significa que todos (incluindo usuários anônimos) podem participar da reunião diretamente, sem esperar no lobby.  |


## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "externalId"
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
