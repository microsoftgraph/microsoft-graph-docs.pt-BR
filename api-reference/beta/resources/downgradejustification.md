---
title: tipo de recurso downgradeJustification
description: Representa a entrada do usuário sobre por que o downgrade foi realizado.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: aacc32ac86df4eda087f49dbb3dca05a356e8080
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939422"
---
# <a name="downgradejustification-resource-type"></a>tipo de recurso downgradeJustification

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a entrada do usuário sobre por que o downgrade foi realizado. A justificação de downgrade pode ser necessária com base na configuração de política de rótulo no centro de conformidade e segurança do Office.

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo    | Descrição                                                                                          |
| :------------------- | :------ | :--------------------------------------------------------------------------------------------------- |
| isDowngradeJustified | Booliano | Indica se o downgrade é ou não justificado.                                              |
| justificationMessage | String  | Mensagem que indica por que um downgrade é justificado. A mensagem aparecerá em logs administrativos. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.downgradeJustification",
  "baseType": null
}-->

```json
{
  "isDowngradeJustified": true,
  "justificationMessage": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "downgradeJustification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->