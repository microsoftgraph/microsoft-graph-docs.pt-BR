---
title: Tipo de recurso mediaStream
description: O tipo mediaStream.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 98fa09655faa6068c48c6fe2d1e340fa28ff253b99717900bed5d9f863561c1b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141438"
---
# <a name="mediastream-resource-type"></a>Tipo de recurso mediaStream

Namespace: microsoft.graph

Isso contém informações sobre o canal de mídia.

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo    | Descrição                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| direction   | String  | A direção. Os valores possíveis `inactive` são , , , `sendOnly` `receiveOnly` `sendReceive` .                  |
| rótulo       | Cadeia de caracteres  | O rótulo de fluxo de mídia.                                                                                       |
| mediaType   | Cadeia de caracteres  | O tipo de mídia. O valor possível é `unknown` , , , , `audio` `video` `videoBasedScreenSharing` `data` .        |
| serverMuted | Booliano | Se a mídia for silenciada pelo servidor.                                                                          |
| sourceId    | Cadeia de caracteres  | A ID de origem.                                                                                                |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted",
    "label"
  ],
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "inactive | sendOnly | receiveOnly | sendReceive",
  "label": "String",
  "mediaType": "unknown | audio | video | videoBasedScreenSharing | data",
  "serverMuted": true,
  "sourceId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

