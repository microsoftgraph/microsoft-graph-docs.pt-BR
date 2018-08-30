# <a name="itemattachment-resource-type"></a>Tipo de recurso itemAttachment

Um contato, evento ou mensagem que está anexado a outro evento, mensagem ou postagem.  

Derivado de [anexo](attachment.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter](../api/attachment_get.md) | [itemAttachment](itemattachment.md) |Leia as propriedades e os relacionamentos do objeto itemAttachment.|
|[Excluir](../api/attachment_delete.md) | Nenhum |Exclua o objeto itemAttachment. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|contentType|Cadeia de caracteres|O tipo de conteúdo do anexo.|
|id|Cadeia de caracteres| A ID do anexo.|
|isInline|Booliano|Defina como verdadeiro se o anexo estiver embutido, como uma imagem incorporada no corpo do item.|
|lastModifiedDateTime|DateTimeOffset|Última data e hora em que o anexo foi alterado.|
|nome|Cadeia de caracteres|O nome de exibição do anexo.|
|dimensionar|Int32|O tamanho do anexo em bytes.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|item|[OutlookItem](outlookitem.md)|A mensagem ou evento anexado. Propriedade de navegação.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "item"
  ],
  "baseType": "microsoft.graph.attachment",
  "@odata.type": "microsoft.graph.itemAttachment",
  "@odata.annotations": [
    {
      "property": "item",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024,
  "item": { "@odata.type": "microsoft.graph.outlookItem" }
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
