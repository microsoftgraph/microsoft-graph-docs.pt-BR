---
title: tipo de recurso incomingContext
description: Representa o contexto associado a uma chamada de entrada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6acd1928b223789df7580a5f74eefc723570ca93
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962527"
---
# <a name="incomingcontext-resource-type"></a>tipo de recurso incomingContext

Namespace: microsoft.graph

Representa o contexto associado a uma chamada de entrada.

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                          | Descrição                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| sourceParticipantId   | String                        | A ID do participante que disparou a chamada de entrada. Somente leitura.  |
| observedParticipantId | String                        | A ID do participante que está sob observação. Somente leitura.         |
| onBehalfOf            | [identitySet](identityset.md) | A identidade em que a chamada está acontecendo em nome de.                   |
| transferidar            | [identitySet](identityset.md) | A identidade que transferiu a chamada.                                 |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "sourceParticipantId",
    "observedParticipantId",
    "onBehalfOf",
    "transferor"
  ],
  "@odata.type": "microsoft.graph.incomingContext"
}-->
```json
{
  "sourceParticipantId": "String",
  "observedParticipantId": "String",
  "onBehalfOf": {"@odata.type": "#microsoft.graph.identitySet"},
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
