---
author: daspek
ms.author: dspektor
title: tipo de recurso itemActionStat
description: O objeto itemActionStat fornece detalhes agregados sobre uma ação em um período de tempo.
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: f1be83bef880b967758a803e694b068df9bfaebf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041264"
---
# <a name="itemactionstat-resource-type"></a>tipo de recurso itemActionStat

Namespace: microsoft.graph

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

