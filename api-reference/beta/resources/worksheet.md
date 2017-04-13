# <a name="worksheet-resource-type"></a>Tipo de recurso Worksheet

Uma planilha do Excel é uma grade de células. Ela pode conter dados, tabelas, gráficos, etc.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get Worksheet](../api/worksheet_get.md) | [Worksheet](worksheet.md) |Leia as propriedades e os relacionamentos do objeto de planilha.|
|[Create Chart](../api/worksheet_post_charts.md) |[Chart](chart.md)| Crie um novo Gráfico ao postar na coleção de gráficos.|
|[Nomes da lista](../api/worksheet_list_names.md) |Coleção [NamedItem](nameditem.md)| Faça com que a coleção de itens nomeados seja associada à planilha.|
|[Listar gráficos](../api/worksheet_list_charts.md) |Coleção [Chart](chart.md)| Obtenha a coleção de objetos Chart.|
|[Create Table](../api/worksheet_post_tables.md) |[Table](table.md)| Crie uma nova Table postando na coleção de tabelas.|
|[List tables](../api/worksheet_list_tables.md) |Coleção [Table](table.md)| Obtenha uma coleção de objetos Table.|
|[Update](../api/worksheet_update.md) | [Worksheet](worksheet.md)    |Atualize o objeto Worksheet. |
|[Cell](../api/worksheet_cell.md)|[Range](range.md)|Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha.|
|[Range](../api/worksheet_range.md)|[Range](range.md)|Obtém o objeto de intervalo especificado pelo nome ou endereço.|
|[Usedrange](../api/worksheet_usedrange.md)|[Range](range.md)|O intervalo usado é o menor intervalo que abrange todas as células que têm um valor ou uma formatação atribuído a elas. Se a planilha estiver em branco, esta função retorna a célula superior esquerda.|
|[Delete](../api/worksheet_delete.md)|Nenhum|Exclui a planilha da pasta de trabalho.|
|[List](../api/worksheet_list.md) | Coleção [Worksheet](worksheet.md) |Obtenha a coleção de objetos da planilha. |
|[Add](../api/worksheetcollection_add.md)|[Worksheet](worksheet.md)|Adiciona uma nova planilha à pasta de trabalho. A planilha será adicionada ao final das planilhas existentes. |
|[List pivotTables](../api/workbookworksheet_list_pivottables.md) |Coleção [workbookPivotTable](workbookpivottable.md)| Obtenha uma coleção de objeto workbookPivotTable.|

## <a name="properties"></a>Propriedades
| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|id|string|Retorna um valor que identifica de forma exclusiva a planilha em uma determinada pasta de trabalho. O valor do identificador permanece o mesmo, ainda que a planilha seja renomeada ou movida. Somente leitura.|
|name|string|O nome de exibição da planilha.|
|position|int|A posição baseada em zero da planilha na pasta de trabalho.|
|visibilidade|string|A visibilidade da planilha. Os valores possíveis são: `Visible`, `Hidden` e `VeryHidden`.|

## <a name="relationships"></a>Relações
| Relação | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|charts|Coleção [Chart](chart.md)|Retorna uma coleção de gráficos que fazem parte da planilha. Somente leitura.|
|names|Coleção [NamedItem](nameditem.md)|Retorna a coleção de nomes associados à planilha. Somente leitura.|
|pivotTables|Coleção [workbookPivotTable](workbookpivottable.md)| Coleção de Tabelas Dinâmicas que fazem parte da planilha. |
|protection|[WorksheetProtection](worksheetprotection.md)|Retorna o objeto de proteção da planilha para uma planilha. Somente leitura.|
|tables|Coleção [Table](table.md)|Coleção de tabelas que fazem parte da planilha. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheet"
}-->

```json
{
  "id": "string",
  "name": "string",
  "position": 1024,
  "visibility": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Worksheet resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
