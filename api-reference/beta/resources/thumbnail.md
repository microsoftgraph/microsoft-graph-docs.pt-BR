# <a name="thumbnail-resource-type"></a>Tipo de recurso thumbnail

O tipo de recurso **thumbnail** representa a miniatura de uma imagem, vídeo, documento ou qualquer arquivo ou pasta no OneDrive que tenha uma representação gráfica.

## <a name="properties"></a>Propriedades

| Propriedade	 | Tipo	   | Descrição                                  |
|:---------|:-------|:---------------------------------------------|
| height   | Int32  | A altura da miniatura em pixels.      |
| url      | Cadeia de caracteres | A URL usada para buscar o conteúdo da miniatura. |
| width    | Int32  | A largura da miniatura em pixels.       |


## <a name="relationships"></a>Relacionamentos

| Nome    | Tipo   | Descrição         |
|:--------|:-------|:--------------------|
| content | Fluxo | O fluxo do conteúdo. |


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": ["content", "height", "width"],
  "@odata.type": "microsoft.graph.thumbnail"
}-->

```json
{
  "url": "string",
  "height": 1024,
  "width": 1024,
  "content": "stream"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "thumbnail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
