---
title: Tipo de recurso resourceReference
description: Tipo complexo que contém propriedades de Insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 7ade1e86fc601d1f00a16136a8610634934d0b4faf7b377a85ff55cf65fab671
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54152618"
---
# <a name="resourcereference-resource-type"></a>Tipo de recurso resourceReference

Namespace: microsoft.graph

Tipo complexo que contém propriedades do [officeGraphInsights](officegraphinsights.md).

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
| id            | Cadeia de caracteres    | O identificador exclusivo do item.           |
| tipo          | Cadeia de caracteres    | Um valor de cadeia de caracteres que pode ser usado para classificar o item, como "microsoft.graph.driveItem" |

