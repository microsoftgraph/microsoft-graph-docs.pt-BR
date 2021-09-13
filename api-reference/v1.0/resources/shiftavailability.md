---
title: Tipo de recurso shiftAvailability
description: Disponibilidade do usuário a ser agendado para o trabalho e seu padrão de recorrência.
ms.localizationpriority: medium
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e04cbdd14349b4ffc3f01ce22c10948e5fbaff0e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59032178"
---
# <a name="shiftavailability-resource-type"></a>Tipo de recurso shiftAvailability

Namespace: microsoft.graph

Disponibilidade do usuário a ser agendado para um [turno](shift.md) e seu padrão de recorrência.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|recurrence|[patternedRecurrence](patternedrecurrence.md)| Especifica o padrão para recorrência |
|timeSlots|[Coleção timeRange](timerange.md)|Os intervalos de tempo preferidos pelo usuário.|
|timeZone|Cadeia de caracteres|Especifica o fuso horário para a hora indicada. |

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

