---
title: Tipo de recurso onlineMeeting
description: Contém informações sobre uma reunião.
author: mkhribech
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 5f84034463044d3f8c832f1a8b0e0c17656c0f3a
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979429"
---
# <a name="onlinemeeting-resource-type"></a>Tipo de recurso onlineMeeting

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre uma reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.

## <a name="methods"></a>Métodos

| Método                                                             | Tipo de retorno                       | Descrição                                                                                                       |
| :----------------------------------------------------------------- | :-------------------------------- | :---------------------------------------------------------------------------------------------------------------- |
| [Criar](../api/application-post-onlineMeetings.md)                | [onlineMeeting](onlinemeeting.md) | Criar uma reunião online.                                                                                         |
| [Obter](../api/onlinemeeting-get.md)                                 | [onlineMeeting](onlinemeeting.md) | Leia as propriedades e as relações de um **objeto onlineMeeting.**                                             |
| [Atualizar](../api/onlinemeeting-update.md)                           | [onlineMeeting](onlinemeeting.md) | Atualize as propriedades de um **objeto onlineMeeting.** |
| [Delete](../api/onlinemeeting-delete.md)                           | Nenhum                              | Excluir um **objeto onlineMeeting.**                                                                             |
| [Criar ou obter OnlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Crie uma reunião online com uma ID externa personalizada. Se a reunião já existir, recupere suas propriedades.      |

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                                          | Descrição                                                                                                                                                                                                                                                 |
| :-------------------- | :-------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| allowedPresenters     | [onlineMeetingPresenters](#onlinemeetingpresenters-values)| Especifica quem pode ser um apresentador em uma reunião. Os valores possíveis `everyone` são , , e `organization` `roleIsPresenter` `organizer` `unknownFutureValue` .                                                                                                    |
| allowAttendeeToEnableCamera | Boleano | Indica se os participantes podem ativar a câmera. |
| allowAttendeeToEnableMic | Boleano | Indica se os participantes podem ativar o microfone. |
| allowMeetingChat      | [meetingChatMode](#meetingchatmode-values) | Especifica o modo de chat de reunião. |
| allowTeamworkReactions | Boleano | Indica se Teams reações estão habilitadas para a reunião. |
| alternativeRecording  | Stream                                        | O fluxo de conteúdo da gravação alternativa de um evento ao vivo. Somente leitura.                                                                                                                                                                                 |
| attendeeReport        | Stream                                        | O fluxo de conteúdo do relatório do participante de um evento ao vivo. Somente leitura.                                                                                                                                                                                       |
| audioConferencing     | [audioConferencing](audioconferencing.md)     | As informações de acesso por telefone (discagem) para uma reunião online. Somente leitura.                                                                                                                                                                                    |
| broadcastSettings     | [broadcastMeetingSettings](broadcastMeetingSettings.md)     | Configurações relacionado a um evento ao vivo.                                                                                                                                                                                                                     |
| chatInfo              | [chatInfo](chatinfo.md)                       | As informações de chat associadas a essa reunião online.                                                                                                                                                                                                   |
| creationDateTime      | DateTime                                      | O tempo de criação da reunião em UTC. Somente leitura.                                                                                                                                                                                                                |
| endDateTime           | DateTime                                      | A hora de término da reunião em UTC.                                                                                                                                                                                                                                |
| externalId            | Cadeia de caracteres                                        | A ID externa. Uma ID personalizada. Opcional.                                                                                                                                                                                                                     |
| id                    | String                                        | A ID padrão associada à reunião online. Somente leitura.                                                                                                                                                                                               |
| isBroadcast           | Boleano                                       | Indica se é um evento ao vivo.                                                                                                                                                                                                                   |
| isEntryExitAnnounced  | Boleano                                       | Indica se os chamadores ingressarão ou sairão.                                                                                                                                                                                                      |
| joinWebUrl            | Cadeia de Caracteres                                        | A URL de junção da reunião online. Somente leitura.                                                                                                                                                                                                              |
| joinInformation       | [itemBody](itembody.md)                       | As informações de junção no idioma e na variante de localidade especificadas no cabeçalho HTTP de solicitação "Accept-Language". Somente leitura                                                                                                                                       |
| lobbyBypassSettings   | [lobbyBypassSettings](lobbyBypassSettings.md) | Especifica quais participantes podem ignorar o lobby da reunião.                                                                                                                                                                                                  |
| meetingAttendanceReport | [meetingAttendanceReport](meetingAttendanceReport.md) | O relatório de participação de uma reunião agendada. Somente leitura. |
| participants          | [meetingParticipants](meetingparticipants.md) | Os participantes associados à reunião online. Isso inclui o organizador e os participantes.                                                                                                                                                        |
| recordAutomatically | Booliano | Indica se deve gravar a reunião automaticamente. |
| recording             | Stream                                        | O fluxo de conteúdo da gravação de um evento ao vivo. Somente leitura.                                                                                                                                                                                             |
| startDateTime         | DateTime                                      | O horário de início da reunião em UTC.                                                                                                                                                                                                                              |
| assunto               | Cadeia de caracteres                                        | O assunto da reunião online.                                                                                                                                                                                                                          |
| videoTeleconferenceId | Cadeia de caracteres                                        | A ID de teleconferência de vídeo. Somente leitura.                                                                                                                                                                                                                   |
| autoAdmittedUsers (preterido)    | Cadeia de Caracteres                                        | A configuração que especifica o tipo de participantes que serão automaticamente permitidos na reunião online. Os valores possíveis são: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`. Somente leitura. |
| capabilities (preterido)         | coleção meetingCapabilities                             | A lista de recursos de reunião. Os valores possíveis são: `questionAndAnswer` , `unknownFutureValue` .                                                                                                                                                                                 |

> [!CAUTION]
>
>- A **propriedade autoAdmittedUsers** é preterida. Use a **propriedade scope** do [lobbyBypassSettings.](lobbyBypassSettings.md)
>- A **propriedade capabilities** é preterida. Use a **propriedade isQuestionAndAnswerEnabled** [de broadcastMeetingSettings.](broadcastMeetingSettings.md)

### <a name="onlinemeetingpresenters-values"></a>valores onlineMeetingPresenters

| Valor              | Descrição                                                   |
| ------------------ | ------------------------------------------------------------- |
| everyone           | Todos são apresentadores (essa é a opção padrão).             |
| organização       | Todos na organização do organizador são apresentadores.          |
| roleIsPresenter    | Somente os participantes cuja função é apresentador são apresentadores. |
| organizer          | Somente o organizador é um apresentador.                           |
| unknownFutureValue | Valor futuro desconhecido.                                         |

> [!TIP]
>
>- Ao criar ou atualizar uma reunião online com o valor **de allowedPresenters** definido como , inclua uma lista completa de participantes com a função de participantes especificada definida como no corpo `roleIsPresenter` da   `presenter` solicitação.
>- Ao criar ou atualizar uma reunião online com o valor **de allowedPresenters** definido como outros valores que não a função dos participantes será mostrar como no corpo `roleIsPresenter` da  `null` resposta.

### <a name="meetingchatmode-values"></a>valores meetingChatMode

| Valor              | Descrição                                                            |
| ------------------ | ---------------------------------------------------------------------- |
| enabled            | O chat de reunião está habilitado.                                               |
| desabilitadas           | O chat de reunião está desabilitado.                                              |
| limited            | O chat de reunião está habilitado, mas somente durante a chamada de reunião. |
| unknownFutureValue | Valor futuro desconhecido.                                                  |

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
