---
title: tipo de recurso expressionEvaluationDetails
description: Representa os detalhes de propriedade, resultado e detalhes da expressão.
localization_priority: Normal
author: yyuank
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 347e356bda19228ea8b3738b5bf8b72f57da95f7
ms.sourcegitcommit: 62c900af626e46439d949462f09061cc5c41d6ff
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/16/2020
ms.locfileid: "44272819"
---
# <a name="expressionevaluationdetails-resource-type"></a>tipo de recurso expressionEvaluationDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de propriedade, resultado e detalhes da expressão.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| expressão | Cadeia de Caracteres | Representa a expressão que foi avaliada. |
| expressionEvaluationDetails | coleção expressionEvaluationDetails | Representa os detalhes da avaliação da expressão. |
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
