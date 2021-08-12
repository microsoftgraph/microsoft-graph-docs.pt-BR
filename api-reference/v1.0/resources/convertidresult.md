---
title: Tipo de recurso convertIdResult
description: O resultado de uma conversão de formato de ID executada pela função translateExchangeIds.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: ec94f586f0f8233f1b56965f4dea4640360b63eb43f9d1fae69988ae61d401e2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54155159"
---
# <a name="convertidresult-resource-type"></a>Tipo de recurso convertIdResult

Namespace: microsoft.graph

O resultado de uma conversão de formato de ID executada pela [função translateExchangeIds.](../api/user-translateexchangeids.md)

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| sourceId | String | O identificador que foi convertido. Esse valor é o identificador original não convertido. |
| targetId | Cadeia de caracteres | O identificador convertido. Esse valor não estará presente se a conversão falhar. |
| errorDetails | [genericError](genericerror.md) | Um objeto de erro que indica o motivo da falha de conversão. Esse valor não estará presente se a conversão tiver êxito. |

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

