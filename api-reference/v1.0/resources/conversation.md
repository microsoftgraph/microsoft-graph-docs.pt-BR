# <a name="conversation-resource-type"></a>tipo de recurso conversation

Uma conversa é uma coleção de [threads](conversationthread.md) e um thread contém postagens para este thread. Todos os threads e postagens em uma conversa compartilham o mesmo assunto.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar conversas](../api/group_list_conversations.md) | Coleção [conversation](conversation.md) |Obtenha a lista de conversas desse grupo.|
|[Create](../api/group_post_conversations.md) |[conversation](conversation.md)| Crie uma nova conversa incluindo um thread e uma postagem.|
|[Obter conversa](../api/conversation_get.md) | [conversation](conversation.md) |Leia as propriedades e os relacionamentos do objeto conversation.|
|[Delete](../api/conversation_delete.md) | Nenhuma |Exclua um objeto conversation. |
|[Listar threads de conversas](../api/conversation_list_threads.md) |Coleção [conversationThread](conversationthread.md)| Obtenha todos os threads em uma conversa de grupo.|
|[Criar thread de conversas](../api/conversation_post_threads.md) |Coleção [conversationThread](conversationthread.md)| Crie um thread na conversa especificada.|


## <a name="properties"></a>Propriedades
| Propriedade	       | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|hasAttachments|Booliano|Indica se qualquer uma das postagens nesta Conversa tem pelo menos um anexo.|
|id|String|Identificador exclusivo de conversas. Somente leitura.|
|lastDeliveredDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|visualização|String|Um breve resumo do corpo da última postagem nesta conversa.|
|topic|String|O tópico da conversa. Essa propriedade pode ser definida quando a conversa é criada, mas não pode ser atualizada.|
|uniqueSenders|Coleção de cadeias de caracteres|Todos os usuários que enviaram uma mensagem para esta conversa.|

## <a name="relationships"></a>Relações
| Relação | Tipo	    |Descrição|
|:---------------|:--------|:----------|
|threads|Coleção [conversationThread](conversationthread.md)|Uma coleção de todos os threads de conversa na conversa. Uma propriedade de navegação. Somente leitura. Anulável.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "threads"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversation"
}-->

```json
{
  "hasAttachments": true,
  "id": "string (identifier)",
  "lastDeliveredDateTime": "String (timestamp)",
  "preview": "string",
  "topic": "string",
  "uniqueSenders": ["string"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
