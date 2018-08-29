# <a name="chartdatalabelformat-resource-type"></a>Tipo de recurso ChartDataLabelFormat

Abrange as propriedades de formatação dos rótulos de dados do gráfico.


## <a name="methods"></a>Métodos
Nenhum

## <a name="properties"></a>Propriedades
Nenhum

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|fill|[WorkbookChartFill](chartfill.md)|Representa o formato de preenchimento do rótulo de dados atual do gráfico. Somente leitura.|
|font|[WorkbookChartFont](chartfont.md)|Representa os atributos de fonte (nome, tamanho, cor, etc.) do rótulo de dados do gráfico. Somente leitura.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartDataLabelFormat"
}-->

```json
{
  "fill": {"@odata.type": "microsoft.graph.workbookChartFill"},
  "font": {"@odata.type": "microsoft.graph.workbookChartFont"}
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartDataLabelFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->