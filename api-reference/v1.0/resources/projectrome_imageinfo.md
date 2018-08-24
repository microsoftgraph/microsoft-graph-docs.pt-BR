# <a name="imageinfo-resource-type"></a>tipo de recurso imageInfo

Um tipo complexo para representar a propriedade **atribuição** na parte [visualInfo](../resources/projectrome_visualinfo.md) do objeto [atividade](../resources/projectrome_activity.md).

## <a name="properties"></a>Propriedades

|Nome | Tipo | Descrição|
|:----|:-----|:-----------|
|iconurl | Sequência de caracteres | Opcional; URI que aponta para um ícone que representa o aplicativo usado para gerar a atividade|
|alternateText | Sequência de caracteres | Opcional; conteúdo de texto ALT acessível para a imagem|
|addImageQuery | Booleano | Opcional; parâmetro usado para indicar que o servidor é capaz de processar imagem dinamicamente em resposta à parametrização. Por exemplo, – uma imagem de alto contraste|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "iconUrl",
    "alternateText",
    "addImageQuery"
  ],
  "@odata.type": "microsoft.graph.imageInfo"
}-->

```json
{
    "@odata.type": "microsoft.graph.imageInfo",
    "iconUrl": "String (URL)",
    "alternateText": "String",
    "addImageQuery": "boolean"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "imageinfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->