# <a name="post-resource-type"></a>tipo de recurso post
Representa um item Post individual em uma entidade [conversationThread](conversationthread.md).

Embora você não possa criar explicitamente uma postagem, seguir um destes procedimentos criaria uma postagem:

- [Responder a uma postagem existente](../api/post_reply.md) 
- [Responder a um thread existente](../api/conversationthread_reply.md) 
- [Criar um thread em uma nova conversa](../api/group_post_threads.md)
- [Criar uma nova conversa](../api/group_post_conversations.md)

Esse recurso permite que você adicione seus próprios dados às propriedades personalizadas usando [extensions](../../../concepts/extensibility_overview.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar postagens](../api/conversationthread_list_posts.md) | [post](post.md) |Obtenha as postagens do thread especificado. |
|[Obter postagem](../api/post_get.md) | [post](post.md) |Obtenha as propriedades e os relacionamentos de uma postagem em um thread especificado.|
|[Responder](../api/post_reply.md)|Nenhuma|Responda a uma postagem e adicione uma nova postagem ao thread especificado em uma conversa de grupo.|
|[Encaminhar](../api/post_forward.md)|Nenhuma|Encaminhe uma postagem para um destinatário.|
|**Anexos**| | |
|[Listar anexos](../api/post_list_attachments.md) |Coleção [attachment](attachment.md)| Obtenha todos os anexos em uma postagem.|
|[Add attachment](../api/post_post_attachments.md) |[attachment](attachment.md)| Adicione um anexo a uma postagem. |
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Criar uma extensão aberta e adicionar propriedades personalizadas em uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension_get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obter um ou mais objetos de extensão ou identificados por nome ou nome totalmente qualificado.|
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[post](post.md)  |Criar uma ou mais propriedades estendidas de valor único em uma postagem nova ou existente.   |
|[Obter postagem com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty_get.md)  | [post](post.md) | Obtenha postagens que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [post](post.md) | Crie uma ou mais propriedades estendidas de vários valores em uma postagem nova ou existente.  |
|[Obter postagem com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty_get.md)  | [post](post.md) | Obtenha uma postagem que contenha uma propriedade estendida de vários valores usando `$expand`. |

## <a name="properties"></a>Propriedades
| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|corpo|[itemBody](itembody.md)|O conteúdo da postagem. Esta é uma propriedade padrão. Esta propriedade pode ser nula.|
|categories|Coleção de cadeias de caracteres|As categorias associadas à postagem.|
|changeKey|String|Identifica a versão da postagem. Toda vez que a postagem muda, ChangeKey também muda. Isso permite que o Exchange aplique alterações na versão correta do objeto.|
|conversationId|String|ID exclusiva da conversa. Somente leitura.|
|conversationThreadId|String|ID exclusiva do thread de conversa. Somente leitura.|
|createdDateTime|DateTimeOffset|Especifica quando a postagem foi criada. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|from|[recipient](recipient.md)|Usado em cenários de acesso de representante. Indica quem postou a mensagem em nome de outro usuário. Esta é uma propriedade padrão.|
|hasAttachments|Booliano|Indica se a postagem tem pelo menos um anexo. Esta é uma propriedade padrão.|
|id|String| Somente leitura.|
|lastModifiedDateTime|DateTimeOffset|Especifica quando a postagem foi modificada pela última vez. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|newParticipants|Coleção [recipient](recipient.md)|Participantes da conversa que foram adicionados ao thread como parte desta postagem.|
|receivedDateTime|DateTimeOffset|Especifica quando a postagem foi recebida. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|sender|[recipient](recipient.md)|Contém o endereço do remetente. O valor de Sender será considerado o endereço do usuário autenticado caso o remetente não seja especificado. Esta é uma propriedade padrão.|

## <a name="relationships"></a>Relações
| Relação | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|attachments|Coleção [Attachment](attachment.md)| Somente leitura. Anulável.|
|extensions|Coleção [Extension](extension.md)|A coleção de extensões abertas definidas para a postagem. Somente leitura. Anulável.|
|inReplyTo|[post](post.md)| Somente leitura.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a postagem. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de valor único definidas para a postagem. Somente leitura. Anulável.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "inReplyTo",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.post"
}-->

```json
{
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "categories": ["string"],
  "changeKey": "string",
  "conversationId": "string",
  "conversationThreadId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "newParticipants": [{"@odata.type": "microsoft.graph.recipient"}],
  "receivedDateTime": "String (timestamp)",
  "sender": {"@odata.type": "microsoft.graph.recipient"}
}

```

## <a name="see-also"></a>Ver também

- [Adicionar dados personalizados a recursos usando extensões](../../../concepts/extensibility_overview.md)
- [Adicionar dados personalizados aos usuários usando extensões abertas (visualização)](../../../concepts/extensibility_open_users.md)
- [Adicionar dados personalizados a grupos usando extensões do esquema (visualização)](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
