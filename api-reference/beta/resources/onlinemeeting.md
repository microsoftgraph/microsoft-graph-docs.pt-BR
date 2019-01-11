---
title: tipo de recurso de onlineMeeting
description: Informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição de captura.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: b1a0b09c0e7c792b0a9662c08daecd212c027c89
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805156"
---
# <a name="onlinemeeting-resource-type"></a>tipo de recurso de onlineMeeting

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Informações sobre a reunião, incluindo a URL de ingresso, a lista de participantes e a descrição de captura.

## <a name="methods"></a>Métodos

| Método         | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
| [Obter onlineMeeting](../api/onlinemeeting-get.md) | [onlineMeeting](onlinemeeting.md) | Leia as propriedades e os relacionamentos do objeto onlineMeeting. |

## <a name="properties"></a>Propriedades

| Propriedade                  | Tipo                                                   | Descrição                                                                                                                |
| :------------------------ | :----------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------- |
| accessLevel               | Cadeia de caracteres                                                 | O nível de acesso que controla a admissão na reunião online. Os valores possíveis são: `everyone`, `invited`, `locked`, `sameEnterprise`, `unknown`. |
| audioConferencing         | [audioConferencing](audioconferencing.md)              | Representa as informações de acesso telefônicas de um onlineMeeting. |
| canceledDateTime          | DateTime                                               | A hora de quando a reunião foi cancelada. |
| chatInfo                  | [chatInfo](chatinfo.md)                                | O chat associado a esta reunião. |
| creationDateTime          | DateTime                                               | A hora em que a reunião foi criada. ReadOnly.
| endDateTime               | DateTime                                               | Hora de término da reunião. |
| entryExitAnnouncement     | Booliano                                                | O status de comunicados de participação da reunião online. Quando os anúncios de presença estão habilitados, a reunião online lançará os nomes dos participantswho ingressar na reunião através do áudio. |
| expirationDateTime        | DateTime                                               | A data de tempo Universal Coordenado (UTC) e a hora após o qual a absoluto da reunião online pode ser excluída. O dia e hora devem estar entre um ano antes e dez anos após a data atual e a hora no servidor. |
| id                        | Cadeia de caracteres                                                 | A ID associada a reunião online. Usado em uma solicitação HTTP GET, como a ID. Somente leitura. Servidor foi gerado. |
| isCancelled               | Booliano                                                | Se a reunião foi cancelada. |
| joinUrl                   | Cadeia de caracteres                                                 | A URL que é usada durante a reunião online está unida a partir da web. |
| meetingType               | Cadeia de caracteres                                                 | Os valores possíveis são: `meetNow`, `scheduled`, `recurring`,`broadcast` |
| participantes              | [meetingParticipants](meetingparticipants.md)          | Os participantes associados a reunião online.  Isso inclui o organizador e os participantes. |
| startDateTime             | DateTime                                               | Inicie o horário da reunião. |
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeeting resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
