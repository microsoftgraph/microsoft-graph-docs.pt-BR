---
title: Tipo de recurso timeStamp
description: Informações de data e hora para um ponto no tempo.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: sites-and-lists
author: JeremyKelley
ms.openlocfilehash: fb82ddf1e69b8ea06cb425ed5199d1f6c5862b52
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66737102"
---
# <a name="timestamp-resource-type"></a>Tipo de recurso timeStamp

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Informações de data e hora para um ponto no tempo.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|data|Data|A parte de data do carimbo de data/hora.|
|hora|TimeOfDay|A parte de hora do carimbo de data/hora.|
|timeZone|Cadeia de caracteres|A parte de fuso horário do carimbo de data/hora, que é uma das 24 áreas longitudinais do mundo.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.timeStamp"
}-->

```json
{
  "date": "String (timestamp)",
  "time": "String (timestamp)",
  "timeZone": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


