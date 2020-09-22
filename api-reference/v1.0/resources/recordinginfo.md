---
title: tipo de recurso recordingInfo
description: Representa informações de gravação de um participante.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: dd640e3ddef6b88f17449c31611ad6bd956ca0b8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078973"
---
# <a name="recordinginfo-resource-type"></a>tipo de recurso recordingInfo

Namespace: microsoft.graph

Representa informações de gravação de um participante.

## <a name="properties"></a>Propriedades

| Propriedade        | Tipo    | Descrição|
|:----------------|:--------|:----------|
| Iniciador     | [identitySet](identitySet.md) | As identidades do iniciador de gravação. |
| recordingStatus | Cadeia de caracteres | Os valores possíveis são: `unknown` , `notRecording` , `recording` , ou `failed` . |

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

