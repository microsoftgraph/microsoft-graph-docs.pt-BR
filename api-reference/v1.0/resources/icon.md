---
title: Tipo de recurso Icon
description: Representa um ícone de célula.
ms.localizationpriority: medium
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 73ae9bbe240df7bd1e8ca2b6cb7a4a0556fae0f5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098997"
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
|set|string|Representa o conjunto do qual ícone faz parte. Os valores possíveis são: `Invalid` , , , , , , , , , `ThreeArrows` , `ThreeArrowsGray` , , , , `ThreeFlags` , , `ThreeTrafficLights1` `ThreeTrafficLights2` `ThreeSigns` , `ThreeSymbols` `ThreeSymbols2` `FourArrows` `FourArrowsGray` `FourRedToBlack` `FourRating` `FourTrafficLights` `FiveArrows` `FiveArrowsGray` `FiveRating` `FiveQuarters` , `ThreeStars` `ThreeTriangles` `FiveBoxes`|

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

