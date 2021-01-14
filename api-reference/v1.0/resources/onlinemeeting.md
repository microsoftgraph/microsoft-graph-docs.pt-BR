---
title: Tipo de recurso onlineMeeting
description: Contém informações sobre uma reunião.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 139cd4a20a6097691189d1bd1f843850ba911a21
ms.sourcegitcommit: dbbf77c732ae8d982e59865432b9b6147002a30a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/14/2021
ms.locfileid: "49866106"
---
# <a name="onlinemeeting-resource-type"></a>Tipo de recurso onlineMeeting

Namespace: microsoft.graph

Contém informações sobre uma reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.

## <a name="methods"></a>Methods

| Método                                                             | Tipo de retorno                       | Descrição                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [Criar ReuniãoOnline](../api/application-post-onlineMeetings.md)  | [onlineMeeting](onlinemeeting.md) | Criar uma reunião online.                                                                                    |
| [Obter onlineMeeting](../api/onlinemeeting-get.md)                   | [onlineMeeting](onlinemeeting.md) | Leia as propriedades e os relacionamentos de um **objeto onlineMeeting.**                                        |
| [Excluir onlineMeeting](../api/onlinemeeting-delete.md)             | Nenhum                              | Excluir uma reunião online.                                                                                    |
| [Criar ou obter onlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Crie uma reunião online com uma ID externa personalizada. Se a reunião já existir, recupere suas propriedades. |

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                                          | Descrição                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| audioConferencing     | [audioConferencing](audioconferencing.md)     | As informações de acesso telefônico (discagem) de uma reunião online. Apenas leitura.                                                   |
| chatInfo              | [chatInfo](chatinfo.md)                       | As informações de chat associadas a esta reunião online.                                                                  |
| creationDateTime      | DateTime                                      | A hora de criação da reunião em UTC. Somente leitura.                                                                               |
| startDateTime         | DateTime                                      | A hora de início da reunião em UTC.                                                                                             |
| endDateTime           | DateTime                                      | A hora de término da reunião em UTC.                                                                                               |
| id                    | Cadeia de caracteres                                        | A ID padrão associada à reunião online. Somente leitura.                                                              |
| joinWebUrl            | Cadeia de caracteres                                        | A URL de junção da reunião online. Somente leitura.                                                                             |
| participants          | [meetingParticipants](meetingparticipants.md) | Os participantes associados à reunião online.  Isso inclui o organizador e os participantes.                       |
| assunto               | Cadeia de caracteres                                        | O assunto da reunião online.                                                                                         |
| videoTeleconferenceId | Cadeia de caracteres                                        | A ID de teleconferência de vídeo. Somente leitura.                                                                                  |
| joinInformation       | [itemBody](itembody.md)                       | As informações de junção na variante de idioma e localidade especificadas no cabeçalho `Accept-Language` HTTP da solicitação. Somente leitura. |
| isEntryExitAnentry  | Boolean                                       | Se será ou não anunciar quando os chamadores ingressarem ou saírem.                                                                     |
| lobbyBypassSettings   | [lobbyBypassSettings](lobbyBypassSettings.md) | Especifica quais participantes podem ignorar o lobby da reunião.                                                               |
| allowedPresenters     | onlineMeetingPresenters                       | Especifica quem pode ser um apresentador em uma reunião. Os valores possíveis estão listados na tabela a seguir.                          |

### <a name="onlinemeetingpresenters-values"></a>Valores de onlineMeetingPresenters

| Valor              | Descrição                                                   |
| ------------------ | ------------------------------------------------------------- |
| everyone           | Todos são apresentadores (essa é a opção padrão).             |
| organization       | Todos na organização do organizador são apresentadores.          |
| roleIsPresenter    | Somente os participantes cuja função é apresentador são apresentadores. |
| organizer          | Somente o organizador é um apresentador.                           |
| unknownFutureValue | Valor futuro desconhecido.                                          |

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
  "videoTeleconferenceId": "String",
  "isEntryExitAnnounced": "Boolean",
  "lobbyBypassSettings": {"@odata.type": "#microsoft.graph.lobbyBypassSettings"},
  "allowedPresenters": "String"
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

