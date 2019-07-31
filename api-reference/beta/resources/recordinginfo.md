---
title: tipo de recurso recordingInfo
description: Informações de gravação de um participante.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ebb9e7d6a5c62b12073d6fa26e76147eb0cbb137
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965478"
---
# <a name="recordinginfo-resource-type"></a>tipo de recurso recordingInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Informações de gravação de um participante.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo    | Descrição|
|:---------------|:--------|:----------|
| initiatedBy | [participantInfo](participantinfo.md) | O participante que iniciou a gravação. |
| status | String | Os valores possíveis são: `recordingCapable`, `notRecording`, `startedRecording`. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "status": "recordingCapable | notRecording | startedRecording"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
