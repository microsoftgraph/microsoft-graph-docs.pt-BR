# <a name="chartpoint-resource-type"></a>Tipo de recurso ChartPoint

Representa um ponto de uma série do gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartPoint](../api/chartpoint_get.md) | [ChartPoint](chartpoint.md) |Leia as propriedades e os relacionamentos do objeto chartPoint.|
|[List](../api/chartpoint_list.md) | Coleção [ChartPoint](chartpoint.md) |Obtenha a coleção de objetos chartPoint. |
|[Itemat](../api/chartpointscollection_itemat.md)|[ChartPoint](chartpoint.md)|Recupera um ponto com base na respectiva posição dentro da série.|

## <a name="properties"></a>Propriedades
| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|value|object|Retorna o valor de um ponto do gráfico. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|formato|[ChartPointFormat](chartpointformat.md)|Encapsula as propriedades de formato de um ponto do gráfico. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartPoint"
}-->

```json
{
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartPoint resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->