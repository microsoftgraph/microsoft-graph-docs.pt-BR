# <a name="table-resource-type"></a>Tipo de recurso Table

Representa uma tabela do Excel.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get Table](../api/table_get.md) | [WorkbookTable](table.md) |Propriedades de leitura e relacionamentos do objeto table.|
|[Create TableColumn](../api/table_post_columns.md) |[WorkbookTableColumn](tablecolumn.md)| Crie uma nova TableColumn postando na coleção de colunas.|
|[List columns](../api/table_list_columns.md) |Coleção [WorkbookTableColumn](tablecolumn.md)| Obtenha uma coleção de objetos TableColumn.|
|[Create TableRow](../api/table_post_rows.md) |[WorkbookTableRow](tablerow.md)| Crie uma nova TableRow postando na coleção de linhas.|
|[List rows](../api/table_list_rows.md) |Coleção [WorkbookTableRow](tablerow.md)| Obtenha uma coleção de objetos TableRow.|
|[Update](../api/table_update.md) | [WorkbookTable](table.md)   |Atualize o objeto Table. |
|[Databodyrange](../api/table_databodyrange.md)|[Range](range.md)|Obtém o objeto de intervalo associado ao corpo de dados da tabela.|
|[Headerrowrange](../api/table_headerrowrange.md)|[Range](range.md)|Obtém o objeto de intervalo associado à linha de cabeçalho da tabela.|
|[Range](../api/table_range.md)|[Range](range.md)|Obtém o objeto de intervalo associado a toda a tabela.|
|[Totalrowrange](../api/table_totalrowrange.md)|[Range](range.md)|Obtém o objeto de intervalo associado à linha de totais da tabela.|
|[Clearfilters](../api/table_clearfilters.md)|Nenhum|Limpa todos os filtros aplicados à tabela no momento.|
|[Converttorange](../api/table_converttorange.md)|[Range](range.md)|Converte a tabela em um intervalo de células normal. Todos os dados são preservados.|
|[Delete](../api/table_delete.md)|Nenhum|Exclui a tabela.|
|[Reapplyfilters](../api/table_reapplyfilters.md)|Nenhum|Aplica novamente todos os filtros à tabela.|
|[List](../api/table_list.md) | Coleção [WorkbookTable](table.md) |Obtenha a coleção de objetos table. |
|[Add](../api/tablecollection_add.md)|[WorkbookTable](table.md)|Cria uma nova tabela. O endereço de origem do intervalo determina a planilha à qual a tabela será adicionada. Se a tabela não puder ser adicionada (por exemplo, porque o endereço é inválido ou a tabela se sobreporia a outra), será gerado um erro.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|sequência de caracteres|Retorna um valor que identifica de forma exclusiva a tabela em uma determinada pasta de trabalho. O valor do identificador permanece o mesmo, ainda que a tabela seja renomeada. Essa propriedade deve ser interpretada como um valor de cadeia de caracteres opacas e não deve ser analisada para qualquer outro tipo. Somente leitura.|
|name|sequência de caracteres|Nome da tabela.|
|showHeaders|booliano|Indica se a linha do cabeçalho está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do cabeçalho.|
|showTotals|booliano|Indica se a linha do total está visível ou não. Esse valor pode ser definido para mostrar ou remover a linha do total.|
|style|sequência de caracteres|Valor constante que representa o estilo de tabela. Os valores possíveis são: TableStyleLight1 até o TableStyleLight21, TableStyleMedium1 até o TableStyleMedium28, TableStyleStyleDark1 até o TableStyleStyleDark11. Um estilo definido pelo usuário personalizado presente na pasta de trabalho também pode ser especificado.|
|highlightFirstColumn|Booliano|Indica se a primeira coluna contém uma formatação especial.   |
|highlightLastColumn|Booliano|Indica se a última coluna contém uma formatação especial. |
|showBandedColumns|Booliano|Indica se as colunas mostram formatação em faixas nas quais as colunas ímpares são realçadas de modo diferente das colunas pares, tornando a leitura da tabela mais fácil.   |
|showBandedRows|Booliano|Indica se as linhas mostram formatação em faixas nas quais as linhas ímpares são realçadas de modo diferente das colunas pares, tornando a leitura da tabela mais fácil.    |
|showFilterButton|Booliano|Indica se os botões de filtro estão visíveis na parte superior de cada cabeçalho da coluna. Essa configuração só será permitida se a tabela tiver uma linha de cabeçalho.   |
|legacyId|Cadeia de caracteres|ID herdada usada em clientes do Excel anteriores. O valor do identificador permanece o mesmo, ainda que a tabela seja renomeada. Essa propriedade deve ser interpretada como um valor de cadeia de caracteres opacas e não deve ser analisada para qualquer outro tipo. Somente leitura.   |

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|columns|Coleção [WorkbookTableColumn](tablecolumn.md)|Representa uma coleção de todas as colunas na tabela. Somente leitura.|
|rows|Coleção [WorkbookTableRow](tablerow.md)|Representa uma coleção de todas as linhas na tabela. Somente leitura.|
|sort|[WorkbookTableSort](tablesort.md)|Representa a classificação da tabela. Somente leitura.|
|planilha|[WorkbookWorksheet](worksheet.md)|A planilha que contém a tabela atual. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTable"
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
  "style": "String",
  "legacyId": "String"
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
