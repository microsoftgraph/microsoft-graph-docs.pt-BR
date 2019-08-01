---
title: Tipo de recurso patternedRecurrence
description: O padrão e o intervalo da recorrência.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a5ad30474b23c6ef96bbc1a66142098e7f696138
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035564"
---
# <a name="patternedrecurrence-resource-type"></a>Tipo de recurso patternedRecurrence

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
