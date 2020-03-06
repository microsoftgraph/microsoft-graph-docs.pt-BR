---
title: tipo de recurso convertIdResult
description: O resultado de uma conversão de formato de ID executada pela função translateExchangeIds.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: svpsiva
ms.openlocfilehash: 6eb66033ef1b0e345c3929982b9f08d6e4ce2573
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531747"
---
# <a name="convertidresult-resource-type"></a>tipo de recurso convertIdResult

Namespace: microsoft.graph

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
