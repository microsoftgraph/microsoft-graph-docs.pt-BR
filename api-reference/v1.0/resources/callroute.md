---
title: Tipo de recurso callRoute
description: Representa o tipo de rota de chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 82d69edb17d1a68ab3fc0f22402bd26c94c02dd3f922f0eb091cce95ce0b921f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141816"
---
# <a name="callroute-resource-type"></a>Tipo de recurso callRoute

Namespace: microsoft.graph

Representa o tipo de rota de chamada.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo                          | Descrição                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| final               | [identitySet](identityset.md) | A identidade que foi resolvida na chamada.               |
| Original            | [identitySet](identityset.md) | A identidade que foi originalmente usada na chamada.           |
| routingType         | Cadeia de caracteres                        | Os valores possíveis são: `forwarded`, `lookup`, `selfFork`.  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

