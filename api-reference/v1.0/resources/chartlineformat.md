# <a name="chartlineformat-resource-type"></a>Tipo de recurso ChartLineFormat

Abrange as opções de formatação dos elementos de linha.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get ChartLineFormat](../api/chartlineformat_get.md) | [ChartLineFormat](chartlineformat.md) |Leia as propriedades e os relacionamentos do objeto chartLineFormat.|
|[Update](../api/chartlineformat_update.md) | [ChartLineFormat](chartlineformat.md)    |Atualize o objeto ChartLineFormat. |
|[Clear](../api/chartlineformat_clear.md)|Nenhum|Limpe a formatação da linha de um elemento do gráfico.|

## <a name="properties"></a>Propriedades
| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|color|string|Código de cor HTML que representa a cor das linhas no gráfico.|

## <a name="relationships"></a>Relacionamentos
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chartLineFormat"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ChartLineFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->