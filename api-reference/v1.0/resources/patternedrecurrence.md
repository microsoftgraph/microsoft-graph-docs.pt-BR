---
title: Tipo de recurso patternedRecurrence
description: O padrão e o intervalo da recorrência.
localization_priority: Normal
author: harini84
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 57e42faaaa30be31c45be7bfec6ad9ee17ffc869
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546200"
---
# <a name="patternedrecurrence-resource-type"></a>Tipo de recurso patternedRecurrence

Namespace: microsoft.graph

O padrão e o intervalo da recorrência.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|pattern|[RecurrencePattern](recurrencepattern.md)|A frequência de um evento.|
|range|[RecurrenceRange](recurrencerange.md)|A duração de um evento.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.patternedRecurrence"
}-->

```json
{
  "pattern": {"@odata.type": "microsoft.graph.recurrencePattern"},
  "range": {"@odata.type": "microsoft.graph.recurrenceRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

