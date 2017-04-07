# <a name="tablesort-resource-type"></a>Tipo de recurso TableSort

Gerencia operações de classificação em objetos Table.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get TableSort](../api/tablesort_get.md) | [TableSort](tablesort.md) |Leia as propriedades e os relacionamentos do objeto tableSort.|
|[Apply](../api/tablesort_apply.md)|Nenhum|Execute uma operação de classificação.|
|[Clear](../api/tablesort_clear.md)|Nenhum|Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.|
|[Reapply](../api/tablesort_reapply.md)|Nenhum|Reaplica os parâmetros de classificação atuais à tabela.|

## <a name="properties"></a>Propriedades
| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|matchCase|booliano|Indica se o uso de maiúsculas ou minúsculas afetou a última classificação da tabela. Somente leitura.|
|method|string|Indica o último método de ordenação de caracteres chineses usado para classificar a tabela. Os valores possíveis são: `PinYin` e `StrokeCount`. Somente leitura.|

## <a name="relationships"></a>Relações
| Relação | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|campos|[SortField](sortfield.md)|Representa as condições atuais usadas para a última classificação da tabela. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tableSort"
}-->

```json
{
  "matchCase": true,
  "method": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "TableSort resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->