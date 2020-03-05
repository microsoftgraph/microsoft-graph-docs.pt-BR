---
title: tipo de recurso workbookIcon
description: Representa um ícone de célula.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ''
ms.openlocfilehash: 6c2cbbe26c3c1440afa8a0954bac5d0d38feea29
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519215"
---
# <a name="workbookicon-resource-type"></a>tipo de recurso workbookIcon

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um ícone de célula.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get Icon](../api/icon-get.md) | [workbookIcon](workbookicon.md) |Leia as propriedades e os relacionamentos do objeto de ícone.|
|[Update](../api/icon-update.md) | [workbookIcon](workbookicon.md)  |Atualize o objeto Icon. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|index|int|Representa o índice do ícone em determinado conjunto.|
|set|string|Representa o conjunto do qual o ícone faz parte. Os valores possíveis são: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles` e `FiveBoxes`.|

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
<!--
{
  "type": "#page.annotation",
  "description": "Icon resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
