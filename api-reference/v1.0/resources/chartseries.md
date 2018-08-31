# <a name="chartseries-resource-type"></a>Tipo de recurso ChartSeries

Representa uma série em um gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter ChartSeries](../api/chartseries_get.md) | [WorkbookChartSeries](chartseries.md) |Leia as propriedades e as relações do objeto chartSeries.|
|[Criar ChartPoints](../api/chartseries_post_points.md) |[ChartPoints](chartpoint.md)| Crie um novo ChartPoints postando na coleção de pontos.|
|[Listar pontos](../api/chartseries_list_points.md) |Coleção [ChartPoints](chartpoint.md)| Obtenha uma coleção de objetos ChartPoints.|
|[Atualizar](../api/chartseries_update.md) | [WorkbookChartSeries](chartseries.md) |Atualize o objeto ChartSeries. |
|[Lista](../api/chartseries_list.md) | Coleção [WorkbookChartSeries](chartseries.md) |Obtenha uma coleção de objetos chartSeries. |
|[ItemAt](../api/chartseriescollection_itemat.md)|[WorkbookChartSeries](chartseries.md)|Recupera uma série com base em sua posição na coleção|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|name|sequência de caracteres|Representa o nome de uma série em um gráfico.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|format|[WorkbookChartSeriesFormat](chartseriesformat.md)|Representa a formatação de uma série do gráfico, que inclui a formatação de linha e de preenchimento. Somente leitura.|
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