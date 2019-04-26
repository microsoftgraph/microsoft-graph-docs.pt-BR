---
title: tipo de recurso onlineMeeting
description: Captura informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 698058fa918462448fcd115d5573e13ada49162e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341838"
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
| creationDatetime          | DateTime                                               | A hora em que a reunião foi criada. Somente leitura.
| endDateTime               | DateTime                                               | Hora de término da reunião. |
| entryExitAnnouncement     | Boolean                                                | O status dos comunicados de presença para a reunião online. Quando os comunicados de presença estiverem habilitados, a reunião online anunciará os nomes dos participantes que ingressarem na reunião por meio de áudio. |
| expirationDateTime        | DateTime                                               | A data e a hora UTC (tempo Universal Coordenado) absoluta após a qual a reunião online pode ser excluída. O dia e a hora devem estar entre um ano antes e dez anos após, a data e a hora atuais no servidor. |
| id                        | String                                                 | A ID associada à reunião online. Usado em uma solicitação HTTP GET como a ID. Somente leitura. Servidor gerado. |
| isCancelled               | Booliano                                                | Se a reunião foi cancelada. |
| joinUrl                   | String                                                 | A URL que é usada quando a reunião online é associada da Web. |
| meetingtype               | String                                                 | Os valores possíveis são `meetNow`: `scheduled`, `recurring`, `broadcast` , (Observação: a [criação](../api/application-post-onlinemeetings.md) de `meetNow`onlineMeeting só oferece suporte). |
| participantes              | [meetingParticipants](meetingparticipants.md)          | Os participantes associados à reunião online.  Isso inclui o organizador e os participantes. |
| startDateTime             | DateTime                                               | Hora de início da reunião. |
| subject                   | Cadeia de caracteres                                                 | O assunto da reunião online. |

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