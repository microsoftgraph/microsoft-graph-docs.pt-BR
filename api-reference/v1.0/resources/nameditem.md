# <a name="nameditem-resource-type"></a>Tipo de recurso NamedItem

Representa um nome definido para um intervalo de células ou um valor. Os nomes podem ser objetos nomeados primitivos (conforme exibido no tipo abaixo), objetos de intervalo ou uma referência a um intervalo. Use esse objeto para obter um objeto de intervalo associado aos nomes.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Add](../api/nameditem_add.md)|[WorkbookNamedItem](nameditem.md)|Adiciona um novo nome à coleção do escopo fornecido.|
|[AddFormulaLocal](../api/nameditem_addformulalocal.md)|[WorkbookNamedItem](nameditem.md)|Adiciona um novo nome à coleção de escopo fornecido usando a localidade do usuário para a fórmula.|
|[Get NamedItem](../api/nameditem_get.md) | [WorkbookNamedItem](nameditem.md) |Propriedades de leitura e os relacionamentos do objeto namedItem.|
|[Update](../api/nameditem_update.md) | [WorkbookNamedItem](nameditem.md)   |Atualiza o objeto NamedItem. |
|[Range](../api/nameditem_range.md)|[Range](range.md)|Retorna o objeto Range associado ao nome. Gera uma exceção quando o tipo de item nomeado não é um intervalo.|
|[List](../api/nameditem_list.md) | Coleção [WorkbookNamedItem](nameditem.md) |Obtém uma coleção de objetos namedItem. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|name|sequência de caracteres|O nome do objeto. Somente leitura.|
|comment|sequência de caracteres|Representa o comentário associado a esse nome.|
|scope|sequência de caracteres|Indica se o nome tem escopo para a pasta de trabalho ou uma planilha específica. Somente leitura.|
|type|sequência de caracteres|Indica o tipo de referência associada ao nome. Os valores possíveis são: `String`, `Integer`, `Double`, `Boolean`, `Range`. Somente leitura.|
|value|Json|Representa a fórmula definida como referência para o nome. Por exemplo, =Plan14!$B$2:$H$12, =4,75, etc. Somente leitura.|
|visible|booliano|Determina se o objeto fica visível ou não.|

## <a name="relationships"></a>Relações
| Relação     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|worksheet|[WorkbookWorksheet](worksheet.md)|Retorna a planilha do escopo do item nomeado. Disponível somente se o item estiver no escopo da planilha. Somente leitura.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookNamedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": {"@odata.type": "microsoft.graph.Json"},
  "visible": true
  
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
