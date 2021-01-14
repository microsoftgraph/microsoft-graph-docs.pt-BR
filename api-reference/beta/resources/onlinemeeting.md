---
title: Tipo de recurso onlineMeeting
description: Contém informações sobre uma reunião.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: fedfb6a7558e081bb333c1fc6f579f2600137e9c
ms.sourcegitcommit: dbbf77c732ae8d982e59865432b9b6147002a30a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/14/2021
ms.locfileid: "49866225"
---
# <a name="onlinemeeting-resource-type"></a>Tipo de recurso onlineMeeting

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre uma reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.

## <a name="methods"></a>Methods

| Método                                                             | Tipo de retorno                       | Descrição                                                                                                       |
| :----------------------------------------------------------------- | :-------------------------------- | :---------------------------------------------------------------------------------------------------------------- |
| [Criar](../api/application-post-onlineMeetings.md)                | [onlineMeeting](onlinemeeting.md) | Criar uma reunião online.                                                                                         |
| [Get](../api/onlinemeeting-get.md)                                 | [onlineMeeting](onlinemeeting.md) | Leia as propriedades e os relacionamentos de um **objeto onlineMeeting.**                                             |
| [Criar ou obter onlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Crie uma reunião online com uma ID externa personalizada. Se a reunião já existir, recupere suas propriedades.      |
| [Update](../api/onlinemeeting-update.md)                           | [onlineMeeting](onlinemeeting.md) | Atualize **as propriedades startDateTime**, **endDateTime**, **assunto** e **participantes** de uma reunião online. |
| [Delete](../api/onlinemeeting-delete.md)                           | Nenhum                              | **Exclua um recurso onlineMeeting.**                                                                             |

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                                          | Descrição                                                                                                                                                                                                                                                 |
| :-------------------- | :-------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| autoAdmittedUsers     | Cadeia de caracteres                                        | A configuração que especifica o tipo de participantes que serão automaticamente permitidos na reunião online. Os valores possíveis são: `everyone`, `everyoneInSameAndFederatedCompany`, `everyoneInCompany`, `invitedUsersInCompany`, `organizer`. Somente leitura. |
| audioConferencing     | [audioConferencing](audioconferencing.md)     | As informações de acesso telefônico (discagem) de uma reunião online. Apenas leitura.                                                                                                                                                                                    |
| chatInfo              | [chatInfo](chatinfo.md)                       | As informações de chat associadas a esta reunião online.                                                                                                                                                                                                   |
| creationDateTime      | DateTime                                      | A hora de criação da reunião em UTC. Somente leitura.                                                                                                                                                                                                                |
| startDateTime         | DateTime                                      | A hora de início da reunião em UTC.                                                                                                                                                                                                                              |
| endDateTime           | DateTime                                      | A hora de término da reunião em UTC.                                                                                                                                                                                                                                |
| id                    | Cadeia de caracteres                                        | A ID padrão associada à reunião online. Somente leitura.                                                                                                                                                                                               |
| joinWebUrl            | Cadeia de caracteres                                        | A URL de junção da reunião online. Somente leitura.                                                                                                                                                                                                              |
| participants          | [meetingParticipants](meetingparticipants.md) | Os participantes associados à reunião online.  Isso inclui o organizador e os participantes.                                                                                                                                                        |
| assunto               | Cadeia de caracteres                                        | O assunto da reunião online.                                                                                                                                                                                                                          |
| capabilities          | Conjunto de cadeias de caracteres                             | A lista de recursos de reunião. Os valores possíveis são: `questionAndAnswer` .                                                                                                                                                                                 |
| videoTeleconferenceId | Cadeia de caracteres                                        | A ID de teleconferência de vídeo. Somente leitura.                                                                                                                                                                                                                   |
| joinInformation       | [itemBody](itembody.md)                       | As informações de junção na variante de idioma e localidade especificadas no cabeçalho HTTP de solicitação "Accept-Language". Somente leitura                                                                                                                                       |
| externalId            | Cadeia de caracteres                                        | A ID externa. Uma ID personalizada. Opcional.                                                                                                                                                                                                                     |
| isEntryExitAnentry  | Boolean                                       | Se será ou não anunciar quando os chamadores ingressarem ou saírem.                                                                                                                                                                                                      |
| lobbyBypassSettings   | [lobbyBypassSettings](lobbyBypassSettings.md) | Especifica quais participantes podem ignorar o lobby da reunião.                                                                                                                                                                                                  |
| allowedPresenters     | onlineMeetingPresenters                       | Especifica quem pode ser um apresentador em uma reunião. Os valores possíveis `everyone` são , , e `organization` `roleIsPresenter` `organizer` `unknownFutureValue` .                                                                                                    |
| isBroadcast           | Boolean                                       | Indica se este é um evento ao vivo.                                                                                                                                                                                                                   |
| broadcastSettings     | [broadcastMeetingSettings](broadcastMeetingSettings.md)     | Configurações relacionadas a um evento ao vivo*                                                                                                                                                                                                                    |
| attendeeReport        | Fluxo                                        | O fluxo de conteúdo do relatório de participantes de um evento ao vivo. Somente leitura.                                                                                                                                                                                       |
| gravação             | Fluxo                                        | O fluxo de conteúdo da gravação de um evento ao vivo. Somente leitura.                                                                                                                                                                                             |
| alternativeRecording  | Fluxo                                        | O fluxo de conteúdo da gravação alternativa de um evento ao vivo. Somente leitura.                                                                                                                                                                                 |

> [!IMPORTANT]
> A **propriedade autoAdmittedUsers** está obsoleta. Use **lobbyBypassSettings.scope em vez** de configurações de opção de reunião.
> 
> *\Criar eventos ao vivo com a **propriedade broadcastSettings** está em Beta, com limitações importantes. Consulte [broadcastSettings](broadcastMeetingSettings.md) para obter mais detalhes.

### <a name="onlinemeetingpresenters-values"></a>Valores de onlineMeetingPresenters

| Valor              | Descrição                                                   |
| ------------------ | ------------------------------------------------------------- |
| everyone           | Todos são apresentadores (essa é a opção padrão).             |
| organization       | Todos na organização do organizador são apresentadores.          |
| roleIsPresenter    | Somente os participantes cuja função é apresentador são apresentadores. |
| organizer          | Somente o organizador é um apresentador.                           |
| unknownFutureValue | Valor futuro desconhecido.                                         |

**Observação:** se o valor de **allowedPresenters** for definido como , especifique a função de reunião de cada participante da reunião usando a propriedade de função em `roleIsPresenter`  [meetingParticipantInfo](../resources/meetingparticipantinfo.md).

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
  "videoTeleconferenceId": "String",
  "isEntryExitAnnounced": "Boolean",
  "lobbyBypassSettings": {"@odata.type": "#microsoft.graph.lobbyBypassSettings"},
  "allowedPresenters": "String",
  "isBroadcast": "Boolean",
  "broadcastSettings": {"@odata.type": "#microsoft.graph.broadcastSettings"}
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


