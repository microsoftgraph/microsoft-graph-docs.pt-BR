# tipo de recurso de tabela dinâmica
<a id="pivottable-resource-type" class="xliff"></a>

Representa uma Tabela Dinâmica do Excel.

## Métodos
<a id="methods" class="xliff"></a>

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get workbookPivotTable](../api/workbookpivottable_get.md) | [workbookPivotTable](workbookpivottable.md) |Leia as propriedades e relacionamentos do objeto workbookPivotTable.|
|[Refresh](../api/workbookpivottable_refresh.md)|Nenhum|Atualiza a Tabela Dinâmica. |
|[Refreshall](../api/workbookpivottable_refreshall.md)|None|Atualização de todas as tabelas dentro de uma determinada planilha. Observe que esta ação está disponível somente na coleção de tabela dinâmica.|

## Propriedades
<a id="properties" class="xliff"></a>
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|Cadeia de caracteres| Id da Tabela Dinâmica.   Somente leitura.|
|name|Cadeia de caracteres|Nome da Tabela Dinâmica.    |

## Relações
<a id="relationships" class="xliff"></a>
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|planilha|[worksheet](worksheet.md)| A planilha que contém a Tabela Dinâmica atual. Somente leitura.   |

## Representação JSON
<a id="json-representation" class="xliff"></a>
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
