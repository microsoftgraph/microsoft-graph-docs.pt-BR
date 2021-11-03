---
title: Tipo de recurso timeStamp
description: Informações de data e hora para um ponto no tempo.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: JeremyKelley
ms.openlocfilehash: ff93ab9a55a695818ec21f60afb039c6542efd0a
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695794"
---
# <a name="timestamp-resource-type"></a>Tipo de recurso timeStamp

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Informações de data e hora para um ponto no tempo.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|data|Data|A parte de data do data do data/hora.|
|hora|TimeOfDay|A parte de tempo do timestamp.|
|timeZone|Cadeia de caracteres|A parte do timezone do timestamp, que é uma das 24 áreas longitudinais do mundo.|

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


