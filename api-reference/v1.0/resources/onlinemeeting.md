---
title: Tipo de recurso onlineMeeting
description: Contém informações sobre uma reunião.
author: mkhribech
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 31d0d6262c9f0784b2a609b29221a51f6e871c96
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2022
ms.locfileid: "65883814"
---
# <a name="onlinemeeting-resource-type"></a>Tipo de recurso onlineMeeting

Namespace: microsoft.graph

Contém informações sobre uma reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.

## <a name="methods"></a>Métodos

| Método                                                             | Tipo de retorno                       | Descrição                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [Criar ReuniãoOnline](../api/application-post-onlineMeetings.md)  | [onlineMeeting](onlinemeeting.md) | Criar uma reunião online.                                                                                    |
| [Obter onlineMeeting](../api/onlinemeeting-get.md)                   | [onlineMeeting](onlinemeeting.md) | Leia as propriedades e as relações de um **objeto onlineMeeting** .                                        |
| [Atualizar](../api/onlinemeeting-update.md)                           | [onlineMeeting](onlinemeeting.md) | Atualize as propriedades de um **objeto onlineMeeting** . |
| [Excluir onlineMeeting](../api/onlinemeeting-delete.md)             | Nenhum                              | **Exclua um objeto onlineMeeting**.                                                                                    |
| [Criar ou obter onlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Crie um **objeto onlineMeeting** com uma ID externa personalizada. Se a reunião já existir, recupere suas propriedades. |

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                                          | Descrição                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| allowedPresenters     | [onlineMeetingPresenters](#onlinemeetingpresenters-values)                       | Especifica quem pode ser um apresentador em uma reunião. Os valores possíveis são listados na tabela a seguir.                          |
| allowAttendeeToEnableCamera     | Booliano                       | Indica se os participantes podem ligar a câmera.                          |
| allowAttendeeToEnableMic     | Booliano                       | Indica se os participantes podem ativar o microfone.                          |
| allowMeetingChat      | [meetingChatMode](#meetingchatmode-values) | Especifica o modo de chat de reunião. |
| allowTeamworkReactions | Booliano | Indica se as reações do Teams estão habilitadas para a reunião. |
| attendeeReport | Stream | O fluxo de conteúdo do relatório de participantes de um [evento ao vivo do Microsoft Teams](/microsoftteams/teams-live-events/what-are-teams-live-events). Somente leitura. |
| audioConferencing     | [audioConferencing](audioconferencing.md)     | As informações de acesso por telefone (discagem) para uma reunião online. Somente leitura.                                                   |
| broadcastSettings              | [broadcastMeetingSettings](broadcastMeetingSettings.md)                      | Configurações relacionadas a um evento ao vivo.                                                                  |
| chatInfo              | [chatInfo](chatinfo.md)                       | As informações de chat associadas a esta reunião online.                                                                  |
| creationDateTime      | DateTime                                      | A hora de criação da reunião em UTC. Somente leitura.                                                                               |
| endDateTime           | DateTime                                      | A hora de término da reunião em UTC.                                                                                               |
| id                    | String                                        | A ID padrão associada à reunião online. Somente leitura.                                                              |
| isBroadcast  | Booliano                                       | Indica se este é um evento ao vivo [do Teams](/microsoftteams/teams-live-events/what-are-teams-live-events).                  |
| isEntryExitAnentry  | Booliano                                       | Indica se os chamadores devem anunciar quando ingressar ou sair.                                                                     |
| joinInformation       | [itemBody](itembody.md)                       | As informações de junção no idioma e na variante de localidade especificadas no cabeçalho `Accept-Language` HTTP da solicitação. Somente leitura. |
| joinWebUrl            | String                                        | A URL de ingresso da reunião online. Somente leitura.                                                                             |
| lobbyBypassSettings   | [lobbyBypassSettings](lobbyBypassSettings.md) | Especifica quais participantes podem ignorar o lobby da reunião.                                                               |
| participants          | [meetingParticipants](meetingparticipants.md) | Os participantes associados à reunião online.  Isso inclui o organizador e os participantes.                       |
| recordAutomatically | Booliano | Indica se a reunião deve ser gravada automaticamente. |
| startDateTime         | DateTime                                      | A hora de início da reunião em UTC.                                                                                             |
| assunto               | String                                        | O assunto da reunião online.                                                                                         |
| videoTeleconferenceId | String                                        | A ID de teleconferência de vídeo. Somente leitura.                                                                                  |

### <a name="onlinemeetingpresenters-values"></a>Valores onlineMeetingPresenters

| Valor              | Descrição                                                   |
| ------------------ | ------------------------------------------------------------- |
| Todos           | Todos são apresentadores (essa é a opção padrão).             |
| organization       | Todos na organização do organizador são apresentadores.          |
| roleIsPresenter    | Somente os participantes cuja função é apresentador são apresentadores. |
| organizer          | Somente o organizador é um apresentador.                           |
| unknownFutureValue | Valor futuro desconhecido.                                          |

> [!TIP]
>
> Ao criar ou atualizar uma reunião online com **allowedPresenters** `roleIsPresenter`definido como , inclua uma lista completa de participantes  com a  `presenter` função de participantes especificada definida como no corpo da solicitação.

### <a name="meetingchatmode-values"></a>valores meetingChatMode

| Valor              | Descrição                                                            |
| ------------------ | ---------------------------------------------------------------------- |
| enabled            | O chat de reunião está habilitado.                                               |
| desabilitadas           | O chat de reunião está desabilitado.                                              |
| Limitado            | O chat de reunião está habilitado, mas somente durante a chamada de reunião. |
| unknownFutureValue | Valor futuro desconhecido.                                                  |

## <a name="relationships"></a>Relações

| Relação | Tipo | Descrição |
| ------------ | ---- | ----------- |
| attendanceReports | [coleção meetingAttendanceReport](meetingAttendanceReport.md) | Os relatórios de participação de uma reunião online. Somente leitura. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "audioConferencing": {"@odata.type": "microsoft.graph.audioConferencing"},
  "chatInfo": {"@odata.type": "microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "joinWebUrl": "String",
  "participants": {"@odata.type": "microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String",
  "videoTeleconferenceId": "String",
  "isEntryExitAnnounced": "Boolean",
  "lobbyBypassSettings": {"@odata.type": "microsoft.graph.lobbyBypassSettings"},
  "allowedPresenters": "String",
  "isBroadcast": "Boolean",
  "broadcastSettings": {"@odata.type": "microsoft.graph.broadcastSettings"},
  "allowMeetingChat": {"@odata.type": "microsoft.graph.meetingChatMode"},
  "allowTeamworkReactions": "Boolean",
  "allowAttendeeToEnableMic": "Boolean",
  "allowAttendeeToEnableCamera": "Boolean"
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

