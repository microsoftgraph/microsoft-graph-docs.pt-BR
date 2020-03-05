---
author: daspek
ms.author: dspektor
title: tipo de recurso itemActionStat
description: O objeto itemActionStat fornece detalhes agregados sobre uma ação em um período de tempo.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 4207c85185281ec9944aa08dfce088739116bb8e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447679"
---
# <a name="itemactionstat-resource-type"></a>tipo de recurso itemActionStat

Namespace: Microsoft. Graph

O recurso **itemActionStat** fornece detalhes agregados sobre uma ação em um período de tempo.

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo  | Descrição
|:------------|:------|:-------------------------------------------------------
| actionCount | Int32 | O número de vezes que a ação ocorreu. Somente leitura.
| actorCount  | Int32 | O número de atores distintos que executaram a ação. Somente leitura.

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

<!--
{
  "type": "#page.annotation",
  "description": "The itemActionStat object provides aggregate details about an action over a period of time.",
  "keywords": "activities,activity,action,analytics",
  "section": "documentation",
  "tocPath": "Resources/itemActionStat",
  "suppressions": []
}
-->
