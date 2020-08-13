---
title: Tipo de recurso workbookSessionInfo
description: Fornece informações sobre a sessão de pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 6d0565edea02d0333f6aa3b97b376ea3c7f32c68
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519145"
---
# <a name="workbooksessioninfo-resource-type"></a>Tipo de recurso workbookSessionInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Fornece informações sobre a sessão de pasta de trabalho.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.workbookSessionInfo"
}-->

```json
{
  "id": "string",
  "persistChanges": true
}
```

## <a name="properties"></a>Propriedades

| Propriedade | Tipo  | Descrição                               |
|:---------|:------|:------------------------------------------|
| id  | cadeia de caracteres | ID da sessão de pasta de trabalho. |
| persistChanges | string |  `true` para sessão persistente. `false` para sessão não persistente (modo de exibição) |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookSessionInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
