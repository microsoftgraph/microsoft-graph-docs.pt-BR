---
title: tipo de recurso genericError
description: Um erro de uso geral.
localization_priority: Normal
ms.openlocfilehash: 314bb5f5e94e44c326fceb71f4a79463989f2129
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333660"
---
# <a name="genericerror-resource-type"></a>tipo de recurso genericError

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um erro de uso geral.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| mensagem | String | A mensagem de erro. |
| código | String | O código de erro. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.genericError"
}-->

```json
{
  "message": "String",
  "code": "String"
}
```
