---
title: Tipo de recurso SortField
description: Representa uma condição em uma operação de classificação.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 914ddf41da1b1f64e0e4e006d947790829b69be768a9f2b1863ba45789b45398
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180471"
---
# <a name="sortfield-resource-type"></a>Tipo de recurso SortField

Namespace: microsoft.graph

Representa uma condição em uma operação de classificação.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|ascending|booliano|Indica se a classificação é feita de forma crescente.|
|color|cadeia de caracteres|Representa a cor que é o destino da condição se a classificação estiver na cor da fonte ou da célula.|
|dataOption|string|Representa as opções de classificação adicionais para esse campo. Os valores possíveis são: `Normal` , `TextAsNumber` .|
|key|int|Representa a coluna (ou linha, dependendo da orientação da classificação) em que a condição está. Representado como um deslocamento da primeira coluna (ou linha).|
|sortOn|string|Representa o tipo de classificação dessa condição. Os valores possíveis são: `Value`, `CellColor`, `FontColor`, `Icon`.|
|ícone|[WorkbookIcon](icon.md)|Representa o ícone que é o destino da condição se a classificação está no ícone da célula.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookSortField"
}-->

```json
{
  "ascending": true,
  "color": "string",
  "dataOption": "string",
  "key": 1024,
  "sortOn": "string",
  "icon": { "@odata.type": "microsoft.graph.workbookIcon" }
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "SortField resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

