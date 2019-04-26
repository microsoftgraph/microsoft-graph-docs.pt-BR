---
title: tipo de recurso timeStamp
description: Informações de data e hora para um ponto no tempo.
localization_priority: Normal
ms.openlocfilehash: 5f96ad5c557bda93ef74787d9d909fce112cfb15
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341950"
---
# <a name="timestamp-resource-type"></a>tipo de recurso timeStamp

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Informações de data e hora para um ponto no tempo.

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
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|data|Data|A parte de data do carimbo de data/hora.|
|time|TimeOfDay|A parte de tempo do carimbo de data/hora.|
|timeZone|Cadeia de caracteres|A parte de fuso horário do carimbo de data/hora, que é uma das 24 áreas de longitudinal do mundo.|

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
