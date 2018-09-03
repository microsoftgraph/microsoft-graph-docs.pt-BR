# <a name="rangeborder-resource-type"></a>Tipo de recurso RangeBorder

Representa a borda de um objeto.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get RangeBorder](../api/rangeborder_get.md) | [WorkbookRangeBorder](rangeborder.md) |Propriedades de leitura e relacionamentos do objeto rangeBorder.|
|[Update](../api/rangeborder_update.md) | [WorkbookRangeBorder](rangeborder.md) |Atualiza o objeto RangeBorder. |
|[List](../api/rangeborder_list.md) | Coleção [WorkbookRangeBorder](rangeborder.md) |Obtém a coleção de objetos rangeBorder. |
|[Itemat](../api/rangebordercollection_itemat.md)|[WorkbookRangeBorder](rangeborder.md)|Obtém um objeto de borda usando seu índice|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|color|sequência de caracteres|Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").|
|id|sequência de caracteres|Representa o identificador da borda. Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Somente leitura.|
|sideIndex|sequência de caracteres|Valor constante que indica o lado específico da borda. Os valores possíveis são: `EdgeTop`, `EdgeBottom`, `EdgeLeft`, `EdgeRight`, `InsideVertical`, `InsideHorizontal`, `DiagonalDown`, `DiagonalUp`. Somente leitura.|
|style|sequência de caracteres|Uma das constantes do estilo da linha, especificando o estilo da linha da borda. Os valores possíveis são: `None`, `Continuous`, `Dash`, `DashDot`, `DashDotDot`, `Dot`, `Double`, `SlantDashDot`.|
|weight|sequência de caracteres|Especifica o peso da borda em um intervalo. Os valores possíveis são: `Hairline`, `Thin`, `Medium`, `Thick`.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookRangeBorder"
}-->

```json
{
  "color": "string",
  "id": "string",
  "sideIndex": "string",
  "style": "string",
  "weight": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeBorder resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->