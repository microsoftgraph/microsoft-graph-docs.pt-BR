# <a name="worksheet-resource-type"></a>Tipo de recurso Worksheet

Uma planilha do Excel é uma grade de células. Ela pode conter dados, tabelas, gráficos, etc.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Obter planilha](../api/worksheet_get.md) | [WorkbookWorksheet](worksheet.md) |Lê propriedades e relacionamentos do objeto worksheet.|
|[Criar gráfico](../api/worksheet_post_charts.md) |[WorkbookChart](chart.md)| Criar um novo Gráfico ao postar na coleção de gráficos.|
|[Nomes da lista](../api/worksheet_list_names.md) |Coleção [WorkbookNamedItem](nameditem.md)| Obter coleção de itens nomeados associada à planilha.|
|[Listar gráficos](../api/worksheet_list_charts.md) |Coleção [WorkbookChart](chart.md)| Obter uma coleção de objetos Chart.|
|[Criar tabela](../api/worksheet_post_tables.md) |[WorkbookTable](table.md)| Criar uma nova Tabela postando na coleção de tabelas.|
|[Listar tabelas](../api/worksheet_list_tables.md) |Coleção [WorkbookTable](table.md)| Obter uma coleção de objetos Table.|
|[Atualizar](../api/worksheet_update.md) | [WorkbookWorksheet](worksheet.md)   |Atualizar o objeto Worksheet. |
|[Célula](../api/worksheet_cell.md)|[Intervalo](range.md)|Obtém o objeto de intervalo que contém a célula única com base nos números de linha e de coluna. A célula pode estar fora dos limites do respectivo intervalo pai, desde que permaneça dentro da grade da planilha.|
|[Intervalo](../api/worksheet_range.md)|[Intervalo](range.md)|Obtém o objeto de intervalo especificado pelo nome ou endereço.|
|[Usedrange](../api/worksheet_usedrange.md)|[Intervalo](range.md)|O intervalo usado é o menor intervalo que abrange todas as células que têm um valor ou uma formatação atribuído a elas. Se a planilha estiver em branco, esta função retorna a célula superior esquerda.|
|[Excluir](../api/worksheet_delete.md)|Nenhum|Exclui a planilha da pasta de trabalho.|
|[Lista](../api/worksheet_list.md) | Coleção [WorkbookWorksheet](worksheet.md) |Obter a coleção de objetos worksheet. |
|[Adicionar](../api/worksheetcollection_add.md)|[WorkbookWorksheet](worksheet.md)|Adiciona uma nova planilha à pasta de trabalho. A planilha será adicionada ao final das planilhas existentes. |
|[Listar pivotTables](../api/workbookworksheet_list_pivottables.md) |Coleção [workbookPivotTable](workbookpivottable.md)| Obter uma coleção de objeto workbookPivotTable.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|sequência de caracteres|Retorna um valor que identifica de forma exclusiva a planilha em uma determinada pasta de trabalho. O valor do identificador permanece o mesmo, ainda que a planilha seja renomeada ou movida. Somente leitura.|
|name|sequência de caracteres|O nome de exibição da planilha.|
|position|int|A posição baseada em zero da planilha na pasta de trabalho.|
|visibilidade|sequência de caracteres|A Visibilidade da planilha. Os valores possíveis são: `Visible`, `Hidden`, `VeryHidden`.|

## <a name="relationships"></a>Relacionamentos
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|charts|Coleção [WorkbookChart](chart.md)|Retorna uma coleção de gráficos que fazem parte da planilha. Somente leitura.|
|names|Coleção [WorkbookNamedItem](nameditem.md)|Retorna a coleção de nomes associados à planilha. Somente leitura.|
|pivotTables|Coleção [workbookPivotTable](workbookpivottable.md)| Coleção de PivotTables que fazem parte da planilha. |
|protection|[WorkbookWorksheetProtection](worksheetprotection.md)|Retorna o objeto de proteção da planilha para uma planilha. Somente leitura.|
|tables|Coleção [WorkbookTable](table.md)|Coleção de tabelas que fazem parte da planilha. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookWorksheet"
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
