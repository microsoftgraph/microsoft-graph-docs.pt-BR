# <a name="chartaxis-resource-type"></a>Tipo de recurso ChartAxis

Representa um único eixo em um gráfico.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter ChartAxis](../api/chartaxis_get.md) | [WorkbookChartAxis](chartaxis.md) |Propriedades de leitura e relacionamentos do objeto chartAxis.|
|[Atualizar](../api/chartaxis_update.md) | [WorkbookChartAxis](chartaxis.md)   |Atualizar o objeto ChartAxis. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| id       |sequência de caracteres   | Identificador único. Somente leitura.|
|majorUnit|Json|Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.|
|maximum|Json|Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.|
|minimum|Json|Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.|
|minorUnit|Json|Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|formato|[WorkbookChartAxisFormat](chartaxisformat.md)|Representa a formatação de um objeto chart, que inclui formatação de linha e de fonte. Somente leitura.|
|majorGridlines|[WorkbookChartGridlines](chartgridlines.md)|Retorna um objeto gridlines que representa as principais linhas de grade do eixo especificado. Somente leitura.|
|minorGridlines|[WorkbookChartGridlines](chartgridlines.md)|Retorna um objeto Gridlines que representa as linhas de grade secundárias do eixo especificado. Somente leitura.|
|título|[WorkbookChartAxisTitle](chartaxistitle.md)|Representa o título do eixo. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookChartAxis"
}-->

```json
{
  "id": "string",
  "majorUnit": "string",
  "maximum": "string",
  "minimum": "string",
  "minorUnit": "string",
   "format": {"@odata.type": "microsoft.graph.workbookChartAxisFormat"},
  "majorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "minorGridlines": {"@odata.type": "microsoft.graph.workbookChartGridlines"},
  "title": {"@odata.type": "microsoft.graph.workbookChartAxisTitle"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartAxis resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->