---
title: Tipo de recurso ChartTitle
description: Representa um objeto de título de gráfico de um gráfico.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 6cf6a2e6355fc4bc8955899dde48f9cc843e920c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879412"
---
# <a name="charttitle-resource-type"></a>Tipo de recurso ChartTitle

Representa um objeto de título de gráfico de um gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartTitle](../api/charttitle-get.md) | [WorkbookChartTitle](charttitle.md) |Leia as propriedades e os relacionamentos do objeto chartTitle.|
|[Update](../api/charttitle-update.md) | [WorkbookChartTitle](charttitle.md)    |Atualize o objeto ChartTitle. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|overlay|booliano|Valor booliano que determina se o título do gráfico deve se sobrepor ao gráfico ou não.|
|texto|string|Representa o texto do título de um gráfico.|
|visible|booliano|Um valor booliano que representa a visibilidade de um objeto de título de gráfico.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formato|[WorkbookChartTitleFormat](charttitleformat.md)|Representa a formatação de um título do gráfico, que inclui a formatação de fonte e de preenchimento. Somente leitura.|

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
<!-- {
  "type": "#page.annotation",
  "description": "ChartTitle resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
