---
author: daspek
title: Tipo de recurso itemActionStat
description: O objeto itemActionStat fornece detalhes agregados sobre uma ação durante um período de tempo.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 13bc306a1b14d7d59ec8eddda5b02a5cba84e649
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50238523"
---
# <a name="itemactionstat-resource-type"></a>Tipo de recurso itemActionStat

Namespace: microsoft.graph

O **recurso itemActionStat** fornece detalhes agregados sobre uma ação durante um período de tempo.

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo  | Descrição
|:------------|:------|:-------------------------------------------------------
| actionCount | Int32 | O número de vezes que a ação ocorreu. Somente leitura.
| actorCount  | Int32 | O número de atores distintos que realizaram a ação. Somente leitura.

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

