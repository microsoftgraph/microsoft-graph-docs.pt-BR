---
title: tipo de recurso recordingInfo
description: Representa informações de gravação de um participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b7044f13f16a9d1126a5b1c72cdc86c3527f6b37
ms.sourcegitcommit: d14e2abb24d9fbab519458b1c9fec890a5e51d70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2020
ms.locfileid: "43543265"
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
  "initiator": {"@odata.type": "#microsoft.graph.identitySet"},
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
