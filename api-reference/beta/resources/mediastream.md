---
title: tipo de recurso mediaStream
description: Contém informações sobre o canal de mídia.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: de5c90453d9adb657c2df5ee761d847056664037
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870177"
---
# <a name="mediastream-resource-type"></a>tipo de recurso mediaStream

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém informações sobre o canal de mídia.

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo    | Descrição                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| direction   | String  | A direção. Os valores possíveis são `inactive`: `sendOnly` `receiveOnly`,, `sendReceive`,.                  |
| rótulo       | String  | O rótulo do fluxo de mídia.                                                                                       |
| Mídia   | String  | O tipo de mídia. O valor possível é `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.        |
| serverMuted | Booliano | Indica se a mídia está com mudo ativado pelo servidor.                                                                          |
| sourceId    | String  | A ID da fonte.                                                                                                |

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
