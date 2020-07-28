---
title: tipo de recurso resourceReference
description: Tipo complexo contendo propriedades de insights.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: fac5ec3b40467034a583933a6e09399e91badfe0
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427393"
---
# <a name="resourcereference-resource-type"></a>tipo de recurso resourceReference

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Tipo complexo contendo propriedades de item de [informações](iteminsights.md)

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
| tipo          | Cadeia de caracteres    | Um valor String que pode ser usado para classificar o item, como "Microsoft. Graph. driveItem" |
