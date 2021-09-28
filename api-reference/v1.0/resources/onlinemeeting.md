---
title: Tipo de recurso onlineMeeting
description: Contém informações sobre uma reunião.
author: mkhribech
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: e07042b485276ab8d8e712d9bf64e32a5771f5c7
ms.sourcegitcommit: 84d9a50dfa9526a207696c69d92381c8763d986a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2021
ms.locfileid: "59979352"
---
# <a name="onlinemeeting-resource-type"></a>Tipo de recurso onlineMeeting

Namespace: microsoft.graph

Contém informações sobre uma reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.

## <a name="methods"></a>Métodos

| Método                                                             | Tipo de retorno                       | Descrição                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [Criar ReuniãoOnline](../api/application-post-onlineMeetings.md)  | [onlineMeeting](onlinemeeting.md) | Criar uma reunião online.                                                                                    |
| [Obter onlineMeeting](../api/onlinemeeting-get.md)                   | [onlineMeeting](onlinemeeting.md) | Leia as propriedades e as relações de um **objeto onlineMeeting.**                                        |
| [Atualizar](../api/onlinemeeting-update.md)                           | [onlineMeeting](onlinemeeting.md) | Atualize as propriedades de um **objeto onlineMeeting.** |
| [Excluir onlineMeeting](../api/onlinemeeting-delete.md)             | Nenhum                              | Excluir um **objeto onlineMeeting.**                                                                                    |
| [Criar ou obter OnlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Crie um **objeto onlineMeeting** com uma ID externa personalizada. Se a reunião já existir, recupere suas propriedades. |

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                                          | Descrição                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| allowedPresenters     | [onlineMeetingPresenters](#onlinemeetingpresenters-values)                       | Especifica quem pode ser um apresentador em uma reunião. Os valores possíveis são listados na tabela a seguir.                          |
| allowAttendeeToEnableCamera     | Boleano                       | Indica se os participantes podem ativar a câmera.                          |
| allowAttendeeToEnableMic     | Booliano                       | Indica se os participantes podem ativar o microfone.                          |
| allowMeetingChat      | [meetingChatMode](#meetingchatmode-values) | Especifica o modo de chat de reunião. |
| allowTeamworkReactions | Boleano | Indica se Teams reações estão habilitadas para a reunião. |
| audioConferencing     | [audioConferencing](audioconferencing.md)     | As informações de acesso por telefone (discagem) para uma reunião online. Somente leitura.                                                   |
| broadcastSettings              | [broadcastMeetingSettings](broadcastMeetingSettings.md)                      | Configurações relacionado a um evento ao vivo.                                                                  |
| chatInfo              | [chatInfo](chatinfo.md)                       | As informações de chat associadas a essa reunião online.                                                                  |
| creationDateTime      | DateTime                                      | O tempo de criação da reunião em UTC. Somente leitura.                                                                               |
| endDateTime           | DateTime                                      | A hora de término da reunião em UTC.                                                                                               |
| id                    | Cadeia de caracteres                                        | A ID padrão associada à reunião online. Somente leitura.                                                              |
| isBroadcast  | Boleano                                       | Indica se esse é um evento ao vivo.                  |
| isEntryExitAnnounced  | Booliano                                       | Indica se os chamadores ingressarão ou sairão.                                                                     |
| joinInformation       | [itemBody](itembody.md)                       | As informações de junção no idioma e na variante de localidade especificadas no `Accept-Language` cabeçalho HTTP da solicitação. Somente leitura. |
| joinWebUrl            | Cadeia de Caracteres                                        | A URL de junção da reunião online. Somente leitura.                                                                             |
| lobbyBypassSettings   | [lobbyBypassSettings](lobbyBypassSettings.md) | Especifica quais participantes podem ignorar o lobby da reunião.                                                               |
| participants          | [meetingParticipants](meetingparticipants.md) | Os participantes associados à reunião online.  Isso inclui o organizador e os participantes.                       |
| startDateTime         | DateTime                                      | O horário de início da reunião em UTC.                                                                                             |
| assunto               | Cadeia de caracteres                                        | O assunto da reunião online.                                                                                         |
| videoTeleconferenceId | Cadeia de Caracteres                                        | A ID de teleconferência de vídeo. Somente leitura.                                                                                  |

### <a name="onlinemeetingpresenters-values"></a>valores onlineMeetingPresenters

| Valor              | Descrição                                                   |
| ------------------ | ------------------------------------------------------------- |
| everyone           | Todos são apresentadores (essa é a opção padrão).             |
| organização       | Todos na organização do organizador são apresentadores.          |
| roleIsPresenter    | Somente os participantes cuja função é apresentador são apresentadores. |
| organizer          | Somente o organizador é um apresentador.                           |
| unknownFutureValue | Valor futuro desconhecido.                                          |

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

