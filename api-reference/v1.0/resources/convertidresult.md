---
title: Tipo de recurso convertIdResult
description: O resultado de uma conversão de formato de ID executada pela função translateExchangeIds.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 1710c437421426b4bd072e3c654df7d076d0f9f7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135151"
---
# <a name="convertidresult-resource-type"></a>Tipo de recurso convertIdResult

Namespace: microsoft.graph

O resultado de uma conversão de formato de ID executada pela [função translateExchangeIds.](../api/user-translateexchangeids.md)

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| sourceId | String | O identificador que foi convertido. Esse valor é o identificador original não convertido. |
| targetId | String | O identificador convertido. Esse valor não estará presente se a conversão falhar. |
| errorDetails | [genericError](genericerror.md) | Um objeto de erro indicando o motivo da falha de conversão. Esse valor não estará presente se a conversão tiver êxito. |

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

