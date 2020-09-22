---
title: tipo de recurso recordingInfo
description: Informações de gravação de um participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 45d844329688e663c27ef5ecdf94282312baa53d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055169"
---
# <a name="recordinginfo-resource-type"></a>tipo de recurso recordingInfo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Informações de gravação de um participante.

## <a name="properties"></a>Propriedades

| Propriedade        | Tipo    | Descrição|
|:----------------|:--------|:----------|
| initiatedBy     | [participantInfo](participantinfo.md) | O participante que iniciou a gravação. |
| recordingStatus | Cadeia de caracteres | Os valores possíveis são: `unknown` , `notRecording` , `recording` , ou `failed` . |
| Iniciador | [identitySet](identitySet.md) | As identidades do iniciador de gravação. |

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
  "recordingStatus": "unknown | notRecording | recording | failed",
  "initiator": {"@odata.type": "#microsoft.graph.initiator"}
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


