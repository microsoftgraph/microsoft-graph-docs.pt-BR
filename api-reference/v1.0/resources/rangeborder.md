---
title: Tipo de recurso RangeBorder
description: Representa a borda de um objeto.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: ad8cbd941b1af5a3a694be308ea2b5c0065a5e05b2f58b02c98c5e8d7bc26398
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246616"
---
# <a name="rangeborder-resource-type"></a>Tipo de recurso RangeBorder

Namespace: microsoft.graph

Representa a borda de um objeto.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get RangeBorder](../api/rangeborder-get.md) | [WorkbookRangeBorder](rangeborder.md) |Leia as propriedades e relacionamentos do objeto rangeBorder.|
|[Update](../api/rangeborder-update.md) | [WorkbookRangeBorder](rangeborder.md) |Atualize o objeto RangeBorder. |
|[List](../api/rangeborder-list.md) | [Coleção WorkbookRangeBorder](rangeborder.md) |Obtenha a coleção de objetos rangeBorder. |
|[Itemat](../api/rangebordercollection-itemat.md)|[WorkbookRangeBorder](rangeborder.md)|Obtém um objeto de borda usando seu índice.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|color|string|Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").|
|id|string|Representa o identificador da borda. Os valores possíveis são: `EdgeTop` , , , , , , , , `EdgeBottom` `EdgeLeft` `EdgeRight` `InsideVertical` `InsideHorizontal` `DiagonalDown` `DiagonalUp` . Somente leitura.|
|sideIndex|string|Valor constante que indica o lado específico da borda. Os valores possíveis são: `EdgeTop` , , , , , , , , `EdgeBottom` `EdgeLeft` `EdgeRight` `InsideVertical` `InsideHorizontal` `DiagonalDown` `DiagonalUp` . Somente leitura.|
|style|cadeia de caracteres|Uma das constantes de estilo de linha especificando o estilo de linha da borda. Os valores possíveis são: `None` , , , , , , , , `Continuous` `Dash` `DashDot` `DashDotDot` `Dot` `Double` `SlantDashDot` .|
|weight|string|Especifica a espessura da borda em torno de um intervalo. Os valores possíveis são: `Hairline`, `Thin`, `Medium`, `Thick`.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

