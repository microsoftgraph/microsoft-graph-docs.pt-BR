---
title: Tipo de recurso expressionEvaluationDetails
description: Representa os detalhes, o resultado e a propriedade de expressão.
ms.localizationpriority: medium
author: psaffaie
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: d588719e8d6bcf32ff337beec8815b6fe329ee0b
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587032"
---
# <a name="expressionevaluationdetails-resource-type"></a>Tipo de recurso expressionEvaluationDetails

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes, o resultado e a propriedade de expressão.

## <a name="properties"></a>Propriedades

| Propriedade                    | Tipo                                        | Descrição                                                      |
| :-------------------------- | :------------------------------------------ | :--------------------------------------------------------------- |
| expressão                  | Cadeia de caracteres                                      | Representa a expressão que foi avaliada.                  |
| expressionEvaluationDetails | Coleção expressionEvaluationDetails      | Representa os detalhes da avaliação da expressão.      |
| expressionResult            | Boolean                                     | Representa o valor do resultado da expressão atual.    |
| propertyToEvaluate          | [propertyToEvaluate](propertytoevaluate.md) | Define o nome da propriedade e o valor dessa propriedade. |

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
  "expressionEvaluationDetails": [
    { "@odata.type": "microsoft.graph.expressionEvaluationDetails" }
  ],
  "expressionResult": true,
  "propertyToEvaluate": { "@odata.type": "microsoft.graph.propertyToEvaluate" }
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
