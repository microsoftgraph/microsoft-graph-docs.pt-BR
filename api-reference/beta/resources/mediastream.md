---
title: tipo de recurso mediaStream
description: Contém informações sobre o canal de mídia.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0274cdb1c35307e91e31c0b357ecf9a16e2d3f19
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913076"
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
