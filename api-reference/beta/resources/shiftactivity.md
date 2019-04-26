---
title: tipo de recurso shiftActivity
description: Representa uma atividade em um turno.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 24946630e9bc3ae9ba418f5c322ab212c022d6d1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343068"
---
# <a name="shiftactivity-resource-type"></a>tipo de recurso shiftActivity

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma atividade em um [turno](shift.md).

## <a name="properties"></a>Propriedades
| Propriedade                         | Tipo                    | Descrição                                                                                                                                                                        |
|------------------------------|-------------------------|---------------------------------------------------------------------------------------------|
| isPago               | `bool`                  | Indica se o `microsoft.graph.user` deve ser pago para a atividade durante seu `shift`. Obrigatório.    |
| startDateTime               | `DateTimeOffset`                  | A data e a hora de início `shiftActivity`para o. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. Obrigatório. |
| endDateTime               | `DateTimeOffset`                  | A data e a hora de término `shiftActivity`para o. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: '2014-01-01T00:00:00Z'. Obrigatório.    |
| código               | `string`                  | Código definido pelo cliente para `shiftActivity`o. Obrigatório.    |
| displayName               | `string`                  | O nome do `shiftActivity`. Obrigatório.    |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shiftActivity"
}-->
```json
{
  "isPaid": true,
  "startDateTime": "2019-03-11T15:00:00Z",
  "endDateTime": "2019-03-11T15:15:00Z",
  "code": "",
  "displayName": "Lunch"
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "shiftActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
