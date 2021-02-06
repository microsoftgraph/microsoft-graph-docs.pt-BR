---
title: Tipo de recurso expressionEvaluationDetails
description: Representa os detalhes da expressão, o resultado e os detalhes da propriedade.
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: 01cc4aa4bd6de88541d3886efe54e5da71228448
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129485"
---
# <a name="expressionevaluationdetails-resource-type"></a>Tipo de recurso expressionEvaluationDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes da expressão, o resultado e os detalhes da propriedade.

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


