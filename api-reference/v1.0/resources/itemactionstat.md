---
author: daspek
title: Tipo de recurso itemActionStat
description: O objeto itemActionStat fornece detalhes agregados sobre uma ação por um período de tempo.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 595a479f98e6327f3e43c2278c646d6e570e5a290cdcae8b7151ac4162d15578
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246672"
---
# <a name="itemactionstat-resource-type"></a>Tipo de recurso itemActionStat

Namespace: microsoft.graph

O **recurso itemActionStat** fornece detalhes agregados sobre uma ação por um período de tempo.

## <a name="properties"></a>Propriedades

| Propriedade    | Tipo  | Descrição
|:------------|:------|:-------------------------------------------------------
| actionCount | Int32 | O número de vezes que a ação ocorreu. Apenas leitura.
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

