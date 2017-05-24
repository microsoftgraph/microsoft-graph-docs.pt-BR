# <a name="patchcontentcommand-resource-type"></a>Tipo de recurso patchContentCommand

As alterações a serem feitas em uma página do OneNote em uma solicitação PATCH.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso, que é enviado no corpo da solicitação [PATCH pages/{id}`](../api/page_update.md). 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}-->

```json
{
  "action": "String",
  "content": "string",
  "position": "String",
  "target": "string"
}

```

## <a name="properties"></a>Propriedades
| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|ação|String|A ação a ser executada no elemento de destino. Os valores possíveis são: `replace`, `append`, `delete`, `insert` ou `prepend`.|
|conteúdo|String|Uma cadeia de caracteres de HTML bem formado para adicionar à página e dados binários de imagem ou arquivo. Se o conteúdo contiver dados binários, a solicitação deverá ser enviada usando o tipo de conteúdo `multipart/form-data` com uma parte "Commands". |
|position|String|O local para adicionar o conteúdo fornecido em relação ao elemento de destino. Os valores possíveis são: `after` (padrão) ou `before`.|
|destino|String|O elemento a atualizar. Deve ser `#<data-id>` ou o `<id>` gerado do elemento ou o `body` ou a palavra-chave de `title`.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->