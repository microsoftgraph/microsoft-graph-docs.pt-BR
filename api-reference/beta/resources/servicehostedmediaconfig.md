---
title: tipo de recurso serviceHostedMediaConfig
description: A mídia que está hospedada remotamente.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 405f6b40260908d7492a3b02c8535588c8475ca8
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870086"
---
# <a name="servicehostedmediaconfig-resource-type"></a>tipo de recurso serviceHostedMediaConfig

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A mídia que está hospedada remotamente. Isso é herdado de [mediaConfig](mediaconfig.md).

## <a name="properties"></a>Propriedades

| Propriedade                    | Tipo                                                        | Descrição                                       |
| :-------------------------- | :---------------------------------------------------------- | :-------------------------------------------------|
| preFetchMedia               | coleção [mediaInfo](mediainfo.md)                        | A lista de mídias a buscar previamente.                   |
| removeFromDefaultAudioGroup | Booliano                                                     | Remover o próprio participante do grupo de áudio padrão. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "preFetchMedia"
  ],
  "baseType": "microsoft.graph.mediaConfig",
  "@odata.type": "microsoft.graph.serviceHostedMediaConfig"
}-->
```json
{
  "preFetchMedia": [ { "@odata.type": "microsoft.graph.mediaInfo" } ],
  "removeFromDefaultAudioGroup": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "serviceHostedMediaConfig resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
