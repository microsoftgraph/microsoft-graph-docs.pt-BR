# <a name="table-resource-type"></a>Tipo de recurso Table

Representa uma tabela do Excel.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get Table](../api/table_get.md) | [Table](table.md) |Leia as propriedades e relacionamentos do objeto de tabela.|
|[Create TableColumn](../api/table_post_columns.md) |[TableColumn](tablecolumn.md)| Crie uma nova TableColumn postando na coleção de colunas.|
|[List columns](../api/table_list_columns.md) |Coleção [TableColumn](tablecolumn.md)| Obtenha uma coleção de objetos TableColumn.|
|[Create TableRow](../api/table_post_rows.md) |[TableRow](tablerow.md)| Crie uma nova TableRow postando na coleção de linhas.|
|[List rows](../api/table_list_rows.md) |Coleção [TableRow](tablerow.md)| Obtenha uma coleção de objetos TableRow.|
|[Update](../api/table_update.md) | [Table](table.md)   |Atualize o objeto Table. |
|[Databodyrange](../api/table_databodyrange.md)|[Range](range.md)|Obtém o objeto de intervalo associado ao corpo de dados da tabela.|
|[Headerrowrange](../api/table_headerrowrange.md)|[Range](range.md)|Obtém o objeto de intervalo associado à linha de cabeçalho da tabela.|
|[Range](../api/table_range.md)|[Range](range.md)|Obtém o objeto de intervalo associado a toda a tabela.|
|[Totalrowrange](../api/table_totalrowrange.md)|[Range](range.md)|Obtém o objeto de intervalo associado à linha de totais da tabela.|
|[Clearfilters](../api/table_clearfilters.md)|Nenhum|Limpa todos os filtros aplicados à tabela no momento.|
|[Converttorange](../api/table_converttorange.md)|[Range](range.md)|Converte a tabela em um intervalo de células normal. Todos os dados são preservados.|
|[Delete](../api/table_delete.md)|Nenhum|Exclui a tabela.|
|[Reapplyfilters](../api/table_reapplyfilters.md)|Nenhum|Aplica novamente todos os filtros à tabela.|
|[List](../api/table_list.md) | Coleção [Table](table.md) |Obtenha a coleção de objetos da tabela. |
|[Add](../api/tablecollection_add.md)|[Table](table.md)|Cria uma nova tabela. O endereço de origem do intervalo determina a planilha à qual a tabela será adicionada. Se a tabela não puder ser adicionada (por exemplo, porque o endereço é inválido ou a tabela se sobreporia a outra), será gerado um erro.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|int|Retorna um valor que identifica de forma exclusiva a tabela em uma determinada pasta de trabalho. O valor do identificador permanece o mesmo, ainda que a tabela seja renomeada. Somente leitura.|
|name|string|Nome da tabela.|
|showHeaders|booliano|Indica se a linha do cabeçalho está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do cabeçalho.|
|showTotals|booliano|Indica se a linha do total está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do total.|
|style|string|Valor da constante que representa o estilo de Tabela. Os valores possíveis são: TableStyleLight1 a TableStyleLight21, TableStyleMedium1 a TableStyleMedium28, TableStyleStyleDark1 a TableStyleStyleDark11. Também é possível usar um estilo definido pelo usuário que esteja presente na planilha.|
|highlightFirstColumn|Booliano|Indica se a primeira coluna contém uma formatação especial.   |
|highlightLastColumn|Booliano|Indica se a última coluna contém uma formatação especial. |
|showBandedColumns|Booliano|Indica se as colunas mostram formatação em faixas nas quais as colunas ímpares são realçadas de modo diferente das colunas pares, tornando a leitura da tabela mais fácil.   |
|showBandedRows|Booliano|Indica se as linhas mostram formatação em faixas nas quais as linhas ímpares são realçadas de modo diferente das colunas pares, tornando a leitura da tabela mais fácil.    |
|showFilterButton|Booliano|Indica se os botões de filtro estão visíveis na parte superior de cada cabeçalho da coluna. Essa configuração só será permitida se a tabela tiver uma linha de cabeçalho.   |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|columns|Coleção [TableColumn](tablecolumn.md)|Representa uma coleção de todas as colunas na tabela. Somente leitura.|
|rows|Coleção [TableRow](tablerow.md)|Representa uma coleção de todas as linhas na tabela. Somente leitura.|
|sort|[TableSort](tablesort.md)|Representa a classificação da tabela. Somente leitura.|
|worksheet|[Worksheet](worksheet.md)|A planilha que contém a tabela atual. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.table"
}-->

```json
{
  "highlightFirstColumn": true,
  "highlightLastColumn": true,
  "id": "String (identifier)",
  "name": "String",
  "showBandedColumns": true,
  "showBandedRows": true,
  "showFilterButton": true,
  "showHeaders": true,
  "showTotals": true,
  "style": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Table resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
