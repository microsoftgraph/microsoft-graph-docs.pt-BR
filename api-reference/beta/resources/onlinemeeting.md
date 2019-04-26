---
title: tipo de recurso onlineMeeting
description: Captura informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d7009ceaf815986d50c8eb3b64d2541c32f01a88
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568854"
---
# <a name="onlinemeeting-resource-type"></a>tipo de recurso onlineMeeting

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Captura informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.

## <a name="methods"></a>Métodos

| Método         | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
| [Obter onlineMeeting](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | Leia as propriedades e os relacionamentos do objeto onlineMeeting. |

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo                                                   | Descrição                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| accessLevel               | String                                                 | O nível de acesso que controla a admissão para a reunião online. Os valores possíveis são: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`. |
| audioConferencing         | [audioConferencing](audioconferencing.md)              | Representa as informações de acesso de telefone de um onlineMeeting. |
| canceledDateTime          | DateTime                                               | A hora em que a reunião foi cancelada. |
| chatInfo                  | [chatInfo](chatinfo.md)                                | O chat associado a esta reunião. |
| creationDatetime          | DateTime                                               | A hora em que a reunião foi criada. ReadOnly.
| endDateTime               | DateTime                                               | Hora de término da reunião. |
| entryExitAnnouncement     | Booliano                                                | O status dos comunicados de presença para a reunião online. Quando os comunicados de presença estiverem habilitados, a reunião online anunciará os nomes do participantswho ingressar na reunião por meio de áudio. |
| expirationDateTime        | DateTime                                               | A data e a hora UTC (tempo Universal Coordenado) absoluta após a qual a reunião online pode ser excluída. O dia e a hora devem estar entre um ano antes e dez anos após, a data e a hora atuais no servidor. |
| id                        | String                                                 | A ID associada à reunião online. Usado em uma solicitação HTTP GET como a ID. Somente leitura. Servidor gerado. |
| isCancelled               | Booliano                                                | Se a reunião foi cancelada. |
| joinUrl                   | String                                                 | A URL que é usada quando a reunião online é associada da Web. |
| meetingtype               | String                                                 | Os valores possíveis são `meetNow`: `scheduled`, `recurring`,,`broadcast` |
| participantes              | [meetingParticipants](meetingparticipants.md)          | Os participantes associados à reunião online.  Isso inclui o organizador e os participantes. |
| startDateTime             | DateTime                                               | Hora de início da reunião. |
| subject                   | String                                                 | O assunto da reunião online. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onlineMeeting"
}-->
```json
{
  "accessLevel": "everyone | invited | locked | sameEnterprise",
  "audioConferencing": {"@odata.type": "#microsoft.graph.audioConferencing"},
  "canceledDateTime": "String (timestamp)",
  "chatInfo": {"@odata.type": "#microsoft.graph.chatInfo"},
  "creationDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "entryExitAnnouncement": true,
  "expirationDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "isCancelled": false,
  "joinUrl": "String",
  "meetingType": "meetNow | scheduled | recurring | broadcast",
  "participants": {"@odata.type": "#microsoft.graph.meetingParticipants"},
  "startDateTime": "String (timestamp)",
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onlinemeeting.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
