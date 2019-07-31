---
author: daspek
description: O recurso itemActionStat fornece detalhes agregados sobre uma ação em um período de tempo.
ms.date: 09/14/2017
title: ItemActionStat
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 719a443af65fd9642feee3bc8ddbc832eb3964c4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010109"
---
# <a name="itemactionstat-resource-type"></a>tipo de recurso itemActionStat

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **itemActionStat** fornece detalhes agregados sobre uma ação em um período de tempo.

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
