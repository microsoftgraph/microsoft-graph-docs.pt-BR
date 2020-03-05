---
title: tipo de recurso timerange
description: Um recurso de intervalo de tempo com um horário de início e de término.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e9edfd06ecd65d7e08d6701d1fc885dce9067689
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519705"
---
# <a name="timerange-resource-type"></a>tipo de recurso timerange

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um recurso de intervalo de tempo com um horário de início e de término.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|endTime|TimeOfDay|Hora de término do intervalo de tempo.|
|startTime|TimeOfDay|Hora de início do intervalo de tempo.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeRange",
  "baseType": null
}-->

```json
{
  "endTime": "String (timestamp)",
  "startTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeRange resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->