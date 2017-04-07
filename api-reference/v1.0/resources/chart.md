# <a name="chart-resource-type"></a>Tipo de recurso Chart

Representa um objeto de gráfico em uma pasta de trabalho.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get Chart](../api/chart_get.md) | [Chart](chart.md) |Leia as propriedades e os relacionamentos do objeto de gráfico.|
|[Create ChartSeries](../api/chart_post_series.md) |[ChartSeries](chartseries.md)| Crie uma nova ChartSeries postando na coleção de séries.|
|[List series](../api/chart_list_series.md) |Coleção [ChartSeries](chartseries.md)| Obtenha uma coleção de objetos ChartSeries.|
|[Update](../api/chart_update.md) | [Chart](chart.md)    |Atualize um objeto Chart. |
|[Image](../api/chart_image.md)|Cadeia de caracteres de imagem codificada em base64|Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.|
|[Delete](../api/chart_delete.md)|Nenhum|Exclui o objeto de gráfico.|
|[SetData](../api/chart_setdata.md)|Nenhum|Redefine os dados de origem do gráfico.|
|[Setposition](../api/chart_setposition.md)|Nenhum|Posiciona o gráfico em relação às células na planilha.|
|[List](../api/chart_list.md) | Coleção [Chart](chart.md) |Obtenha a coleção de objetos do gráfico. |
|[Itemat](../api/chartcollection_itemat.md)|[Chart](chart.md)|Obtém um gráfico com base em sua posição na coleção.|
|[Add](../api/chartcollection_add.md)|[Chart](chart.md)|Cria um novo gráfico.|

## <a name="properties"></a>Propriedades
| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|height|Double|Representa a altura, em pontos, do objeto Chart.|
|id|string|Obtém um gráfico com base em sua posição no conjunto. Somente leitura.|
|left|Double|A distância, em pontos, da esquerda do gráfico à origem da planilha.|
|name|string|Representa o nome de um objeto Chart.|
|top|Double|Representa a distância, em pontos, da borda superior do objeto à parte superior da primeira linha de uma planilha ou da área de um gráfico.|
|width|Double|Representa a largura, em pontos, do objeto de gráfico.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|axes|[ChartAxes](chartaxes.md)|Representa os eixos de um gráfico. Somente leitura.|
|dataLabels|[ChartDataLabels](chartdatalabels.md)|Representa os rótulos de dados no gráfico. Somente leitura.|
|format|[ChartAreaFormat](chartareaformat.md)|Encapsula as propriedades de formato da área do gráfico. Somente leitura.|
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
<!-- {
  "type": "#page.annotation",
  "description": "Chart resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->