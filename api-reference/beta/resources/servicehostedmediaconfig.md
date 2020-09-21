---
title: tipo de recurso serviceHostedMediaConfig
description: A mídia que está hospedada remotamente.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d006a4417401859c0c385f9537656993f985198d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023951"
---
# <a name="servicehostedmediaconfig-resource-type"></a>tipo de recurso serviceHostedMediaConfig

Namespace: microsoft.graph

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


