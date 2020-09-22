---
title: Tipo de recurso ChartSeries
description: Representa uma série de um gráfico.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 173f9878daecd3443137800f143a2b3633a2fa20
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988370"
---
# <a name="chartseries-resource-type"></a>Tipo de recurso ChartSeries

Namespace: microsoft.graph

Representa uma série de um gráfico.


## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartSeries](../api/chartseries-get.md) | [WorkbookChartSeries](chartseries.md) |Leia as propriedades e os relacionamentos do objeto chartSeries.|
|[Create ChartPoints](../api/chartseries-post-points.md) |[ChartPoints](chartpoint.md)| Crie um novo ChartPoints postando na coleção de pontos.|
|[List points](../api/chartseries-list-points.md) |Coleção [ChartPoints](chartpoint.md)| Obtenha uma coleção de objetos ChartPoints.|
|[Update](../api/chartseries-update.md) | [WorkbookChartSeries](chartseries.md) |Atualize o objeto ChartSeries. |
|[List](../api/chartseries-list.md) | Coleção [WorkbookChartSeries](chartseries.md) |Obtenha uma coleção de objetos chartSeries. |
|[ItemAt](../api/chartseriescollection-itemat.md)|[WorkbookChartSeries](chartseries.md)|Recupera uma série com base na respectiva posição na coleção|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|nome|string|Representa o nome de uma série do gráfico.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formato|[WorkbookChartSeriesFormat](chartseriesformat.md)|Representa a formatação de uma série do gráfico, que inclui a formatação de linha e de preenchimento. Somente leitura.|
|points|Coleção [WorkbookChartPoint](chartpoint.md)|Representa uma coleção de todos os pontos da série. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookChartSeries"
}-->

```json
{
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartSeries resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

