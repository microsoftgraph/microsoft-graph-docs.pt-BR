---
title: tipo de recurso workbookChartTitle
description: Representa um objeto ChartTitle de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 8c102ea62b29cba017793dcaf135853121fc4bd4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007148"
---
# <a name="workbookcharttitle-resource-type"></a>tipo de recurso workbookChartTitle

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um objeto ChartTitle de um gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter workbookChartTitle](../api/charttitle-get.md) | [workbookChartTitle](workbookcharttitle.md) |Leia as propriedades e os relacionamentos do objeto chartTitle.|
|[Update](../api/charttitle-update.md) | [workbookChartTitle](workbookcharttitle.md)    |Atualize o objeto ChartTitle. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|overlay|booliano|Valor booliano que determina se o título do gráfico deve se sobrepor ao gráfico ou não.|
|texto|string|Representa o texto do título de um gráfico.|
|visible|booliano|Um valor booliano que representa a visibilidade de um objeto de título de gráfico.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formato|[workbookChartTitleFormat](workbookcharttitleformat.md)|Representa a formatação de um título do gráfico, que inclui a formatação de fonte e de preenchimento. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartTitle"
}-->

```json
{
  "overlay": true,
  "text": "string",
  "visible": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
