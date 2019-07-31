---
title: tipo de recurso callRoute
description: O tipo callRoute.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9978bffd55f62f0646f84d2405df70eba6232d68
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974050"
---
# <a name="callroute-resource-type"></a>tipo de recurso callRoute

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo callRoute.

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo                          | Descrição                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| recente               | [identitySet](identityset.md) | A identidade que foi resolvida para na chamada.               |
| Original            | [identitySet](identityset.md) | A identidade que foi usada originalmente na chamada.           |
| RoutingType         | String                        | Os valores possíveis são: `forwarded`, `lookup`, `selfFork`.  |

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
