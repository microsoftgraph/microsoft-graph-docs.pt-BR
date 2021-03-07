---
title: Tipo de recurso onlineMeeting
description: Contém informações sobre uma reunião.
author: ananmishr
localization_priority: Normal
doc_type: resourcePageType
ms.prod: cloud-communications
ms.openlocfilehash: 8ded2e79f8a9a2004f2ffa412b6d42e3275556b8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516091"
---
# <a name="onlinemeeting-resource-type"></a>Tipo de recurso onlineMeeting

Namespace: microsoft.graph

Contém informações sobre uma reunião, incluindo a URL usada para ingressar em uma reunião, a lista de participantes e a descrição.

## <a name="methods"></a>Métodos

| Método                                                             | Tipo de retorno                       | Descrição                                                                                                  |
| :----------------------------------------------------------------- | :-------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| [Criar ReuniãoOnline](../api/application-post-onlineMeetings.md)  | [onlineMeeting](onlinemeeting.md) | Criar uma reunião online.                                                                                    |
| [Obter onlineMeeting](../api/onlinemeeting-get.md)                   | [onlineMeeting](onlinemeeting.md) | Leia as propriedades e as relações de um **objeto onlineMeeting.**                                        |
| [Update](../api/onlinemeeting-update.md)                           | [onlineMeeting](onlinemeeting.md) | Atualize as propriedades de um **objeto onlineMeeting.** |
| [Excluir onlineMeeting](../api/onlinemeeting-delete.md)             | Nenhum                              | Excluir um **objeto onlineMeeting.**                                                                                    |
| [Criar ou obter OnlineMeeting](../api/onlinemeeting-createorget.md) | [onlineMeeting](onlinemeeting.md) | Crie um **objeto onlineMeeting** com uma ID externa personalizada. Se a reunião já existir, recupere suas propriedades. |

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                                          | Descrição                                                                                                                |
| :-------------------- | :-------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| allowedPresenters     | onlineMeetingPresenters                       | Especifica quem pode ser um apresentador em uma reunião. Os valores possíveis são listados na tabela a seguir.                          |
| audioConferencing     | [audioConferencing](audioconferencing.md)     | As informações de acesso por telefone (discagem) para uma reunião online. Apenas leitura.                                                   |
| chatInfo              | [chatInfo](chatinfo.md)                       | As informações de chat associadas a essa reunião online.                                                                  |
| creationDateTime      | DateTime                                      | O tempo de criação da reunião em UTC. Somente leitura.                                                                               |
| endDateTime           | DateTime                                      | A hora de término da reunião em UTC.                                                                                               |
| id                    | Cadeia de caracteres                                        | A ID padrão associada à reunião online. Somente leitura.                                                              |
| isEntryExitAnnounced  | Booliano                                       | Se os chamadores ingressarão ou sairão.                                                                     |
| joinInformation       | [itemBody](itembody.md)                       | As informações de junção no idioma e na variante de localidade especificadas no `Accept-Language` cabeçalho HTTP da solicitação. Somente leitura. |
| joinWebUrl            | Cadeia de caracteres                                        | A URL de junção da reunião online. Somente leitura.                                                                             |
| lobbyBypassSettings   | [lobbyBypassSettings](lobbyBypassSettings.md) | Especifica quais participantes podem ignorar o lobby da reunião.                                                               |
| participants          | [meetingParticipants](meetingparticipants.md) | Os participantes associados à reunião online.  Isso inclui o organizador e os participantes.                       |
| startDateTime         | DateTime                                      | O horário de início da reunião em UTC.                                                                                             |
| assunto               | Cadeia de caracteres                                        | O assunto da reunião online.                                                                                         |
| videoTeleconferenceId | Cadeia de caracteres                                        | A ID de teleconferência de vídeo. Somente leitura.                                                                                  |

### <a name="onlinemeetingpresenters-values"></a>valores onlineMeetingPresenters

| Valor              | Descrição                                                   |
| ------------------ | ------------------------------------------------------------- |
| everyone           | Todos são apresentadores (essa é a opção padrão).             |
| organização       | Todos na organização do organizador são apresentadores.          |
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

