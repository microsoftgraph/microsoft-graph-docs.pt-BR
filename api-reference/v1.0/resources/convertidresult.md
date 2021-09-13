---
title: Tipo de recurso convertIdResult
description: O resultado de uma conversão de formato de ID executada pela função translateExchangeIds.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: e2bb28e7ee4d889fec24152de27e37399e8acfa1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59053151"
---
# <a name="convertidresult-resource-type"></a>Tipo de recurso convertIdResult

Namespace: microsoft.graph

O resultado de uma conversão de formato de ID executada pela [função translateExchangeIds.](../api/user-translateexchangeids.md)

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| sourceId | Cadeia de caracteres | O identificador que foi convertido. Esse valor é o identificador original não convertido. |
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

