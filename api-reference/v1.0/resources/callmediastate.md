---
title: tipo de recurso callMediaState
description: Representa o estado de mídia de uma chamada.
author: ananmishr
ms.prod: cloud-communications
ms.localizationpriority: medium
doc_type: resourcePageType
ms.openlocfilehash: d07562bfaf14a69175535f8b38b73f56fdb0faa8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59104359"
---
# <a name="callmediastate-resource-type"></a>tipo de recurso callMediaState

Namespace: microsoft.graph


Representa o estado de mídia de uma [chamada](call.md).

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo    | Descrição                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| audio           | mediaState  | O estado da mídia de áudio. Os valores possíveis são: `active`, `inactive`, `unknownFutureValue`. |

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

