---
title: tipo de recurso timeOffItem
description: Representa uma versão do timeOff.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c83a8725a0048a622ed88ec8265be76c30e46cc0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582853"
---
# <a name="timeoffitem-resource-type"></a>tipo de recurso timeOffItem

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma versão do [timeOff](timeoff.md).

## <a name="properties"></a>Propriedades
| Propriedade                         | Tipo                    | Descrição                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| timeOffReasonId               | `string`                  | ID do `timeOffReason` para isso `timeOffItem`. Obrigatório.     |
| startDateTime               | `DateTimeOffset`                  | A data e a hora de início `timeOffItem`para o. Obrigatório. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
| endDateTime               | `DateTimeOffset`                  | A data e a hora de término `timeOffItem`para o. Obrigatório. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
| tema | `enum`   | Cores suPortadas: branco; azuis natureza roxa Rosa amarelo acinzentada darkBlue; darkGreen; darkPurple; darkPink; darkYellow. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffItem"
}-->
```json
{
  "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
  "startDateTime": "2019-03-11T07:00:00Z",
  "endDateTime": "2019-03-12T07:00:00Z",
  "theme": "pink"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeOffItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/timeoffitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
