---
title: Tipo de recurso incomingContext
description: Representa o contexto associado a uma chamada de entrada.
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 80f300fc4f3cf051466b37c4445272444fdc71bc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123353"
---
# <a name="incomingcontext-resource-type"></a>Tipo de recurso incomingContext

Namespace: microsoft.graph

Representa o contexto associado a uma chamada de entrada.

## <a name="properties"></a>Propriedades

| Propriedade              | Tipo                          | Descrição                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| sourceParticipantId   | Cadeia de caracteres                        | A ID do participante que disparou a chamada de entrada. Somente leitura.  |
| observedParticipantId | String                        | A ID do participante que está em observação. Somente leitura.         |
| onBehalfOf            | [identitySet](identityset.md) | A identidade de que a chamada está acontecendo em nome.                   |
| transferor            | [identitySet](identityset.md) | A identidade que transferiu a chamada.                                 |

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

