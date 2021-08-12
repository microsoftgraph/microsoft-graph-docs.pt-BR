---
title: Tipo de recurso ChartDataLabels
description: Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 2ad59daf46d6b6f13c7e95ac206b6525b771b3a39f8aa4612af357ee2e634de8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54252085"
---
# <a name="chartdatalabels-resource-type"></a>Tipo de recurso ChartDataLabels

Namespace: microsoft.graph

Representa uma coleção de todos os rótulos de dados em um ponto do gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartDataLabels](../api/chartdatalabels-get.md) | [WorkbookChartDataLabels](chartdatalabels.md) |Leia as propriedades e os relacionamentos do objeto chartDataLabels.|
|[Update](../api/chartdatalabels-update.md) | [WorkbookChartDataLabels](chartdatalabels.md) |Atualize o objeto ChartDataLabels. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|position|string|Valor de DataLabelPosition que representa a posição do rótulo de dados. Os valores possíveis são: `None` , , , , , , , , , `Center` , , , `InsideEnd` `InsideBase` `OutsideEnd` `Left` `Right` `Top` `Bottom` `BestFit` `Callout` .|
|separator|string|Cadeia de caracteres que representa o separador usado para os rótulos de dados em um gráfico.|
|showBubbleSize|booliano|Valor booliano que determina se o tamanho da bolha do rótulo de dados fica visível ou não.|
|showCategoryName|booliano|Valor booliano que determina se o nome da categoria do rótulo de dados fica visível ou não.|
|showLegendKey|booliano|Valor booliano que determina se o código de legenda do rótulo de dados fica visível ou não.|
|showPercentage|booliano|Valor booliano que determina se o percentual do rótulo de dados fica visível ou não.|
|showSeriesName|booliano|Valor booliano que determina se o nome da série do rótulo de dados fica visível ou não.|
|showValue|booliano|Valor booliano que determina se o valor do rótulo de dados fica visível ou não.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formato|[WorkbookChartDataLabelFormat](chartdatalabelformat.md)|Representa o formato dos rótulos de dados do gráfico, que inclui a formatação de fonte e de preenchimento. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.workbookChartDataLabels"
}-->

```json
{
  "position": "string",
  "separator": "string",
  "showBubbleSize": true,
  "showCategoryName": true,
  "showLegendKey": true,
  "showPercentage": true,
  "showSeriesName": true,
  "showValue": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabels resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

