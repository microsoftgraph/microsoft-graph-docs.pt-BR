---
title: tipo de recurso resourceReference
description: Tipo complexo contendo propriedades de insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 56f1cc992deaa74623930074ea75b6cb0fa9e0ac
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054837"
---
# <a name="resourcereference-resource-type"></a>tipo de recurso resourceReference

Namespace: microsoft.graph

Tipo complexo contendo as propriedades de [officeGraphInsights](officegraphinsights.md).

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso
<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.resourceReference"
}-->
```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo      | Descrição  |
| ------------- |-----------| -------------|
| webUrl        | String    | Uma URL que conduz ao item referenciado. |
| id            | String    | O identificador exclusivo do item.           |
| tipo          | String    | Um valor String que pode ser usado para classificar o item, como "Microsoft. Graph. driveItem" |

