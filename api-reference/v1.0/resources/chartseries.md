# <a name="chartseries-resource-type"></a>Tipo de recurso ChartSeries

Representa uma série em um gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartSeries](../api/chartseries_get.md) | [ChartSeries](chartseries.md) |Leia as propriedades e os relacionamentos do objeto chartSeries.|
|[Create ChartPoints](../api/chartseries_post_points.md) |[ChartPoints](chartpoint.md)| Crie um novo ChartPoints postando na coleção de pontos.|
|[List points](../api/chartseries_list_points.md) |Coleção [ChartPoints](chartpoint.md)| Obtenha uma coleção de objetos ChartPoints.|
|[Update](../api/chartseries_update.md) | [ChartSeries](chartseries.md)    |Atualize o objeto ChartSeries. |
|[List](../api/chartseries_list.md) | Coleção [ChartSeries](chartseries.md) |Obtenha uma coleção de objetos chartSeries. |
|[Itemat](../api/chartseriescollection_itemat.md)|[ChartSeries](chartseries.md)|Recupera uma série com base na respectiva posição na coleção.|

## <a name="properties"></a>Propriedades
| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|name|string|Representa o nome de uma série em um gráfico.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|formato|[ChartSeriesFormat](chartseriesformat.md)|Representa a formatação de uma série do gráfico, que inclui a formatação de linha e de preenchimento. Somente leitura.|
|points|Coleção [ChartPoints](chartpoint.md)|Representa uma coleção de todos os pontos da série. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartSeries"
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