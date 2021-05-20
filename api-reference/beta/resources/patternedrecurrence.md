---
title: Tipo de recurso patternedRecurrence
description: O padrão e o intervalo da recorrência.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: harini84
ms.openlocfilehash: baff2147ee0a9e03e4e55a143341171707dee2d7
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579299"
---
# <a name="patternedrecurrence-resource-type"></a>Tipo de recurso patternedRecurrence

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O padrão e o intervalo da recorrência.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|pattern|[recurrencePattern](recurrencepattern.md)|A frequência de um evento. Não especifique para uma revisão de acesso único.|
|intervalo|[recurrenceRange](recurrencerange.md)|A duração de um evento.|

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
<!--
{
  "type": "#page.annotation",
  "description": "patternedRecurrence resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


