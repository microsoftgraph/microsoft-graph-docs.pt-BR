---
title: tipo de recurso shiftAvailability
description: Disponibilidade do usuário a ser agendada para trabalho e seu padrão de recorrência.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4a284774b76774da0420322f0cd2e092aec6ce83
ms.sourcegitcommit: ed03445225e98cf0881de08273c36be8d0e576ea
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2020
ms.locfileid: "40952283"
---
# <a name="shiftavailability-resource-type"></a>tipo de recurso shiftAvailability

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Disponibilidade do usuário a ser agendada para um [turno](shift.md) e seu padrão de recorrência.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|recurrence|[patternedRecurrence](patternedrecurrence.md)| Especifica o padrão de recorrência |
|Intervalos|coleção [timerange](timerange.md)|O (s) intervalo (s) de tempo preferido pelo usuário.|
|timeZone|Cadeia de caracteres|Especifica o fuso horário do horário indicado. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.shiftAvailability",
  "baseType": null
}-->

```json
{
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "timeSlots": [{"@odata.type": "microsoft.graph.timeRange"}],
  "timeZone": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "shiftAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
