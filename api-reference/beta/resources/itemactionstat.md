---
author: daspek
description: O recurso itemActionStat fornece detalhes agregados sobre uma ação durante um período de tempo.
ms.date: 09/14/2017
title: ItemActionStat
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
ms.openlocfilehash: b1fb726904c3b97ead34162410025a82f410231d
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176298"
---
# <a name="itemactionstat-resource-type"></a>Tipo de recurso itemActionStat

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O **recurso itemActionStat** fornece detalhes agregados sobre uma ação durante um período de tempo.

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.itemActionStat",
}-->

```json
{
  "actionCount": 123,
  "actorCount": 60
}
```

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo  | Descrição
|:------------|:------|:-------------------------------------------------------
| actionCount | Int32 | O número de vezes que a ação ocorreu. Somente leitura.
| actorCount  | Int32 | O número de atores distintos que executaram a ação. Somente leitura.

<!--
{
  "type": "#page.annotation",
  "description": "The ItemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/ItemActionStat",
  "suppressions": []
}
-->


