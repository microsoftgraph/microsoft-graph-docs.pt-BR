---
title: tipo de recurso mediaPrompt
description: O tipo mediaPrompt.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: b8824a6fb2dcef69568821c251d0b44fa3d2edf7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009780"
---
# <a name="mediaprompt-resource-type"></a>tipo de recurso mediaPrompt

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo mediaPrompt.

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo                      | Descrição                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| mediaInfo   | [mediaInfo](mediainfo.md) | As informações de mídia                                                           |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

## <a name="example"></a>Exemplo

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->
```json
{
  "@odata.type": "#microsoft.graph.mediaPrompt",
  "mediaInfo": {
    "@odata.type": "#microsoft.graph.mediaInfo",
    "uri": "https://cdn.contoso.com/beep.wav",
    "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
