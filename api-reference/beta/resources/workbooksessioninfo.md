---
title: Tipo de recurso workbookSessionInfo
description: Fornece informações sobre a sessão de pasta de trabalho.
author: lumine2008
ms.openlocfilehash: 5a86fd4dfd653f16445eeccad8478db56db0ac5f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316839"
---
# <a name="workbooksessioninfo-resource-type"></a>Tipo de recurso workbookSessionInfo

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
| id  | string | ID da sessão de pasta de trabalho. |
| persistChanges | string |  `true` para sessão persistente. `false` para sessão não persistente (modo de exibição) |

