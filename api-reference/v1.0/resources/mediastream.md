---
title: tipo de recurso mediaStream
description: O tipo mediaStream.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d1158dfb01b9e92c5dc97f34bef3bb3661da51b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48088486"
---
# <a name="mediastream-resource-type"></a>tipo de recurso mediaStream

Namespace: microsoft.graph

Contém informações sobre o canal de mídia.

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo    | Descrição                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| direction   | String  | A direção. Os valores possíveis são:,,, `inactive` `sendOnly` `receiveOnly` `sendReceive` .                  |
| rótulo       | Cadeia de caracteres  | O rótulo do fluxo de mídia.                                                                                       |
| mediaType   | Cadeia de caracteres  | O tipo de mídia. O valor possível é `unknown` , `audio` , `video` , `videoBasedScreenSharing` , `data` .        |
| serverMuted | Booliano | Se a mídia estiver com mudo ativado pelo servidor.                                                                          |
| sourceId    | Cadeia de caracteres  | A ID da fonte.                                                                                                |

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

