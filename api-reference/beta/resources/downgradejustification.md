---
title: Tipo de recurso downgradeJustification
description: Representa a entrada do usuário sobre por que a rebaixamento foi realizada.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: bc7336469f93de9e6d2b07fe73df9dce2eafd47f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941796"
---
# <a name="downgradejustification-resource-type"></a>Tipo de recurso downgradeJustification

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a entrada do usuário sobre por que a rebaixamento foi realizada. A justificativa de downgrade pode ser necessária com base na configuração da política de rótulo no Centro de Conformidade e Segurança do Office.

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo    | Descrição                                                                                          |
| :------------------- | :------ | :--------------------------------------------------------------------------------------------------- |
| isDowngradeJustified | Booliano | Indica se a rebaixamento é ou não justificada.                                              |
| justificationMessage | Cadeia de caracteres  | Mensagem que indica por que uma rebaixamento é justificada. A mensagem aparecerá em logs administrativos. |

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

