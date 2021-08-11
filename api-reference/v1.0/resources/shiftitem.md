---
title: Tipo de recurso shiftItem
description: Um shiftItem representa uma versão do shift.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 97891ada6a9587f6ef679bdc13d58564ab407cc623c6c3b339fc7f4e289894c9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54189314"
---
# <a name="shiftitem-resource-type"></a>Tipo de recurso shiftItem

Namespace: microsoft.graph

Representa uma versão de um [turno](shift.md).

## <a name="properties"></a>Propriedades
| Propriedade                         | Tipo                    | Descrição                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| notes               | string                  | As notas de turno para `shiftItem` o .      |
| displayName               | string                  | O rótulo de turno do `shiftItem` . |
| startDateTime               | DateTimeOffset                  | A data e a hora de início do `shiftItem` . O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Obrigatório. |
| endDateTime               | DateTimeOffset                 | A data e a hora de término do `shiftItem` . Obrigatório. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. |
| tema | scheduleEntityTheme   |  Cores com suporte: branco; azul; verde; roxo; rosa; amarelo; cinza; darkBlue; darkGreen; darkPurple; darkPink; darkYellow. |
| activities    | [Coleção shiftActivity](shiftactivity.md)   | Uma parte incremental de um turno que pode abranger detalhes de quando e onde um funcionário está durante o turno. Por exemplo, uma atribuição ou uma pausa ou almoço agendado. Obrigatório. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftItem"
}-->
```json
{
  "displayName": "String",
  "notes": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "theme": "String",
  "activities": [{"@odata.type": "microsoft.graph.shiftActivity"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

