---
title: Tipo de recurso expressionEvaluationDetails
description: Representa os detalhes, o resultado e a propriedade de expressão.
localization_priority: Normal
author: Jordanndahl
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: a2e2b2620f30234c23753ef743f14e55e29f6f91
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52679894"
---
# <a name="expressionevaluationdetails-resource-type"></a>Tipo de recurso expressionEvaluationDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes, o resultado e a propriedade de expressão.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| expressão | String | Representa a expressão que foi avaliada. |
| expressionEvaluationDetails | Coleção expressionEvaluationDetails | Representa os detalhes da avaliação da expressão. |
| expressionResult | Boolean | Representa o valor do resultado da expressão atual. |
| propertyToEvaluate | [propertyToEvaluate](propertytoevaluate.md) | Define o nome da propriedade e o valor dessa propriedade. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.expressionEvaluationDetails",
  "baseType": null
}-->

```json
{
  "expression": "String",
  "expressionEvaluationDetails": [{"@odata.type": "microsoft.graph.expressionEvaluationDetails"}],
  "expressionResult": true,
  "propertyToEvaluate": {"@odata.type": "microsoft.graph.propertyToEvaluate"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "expressionEvaluationDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


