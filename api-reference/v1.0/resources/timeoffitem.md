---
title: Tipo de recurso timeOffItem
description: Representa uma versão do timeOff.
author: akumar39
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 349b37cfdc414323d35ee4648009fd8ab4d59bbf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59019101"
---
# <a name="timeoffitem-resource-type"></a>Tipo de recurso timeOffItem

Namespace: microsoft.graph

Representa uma versão do [timeOff](timeoff.md).

## <a name="properties"></a>Propriedades
| Propriedade                         | Tipo                    | Descrição                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| timeOffReasonId               | cadeia de caracteres                  | ID do `timeOffReason` para isso `timeOffItem` . Obrigatório.     |
| startDateTime               | DateTimeOffset                  | A data e a hora de início do `timeOffItem` . Obrigatório. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
| endDateTime               | DateTimeOffset                  | A data e a hora de término do `timeOffItem` . Obrigatório. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
| tema | scheduleEntityTheme   | Cores com suporte: branco; azul; verde; roxo; rosa; amarelo; cinza; darkBlue; darkGreen; darkPurple; darkPink; darkYellow. |

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

