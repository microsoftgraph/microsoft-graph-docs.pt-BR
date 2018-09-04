# <a name="chart-resource-type"></a>Tipo de recurso Chart

Representa um objeto de gráfico em uma pasta de trabalho.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter Chart](../api/chart_get.md) | [WorkbookChart](chart.md) |Lê as propriedades e os relacionamentos do objeto de gráfico.|
|[Criar ChartSeries](../api/chart_post_series.md) |[WorkbookChartSeries](chartseries.md)| Cria um novo ChartSeries postando na coleção de séries.|
|[Lista de séries](../api/chart_list_series.md) |Coleção [WorkbookChartSeries](chartseries.md)| Obtém uma coleção de objetos ChartSeries.|
|[Atualizar](../api/chart_update.md) | [WorkbookChart](chart.md)   |Atualiza um objeto Chart. |
|[Imagem](../api/chart_image.md)|Sequência de caracteres de imagem codificada em base64|Processa o gráfico como uma imagem codificada em base64, dimensionando o gráfico para se ajustar às dimensões especificadas.|
|[Excluir](../api/chart_delete.md)|Nenhum|Exclui o objeto de gráfico.|
|[SetData](../api/chart_setdata.md)|Nenhum|Redefine os dados de origem do gráfico.|
|[Setposition](../api/chart_setposition.md)|Nenhum|Posiciona o gráfico em relação às células na planilha.|
|[Lista](../api/chart_list.md) | Coleção [WorkbookChart](chart.md) |Obtém a coleção de objetos do gráfico. |
|[Itemat](../api/chartcollection_itemat.md)|[WorkbookChart](chart.md)|Obtém um gráfico com base em sua posição na coleção.|
|[Adicionar](../api/chartcollection_add.md)|[WorkbookChart](chart.md)|Cria um novo gráfico.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|altura|Double|Representa a altura, em pontos, do objeto Chart.|
|id|sequência de caracteres|Obtém um gráfico com base em sua posição no conjunto. Somente leitura.|
|esquerda|Double|A distância, em pontos, da esquerda do gráfico à origem da planilha.|
|nome|sequência de caracteres|Representa o nome de um objeto Chart.|
|superior|Double|Representa a distância, em pontos, da borda superior do objeto à parte superior da primeira linha de uma planilha ou da área de um gráfico.|
|largura|Double|Representa a largura, em pontos, do objeto de gráfico.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|eixos|[WorkbookChartAxes](chartaxes.md)|Representa os eixos de um gráfico. Somente leitura.|
|dataLabels|[WorkbookChartDataLabels](chartdatalabels.md)|Representa os rótulos de dados no gráfico. Somente leitura.|
|formato|[WorkbookChartAreaFormat](chartareaformat.md)|Encapsula as propriedades de formato da área do gráfico. Somente leitura.|
|legenda|[WorkbookChartLegend](chartlegend.md)|Representa a legenda do gráfico. Somente leitura.|
|série|Coleção [WorkbookChartSeries](chartseries.md)|Representa uma única série ou uma coleção de séries no gráfico. Somente leitura.|
|título|[WorkbookChartTitle](charttitle.md)|Representa o título do gráfico especificado, incluindo o texto, a visibilidade, a posição e a formatação. Somente leitura.|
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