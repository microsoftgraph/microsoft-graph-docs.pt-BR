---
title: tipo de recurso genericError
description: Um erro de uso geral.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 701a3b7ed0d7bad6e33f8ba41e77ec7340a57146
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973521"
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
