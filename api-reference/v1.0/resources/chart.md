---
title: Tipo de recurso Chart
description: Representa um objeto chart em uma pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 160fcb95fd8ffe4b4d0c2d4e9233afe3492ef32d27b910ee40bb7519b20e591a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54121414"
---
# <a name="chart-resource-type"></a>Tipo de recurso Chart

Namespace: microsoft.graph

Representa um objeto chart em uma pasta de trabalho.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get Chart](../api/chart-get.md) | [WorkbookChart](chart.md) |Leia as propriedades e os relacionamentos do objeto de gráfico.|
|[Create ChartSeries](../api/chart-post-series.md) |[WorkbookChartSeries](chartseries.md)| Crie uma nova ChartSeries postando na coleção de séries.|
|[List series](../api/chart-list-series.md) |[Coleção WorkbookChartSeries](chartseries.md)| Obtenha uma coleção de objetos ChartSeries.|
|[Update](../api/chart-update.md) | [WorkbookChart](chart.md)   |Atualize um objeto Chart. |
|[Image](../api/chart-image.md)|Cadeia de caracteres de imagem codificada em base64|Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.|
|[Delete](../api/chart-delete.md)|None|Exclui o objeto de gráfico.|
|[SetData](../api/chart-setdata.md)|Nenhum|Redefine os dados de origem do gráfico.|
|[Setposition](../api/chart-setposition.md)|Nenhum|Posiciona o gráfico em relação às células na planilha.|
|[List](../api/chart-list.md) | Conjunto [WorkbookChart](chart.md)  |Obtenha a coleção de objetos do gráfico. |
|[Itemat](../api/chartcollection-itemat.md)|[WorkbookChart](chart.md)|Obtém um gráfico com base em sua posição na coleção.|
|[Add](../api/chartcollection-add.md)|[WorkbookChart](chart.md)|Cria um novo gráfico.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|height|Double|Representa a altura, em pontos, do objeto Chart.|
|id|string|Obtém um gráfico com base em sua posição no conjunto. Somente leitura.|
|left|Double|A distância, em pontos, da esquerda do gráfico à origem da planilha.|
|nome|string|Representa o nome de um objeto Chart.|
|top|Double|Representa a distância, em pontos, da borda superior do objeto à parte superior da primeira linha de uma planilha ou da área de um gráfico.|
|width|Double|Representa a largura, em pontos, do objeto de gráfico.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|axes|[WorkbookChartAxes](chartaxes.md)|Representa os eixos de um gráfico. Somente leitura.|
|dataLabels|[WorkbookChartDataLabels](chartdatalabels.md)|Representa os rótulos de dados no gráfico. Somente leitura.|
|format|[WorkbookChartAreaFormat](chartareaformat.md)|Encapsula as propriedades de formato da área do gráfico. Somente leitura.|
|legend|[WorkbookChartLegend](chartlegend.md)|Representa a legenda do gráfico. Somente leitura.|
|series|[Coleção WorkbookChartSeries](chartseries.md)|Representa uma única série ou uma coleção de séries no gráfico. Somente leitura.|
|title|[WorkbookChartTitle](charttitle.md)|Representa o título do gráfico especificado, incluindo o texto, a visibilidade, a posição e a formatação. Somente leitura.|
|planilha|[WorkbookWorksheet](worksheet.md)|A planilha que contém o gráfico atual. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChart"
}-->

```json
{
  "height": 1024,
  "id": "string",
  "left": 1024,
  "name": "string",
  "top": 1024,
  "width": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

