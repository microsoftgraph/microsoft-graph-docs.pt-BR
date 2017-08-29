# <a name="attachment-resource-type"></a>tipo de recurso attachment

Você pode adicionar conteúdo relacionado a um [event](../resources/event.md), [message](../resources/message.md) u [post](../resources/post.md) na forma de anexo

**attachment** é o recurso de base para os seguintes tipos de anexo derivados:

* Um arquivo (recurso [fileAttachment](../resources/fileattachment.md))
* Um item (contato, evento ou mensagem, representado por um recurso [itemAttachment](../resources/itemattachment.md))
* Um link para um arquivo (recurso [referenceAttachment](../resources/referenceAttachment.md))


## <a name="methods"></a>Métodos

Os métodos a seguir se aplicam a qualquer um dos tipos de anexo derivados (**fileAttachment**, **itemAttachment** ou **referenceAttachment**).

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter anexo](../api/attachment_get.md) | [attachment](attachment.md) |Leia as propriedades e as relações de um anexo, anexados a um evento, mensagem ou postagem.|
|[Adicionar anexo a um event](../api/event_post_attachments.md) | [attachment](attachment.md) |Adicione um arquivo, item ou anexo de link a um evento.|
|[Adicionar um anexo a uma mensagem](../api/message_post_attachments.md) | [attachment](attachment.md) |Adicione um arquivo, item ou anexo de link a uma mensagem.|
|[Adicionar anexo a uma postagem](../api/post_post_attachments.md) | [attachment](attachment.md) |Adicione um arquivo, item ou anexo de link a uma postagem.|
|[Listar anexos de um evento](../api/event_list_attachments.md) | Coleção [attachment](attachment.md) | Obtenha uma lista de anexos de um evento. |
|[Listar anexos de uma mensagem](../api/message_list_attachments.md) | Coleção [attachment](attachment.md) | Obtenha uma lista de anexos de uma mensagem. |
|[Listar anexos de uma postagem](../api/post_list_attachments.md) | Coleção [attachment](attachment.md) | Obtenha uma lista de anexos de uma postagem. |
|[Delete](../api/attachment_delete.md) | Nenhum |Exclua um anexo em um evento, mensagem ou postagem. |

## <a name="properties"></a>Propriedades

A seguir estão as propriedades de base de qualquer recurso de anexo. Consulte o tipo de anexo específico ([fileAttachment](../resources/fileattachment.md), [itemAttachment](../resources/itemattachment.md) ou [referenceAttachment](../resources/referenceAttachment.md)) para propriedades adicionais.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|contentType|String|O tipo MIME.|
|id|String| Somente leitura.|
|isInline|Booliano|`true` se o anexo for embutido; caso contrário, `false`.|
|lastModifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|nome|String|Nome de arquivo do anexo.|
|size|Int32|O comprimento do anexo em bytes.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.attachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "size": 1024
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
