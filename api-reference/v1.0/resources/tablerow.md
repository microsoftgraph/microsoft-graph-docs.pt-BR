# <a name="tablerow-resource-type"></a>Tipo de recurso TableRow

Representa uma linha em uma tabela.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get TableRow](../api/tablerow_get.md) | [WorkbookTableRow](tablerow.md) |Leia as propriedades e os relacionamentos do objeto tableRow.|
|[Atualizar](../api/tablerow_update.md) | [WorkbookTableRow](tablerow.md)  |Atualize o objeto TableRow. |
|[Intervalo](../api/tablerow_range.md)|[Intervalo](range.md)|Retorna o objeto de intervalo associado a toda a linha.|
|[Excluir](../api/tablerow_delete.md)|Nenhum|Exclui a linha da tabela.|
|[Lista](../api/tablerow_list.md) | Coleção [WorkbookTableRow](tablerow.md) |Obtenha uma coleção de objetos tableRow. |
|[Itemat](../api/tablerowcollection_itemat.md)|[WorkbookTableRow](tablerow.md)|Obtém uma linha com base em sua posição na coleção.|
|[Adicionar](../api/tablerowcollection_add.md)|[WorkbookTableRow](tablerow.md)|Adiciona uma nova linha à tabela.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|índice|int|Retorna o número de índice da linha na coleção de linhas da tabela. Indexados com zero. Somente leitura.|
|values|Json|Representa os valores brutos do intervalo especificado. Os dados retornados podem ser dos tipos: cadeia de caracteres, número ou booliano. Células que contêm um erro retornarão a cadeia de caracteres de erro.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookTableRow"
}-->

```json
{
  "index": 1024,
  "values": "json"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableRow resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->