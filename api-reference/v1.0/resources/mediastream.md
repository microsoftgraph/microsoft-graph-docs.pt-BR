---
title: Tipo de recurso mediaStream
description: O tipo mediaStream.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4fa45c863bf06d2c1c2083a1f66796abcb46eaff
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134602"
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

