---
title: tipo de recurso de mediaStream
description: O tipo de mediaStream.
ms.openlocfilehash: 28eb98a3ab1be67c60c6ebd35deb7618f1618be3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040722"
---
# <a name="mediastream-resource-type"></a>tipo de recurso de mediaStream

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O tipo de mediaStream.

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo    | Descrição                                                                                                   |
| :---------- | :------ | :------------------------------------------------------------------------------------------------------------ |
| direção   | String  | A direção. Os valores possíveis são `inactive`, `sendOnly`, `receiveOnly`, `sendReceive`.                  |
| rótulo       | String  | O rótulo de fluxo de mídia.                                                                                       |
| mediaType   | String  | O tipo de mídia. Os valores possíveis são `unknown`, `audio`, `video`, `videoBasedScreenSharing`, `data`.        |
| serverMuted | Booliano | Se a mídia está sem som pelo servidor.                                                                          |
| sourceId    | String  | A ID de origem.                                                                                                |

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
<!-- {
  "type": "#page.annotation",
  "description": "mediaStream resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
