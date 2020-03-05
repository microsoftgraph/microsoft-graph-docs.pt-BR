---
title: tipo de recurso callMediaState
description: Representa o estado de mídia de uma chamada.
author: ananmishr
ms.prod: cloud-communications
localization_priority: Normal
doc_type: resourcePageType
ms.openlocfilehash: c9c55908f62214c386aacee34be76bb11fc318b7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507807"
---
# <a name="callmediastate-resource-type"></a>tipo de recurso callMediaState

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o estado de mídia de uma [chamada](call.md).

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo    | Descrição                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| audio           | String  | O estado da mídia de áudio. Os valores possíveis são: `active` e `inactive`. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callMediaState"
}-->
```json
{
  "audio": "active | inactive",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "callMediaState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
