---
title: tipo de recurso timeStamp
description: Informações de data e hora para um ponto no tempo.
localization_priority: Normal
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0629eaabd282f03184be28ade67c2d17d5598602
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808141"
---
# <a name="timestamp-resource-type"></a>tipo de recurso timeStamp

Namespace: microsoft.graph

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
| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|data|Data|A parte de data do carimbo de data/hora.|
|time|TimeOfDay|A parte de tempo do carimbo de data/hora.|
|timeZone|Cadeia de caracteres|A parte de fuso horário do carimbo de data/hora, que é uma das 24 áreas de longitudinal do mundo.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
