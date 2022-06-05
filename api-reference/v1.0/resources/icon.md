---
title: Tipo de recurso Icon
description: Representa um ícone de célula.
ms.localizationpriority: medium
author: ruoyingl
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: cc8a3ff251a321d6accc89015ba9b0ec751ed0ed
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899705"
---
# <a name="icon-resource-type"></a>Tipo de recurso Icon

Namespace: microsoft.graph

Representa um ícone de célula.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get Icon](../api/icon-get.md) | [Icon](icon.md) |Leia as propriedades e os relacionamentos do objeto de ícone.|
|[Update](../api/icon-update.md) | [Icon](icon.md)  |Atualize o objeto Icon. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|index|int|Representa o índice do ícone em determinado conjunto.|
|set|string|Representa o conjunto do qual ícone faz parte. Os valores possíveis são: , , , , , `ThreeTrafficLights1`, `ThreeSymbols``ThreeSigns``ThreeTrafficLights2`, `ThreeSymbols2`, `FourArrows`, , `FourArrowsGray`, `FourRating``FourRedToBlack`, , `FourTrafficLights`, , `FiveArrows``FiveArrowsGray`, , `FiveRating`, , , `FiveBoxes``ThreeTriangles``ThreeStars``FiveQuarters``ThreeFlags``ThreeArrowsGray``ThreeArrows``Invalid`|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookIcon"
}-->

```json
{
  "index": 1024,
  "set": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

