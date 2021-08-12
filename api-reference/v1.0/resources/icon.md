---
title: Tipo de recurso Icon
description: Representa um ícone de célula.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e872bf7bccec06d1ac4fb956a0e8e3b244b5bbc8dc7fe1354c9baea8a0492f20
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54238121"
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

