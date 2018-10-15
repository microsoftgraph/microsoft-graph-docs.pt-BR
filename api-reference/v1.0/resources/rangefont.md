# <a name="rangefont-resource-type"></a>Tipo de recurso RangeFont

Esse objeto representa os atributos de fonte de um objeto, como nome, tamanho, cor, etc.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get RangeFont](../api/rangefont_get.md) | [WorkbookRangeFont](rangefont.md) |Leia as propriedades e os relacionamentos do objeto rangeFormat.|
|[Atualizar](../api/rangefont_update.md) | [WorkbookRangeFont](rangefont.md)   |Atualize o objeto RangeFont. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|negrito|booliano|Representa o status da fonte em negrito.|
|cor|sequência de caracteres|Representação de código de cor HTML para a cor do texto. Por exemplo, #FF0000 representa vermelho.|
|italico|booliano|Representa o status da fonte em itálico.|
|nome|sequência de caracteres|Nome da fonte (por exemplo, "Calibri")|
|dimensionar|Double|Font Size|
|underline|sequência de caracteres|Tipo de sublinhado aplicado à fonte. Os valores possíveis são: `None`, `Single`, `Double`, `SingleAccountant`, `DoubleAccountant`.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeFont"
}-->

```json
{
  "bold": true,
  "color": "string",
  "italic": true,
  "name": "string",
  "size": 1024,
  "underline": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFont resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->