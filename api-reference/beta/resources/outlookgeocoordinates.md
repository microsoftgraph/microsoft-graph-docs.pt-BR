---
title: Tipo de recurso outlookGeoCoordinates
description: As coordenadas geográficas, a elevação e o grau de precisão delas para um local físico.
localization_priority: Normal
ms.openlocfilehash: 2522410cd55705411084945b0519738871dedaa0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845357"
---
# <a name="outlookgeocoordinates-resource-type"></a>Tipo de recurso outlookGeoCoordinates

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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
