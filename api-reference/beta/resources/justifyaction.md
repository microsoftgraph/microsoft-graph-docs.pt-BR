---
title: tipo de recurso justifyaction
description: Indica que uma justificativa é necessária para a operação especificada.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bc96062febc15310de6a3b2ed04f96a8cf1e69e5
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939310"
---
# <a name="justifyaction-resource-type"></a>tipo de recurso justifyaction

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Indica que uma justificativa é necessária para a operação especificada. As APIs [evaluateApplication](../api/informationprotectionlabel-evaluateApplication.md), [evaluateClassificationResults](../api/informationprotectionlabel-evaluateClassificationResults.md)ou [evaluateRemoval](../api/informationprotectionlabel-evaluateRemoval.md) podem retornar **justifyaction**. A justificativa é fornecida por meio do [labelingOptions](../resources/labelingoptions.md). A chamada anterior deve ser repetida, mas com a propriedade **downgradeJustification** de **labelingOptions** definida com uma mensagem de justificativa, fornecida por meio de entrada do usuário ou lógica do aplicativo.

## <a name="properties"></a>Propriedades

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.justifyAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "justifyAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->