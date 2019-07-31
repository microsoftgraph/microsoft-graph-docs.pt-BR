---
title: tipo de recurso timeOffItem
description: Representa uma versão do timeOff.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 6b240f587e20e2da178f9afa3e8d712cf2ae114d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964302"
---
# <a name="timeoffitem-resource-type"></a>tipo de recurso timeOffItem

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma versão do [timeOff](timeoff.md).

## <a name="properties"></a>Propriedades
| Propriedade                         | Tipo                    | Descrição                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| timeOffReasonId               | string                  | ID do `timeOffReason` para isso `timeOffItem`. Obrigatório.     |
| startDateTime               | DateTimeOffset                  | A data e a hora de início `timeOffItem`para o. Obrigatório. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
| endDateTime               | DateTimeOffset                  | A data e a hora de término `timeOffItem`para o. Obrigatório. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
| tema | scheduleEntityTheme   | Cores suportadas: branco; azuis natureza roxa Rosa amarelo acinzentada darkBlue; darkGreen; darkPurple; darkPink; darkYellow. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffItem"
}-->
```json
{
  "timeOffReasonId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
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
  "suppressions": []
}
-->
