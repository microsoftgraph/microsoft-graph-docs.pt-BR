---
title: Tipo de recurso timeStamp
description: Informações de data e hora para um ponto no tempo.
ms.localizationpriority: medium
author: JeremyKelley
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f284439f63d15c1cf6d070894a8f9f9074f69e24
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59093985"
---
# <a name="timestamp-resource-type"></a>Tipo de recurso timeStamp

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
|data|Data|A parte de data do data do data/hora.|
|hora|TimeOfDay|A parte de tempo do timestamp.|
|timeZone|Cadeia de caracteres|A parte do timezone do timestamp, que é uma das 24 áreas longitudinais do mundo.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeStamp resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

