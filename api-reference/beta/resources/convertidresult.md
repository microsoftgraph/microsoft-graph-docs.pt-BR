---
title: tipo de recurso convertIdResult
description: O resultado de uma conversão de formato de ID executada pela função translateExchangeIds.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 040b13ab83eacffb33e8903f7d11823adb6e1bf1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973190"
---
# <a name="convertidresult-resource-type"></a>tipo de recurso convertIdResult

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O resultado de uma conversão de formato de ID executada pela função [translateExchangeIds](../api/user-translateexchangeids.md) .

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| sourceId | String | O identificador que foi convertido. Esse valor é o identificador original não convertido. |
| targetId | String | O identificador convertido. Esse valor não estará presente se a conversão tiver falhado. |
| errorDetails | [genericError](genericerror.md) | Um objeto Error que indica o motivo da falha de conversão. Esse valor não estará presente se a conversão tiver sido bem-sucedida. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "targetId",
    "errorDetails"
  ],
  "@odata.type": "microsoft.graph.convertIdResult"
}-->

```json
{
  "sourceId": "String",
  "targetId": "String",
  "errorDetails": {
    "@odata.type": "microsoft.graph.genericError"
  }
}
```
