---
title: tipo de recurso recordingInfo
description: Representa informações de gravação de um participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6a41195705a46ac46bd085f3b4a655943b730ad3
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962526"
---
# <a name="recordinginfo-resource-type"></a>tipo de recurso recordingInfo

Namespace: microsoft.graph

Representa informações de gravação de um participante.

## <a name="properties"></a>Propriedades

| Propriedade        | Tipo    | Descrição|
|:----------------|:--------|:----------|
| Iniciador     | [identitySet](identitySet.md) | As identidades do iniciador de gravação. |
| recordingStatus | String | Os valores possíveis são `unknown`: `notRecording`, `recording`,, `failed`ou. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "initiator"
  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "recordingStatus": "unknown | notRecording | recording | failed"
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
