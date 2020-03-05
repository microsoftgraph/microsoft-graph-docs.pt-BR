---
title: tipo de recurso shiftItem
description: Um shiftItem representa uma versão do turno.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9ea8999a500f937e5863819554562ffc84bbdad7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520615"
---
# <a name="shiftitem-resource-type"></a>tipo de recurso shiftItem

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma versão de um [turno](shift.md).

## <a name="properties"></a>Propriedades
| Propriedade                         | Tipo                    | Descrição                                                                             |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| notes               | string                  | As notas para o `shiftItem`.      |
| displayName               | string                  | O nome do `shiftItem`. |
| startDateTime               | DateTimeOffset                  | A data e a hora de início `shiftItem`para o. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. Obrigatório. |
| endDateTime               | DateTimeOffset                 | A data e a hora de término `shiftItem`para o. Obrigatório. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. |
| tema | scheduleEntityTheme   |  Cores suportadas: branco; azuis natureza roxa Rosa amarelo acinzentada darkBlue; darkGreen; darkPurple; darkPink; darkYellow. |
| activities    | coleção [shiftActivity](shiftactivity.md)   | Uma parte incremental de um turno que pode abranger detalhes de quando e onde um funcionário está durante o turno. Por exemplo, uma atribuição ou uma quebra ou almoço agendado. Obrigatório. |

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
