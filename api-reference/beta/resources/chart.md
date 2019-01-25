---
title: Tipo de recurso Chart
description: Representa um objeto de gráfico em uma pasta de trabalho.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 4bc0ad0d31981e7e84241519e92569ab25c2cf18
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529520"
---
# <a name="chart-resource-type"></a>Tipo de recurso Chart

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um objeto de gráfico em uma pasta de trabalho.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|Get Chart | [Chart](chart.md) |Leia as propriedades e os relacionamentos do objeto de gráfico.|
|Create ChartSeries |ChartSeries| Crie uma nova ChartSeries postando na coleção de séries.|
|List series |Coleção ChartSeries| Obtenha uma coleção de objetos ChartSeries.|
|[Update](../api/chart-update.md) | [Chart](chart.md)   |Atualize um objeto Chart. |
|[Image](../api/chart-image.md)|Cadeia de caracteres de imagem codificada em base64|Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.|
|[Delete](../api/chart-delete.md)|Nenhum|Exclui o objeto de gráfico.|
|[SetData](../api/chart-setdata.md)|Nenhum|Redefine os dados de origem do gráfico.|
|[Setposition](../api/chart-setposition.md)|Nenhum|Posiciona o gráfico em relação às células na planilha.|
|[List](../api/chart-list.md) | Coleção Chart |Obtenha a coleção de objetos do gráfico. |
|[Itemat](../api/chartcollection-itemat.md)|[Chart](chart.md)|Obtém um gráfico com base em sua posição na coleção.|
|[Add](../api/chartcollection-add.md)|[Chart](chart.md)|Cria um novo gráfico.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|height|double|Representa a altura, em pontos, do objeto Chart.|
|id|string|Obtém um gráfico com base em sua posição no conjunto. Somente leitura.|
|left|double|A distância, em pontos, da esquerda do gráfico à origem da planilha.|
|name|string|Representa o nome de um objeto Chart.|
|top|double|Representa a distância, em pontos, da borda superior do objeto à parte superior da primeira linha de uma planilha ou da área de um gráfico.|
|width|Double|Representa a largura, em pontos, do objeto de gráfico.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|axes|[ChartAxes](chartaxes.md)|Representa os eixos de um gráfico. Somente leitura.|
|dataLabels|[ChartDataLabels](chartdatalabels.md)|Representa os rótulos de dados no gráfico. Somente leitura.|
|formato|[ChartAreaFormat](chartareaformat.md)|Encapsula as propriedades de formato da área do gráfico. Somente leitura.|
|legend|[ChartLegend](chartlegend.md)|Representa a legenda do gráfico. Somente leitura.|
|series|Coleção [ChartSeries](chartseries.md)|Representa uma única série ou uma coleção de séries no gráfico. Somente leitura.|
|title|[ChartTitle](charttitle.md)|Representa o título do gráfico especificado, incluindo o texto, a visibilidade, a posição e a formatação. Somente leitura.|
|planilha|[Worksheet](worksheet.md)|A planilha que contém o gráfico atual. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chart"
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
<!--
{
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chart.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
