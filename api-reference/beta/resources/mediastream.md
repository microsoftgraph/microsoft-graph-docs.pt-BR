---
title: tipo de recurso mediaStream
description: O tipo mediaStream.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c39c4eb0754f327361fec04852293ef084b0c412
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966822"
---
# <a name="mediastream-resource-type"></a>tipo de recurso mediaStream

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo mediaStream.

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo    | Descrição                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| direction   | String  | A direção. Os valores possíveis são `inactive`: `sendOnly` `receiveOnly`,, `sendReceive`,.                  |
| rótulo       | String  | O rótulo do fluxo de mídia.                                                                                       |
| Mídia   | String  | O tipo de mídia. O valor possível é `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.        |
| serverMuted | Booliano | Se a mídia estiver com mudo ativado pelo servidor.                                                                          |
| sourceId    | String  | A ID da fonte.                                                                                                |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "serverMuted"
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

## <a name="example"></a>Exemplo

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaStream"
}-->
```json
{
  "direction": "sendReceive",
  "label": "main-audio",
  "mediaType": "audio",
  "serverMuted": false,
  "sourceId": "1024"
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
