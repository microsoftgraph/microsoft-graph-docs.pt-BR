---
title: tipo de recurso convertIdResult
description: O resultado de uma conversão de formato de ID executada pela função translateExchangeIds.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: aa663420dd7b6e1c79e03af675b1f505c08cb875
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091849"
---
# <a name="convertidresult-resource-type"></a>tipo de recurso convertIdResult

Namespace: microsoft.graph

O resultado de uma conversão de formato de ID executada pela função [translateExchangeIds](../api/user-translateexchangeids.md) .

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| sourceId | Cadeia de caracteres | O identificador que foi convertido. Esse valor é o identificador original não convertido. |
| targetId | Cadeia de caracteres | O identificador convertido. Esse valor não estará presente se a conversão tiver falhado. |
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

