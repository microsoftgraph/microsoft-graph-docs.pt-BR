---
title: tipo de recurso downgradeJustification
description: Representa a entrada do usuário sobre por que o downgrade foi realizado.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 91bcb5a8e12a159bf2c6586a0e3dc49a540a69f2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505788"
---
# <a name="downgradejustification-resource-type"></a>tipo de recurso downgradeJustification

Namespace: microsoft.graph

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