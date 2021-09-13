---
title: Tipo de recurso resourceReference
description: Tipo complexo que contém propriedades de Insights.
author: simonhult
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c7694aa2c9a487a3e07ce99d9850445de26c3acb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123360"
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
| id            | String    | O identificador exclusivo do item.           |
| tipo          | Cadeia de caracteres    | Um valor de cadeia de caracteres que pode ser usado para classificar o item, como "microsoft.graph.driveItem" |

