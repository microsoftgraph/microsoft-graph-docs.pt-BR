---
title: tipo de recurso callRoute
description: Representa o tipo de rota de chamada.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d316c6ba9a7a9d34b34110023019169c39859c79
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962516"
---
# <a name="callroute-resource-type"></a>tipo de recurso callRoute

Namespace: microsoft.graph

Representa o tipo de rota de chamada.

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
