---
title: Tipo de recurso outlookGeoCoordinates
description: As coordenadas geográficas, a elevação e o grau de precisão delas para um local físico.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1926d398a07bb38f27f46b8886ba7454321d5796
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447266"
---
# <a name="outlookgeocoordinates-resource-type"></a>Tipo de recurso outlookGeoCoordinates

Namespace: Microsoft. Graph

As coordenadas geográficas, a elevação e o grau de precisão delas para um local físico.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.outlookGeoCoordinates"
}-->

```json
{
  "accuracy": 1024.13,
  "altitude": 1024.13,
  "altitudeAccuracy": 1024.13,
  "latitude": 1024.13,
  "longitude": 1024.13
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|accuracy|double|A precisão da latitude e da longitude. Por exemplo, a precisão pode ser medida em metros, como a precisão da latitude e da longitude em um raio de 50 metros.|
|altitude|double|A altitude do local.|
|altitudeAccuracy|double|A precisão da altitude.|
|latitude|double|A latitude do local.|
|longitude|double|A longitude do local.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "outlookGeoCoordinates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
