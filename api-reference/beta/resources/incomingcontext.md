---
title: tipo de recurso incomingContext
description: O contexto associado a uma chamada recebida.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fdbaaadc55877aee89f7ea984d60818cbbad0814
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016556"
---
# <a name="incomingcontext-resource-type"></a>tipo de recurso incomingContext

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O contexto associado a uma chamada recebida.

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                          | Descrição                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| observedParticipantId | String                        | A ID do participante que está sob observação. Somente leitura.         |
| onBehalfOf            | [identitySet](identityset.md) | A identidade em que a chamada está acontecendo em nome de.                   |
| sourceParticipantId   | String                        | A ID do participante que disparou a chamada de entrada. Somente leitura.  |
| transferidar            | [identitySet](identityset.md) | A identidade que transferiu a chamada.                                 |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "observedParticipantId",
    "onBehalfOf",
    "transferor"
  ],
  "@odata.type": "microsoft.graph.incomingContext"
}-->
```json
{
  "observedParticipantId": "String",
  "onBehalfOf": {"@odata.type": "#microsoft.graph.identitySet"},
  "sourceParticipantId": "String",
  "transferor": {"@odata.type": "#microsoft.graph.identitySet"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "incomingContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


