# <a name="pivottable-resource-type"></a>tipo de recurso de tabela dinâmica

Representa uma Tabela Dinâmica do Excel.

### <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get workbookPivotTable](../api/workbookpivottable_get.md) | [workbookPivotTable](workbookpivottable.md) |Leia as propriedades e relacionamentos do objeto workbookPivotTable.|
|[Refresh](../api/workbookpivottable_refresh.md)|Nenhum|Atualiza a Tabela Dinâmica.    |
|[Refreshall](../api/workbookpivottable_refreshall.md)|None|Atualização de todas as tabelas dentro de uma determinada planilha. Observe que esta ação está disponível somente na coleção de tabela dinâmica.|

### <a name="properties"></a>Propriedades
| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|id|String| Id da Tabela Dinâmica.    Somente leitura.|
|name|Cadeia de caracteres|Nome da Tabela Dinâmica.    |

### <a name="relationships"></a>Relações
| Relação | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|planilha|[worksheet](worksheet.md)| A planilha que contém a Tabela Dinâmica atual. Somente leitura.    |

### <a name="json-representation"></a>Representação JSON

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
