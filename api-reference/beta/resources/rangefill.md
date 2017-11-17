# <a name="rangefill-resource-type"></a>Tipo de recurso RangeFill

Representa o plano de fundo de um objeto de intervalo.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get RangeFill](../api/rangefill_get.md) | [RangeFill](rangefill.md) |Leia as propriedades e os relacionamentos do objeto rangeFill.|
|[Update](../api/rangefill_update.md) | [RangeFill](rangefill.md)    |Atualize o objeto RangeFill. |
|[Clear](../api/rangefill_clear.md)|Nenhum|Redefine o plano de fundo do intervalo.|

## <a name="properties"></a>Propriedades
| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|color|string|Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rangeFill"
}-->

```json
{
  "color": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFill resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->