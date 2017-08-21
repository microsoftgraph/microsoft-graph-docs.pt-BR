# <a name="create-thread"></a>Criar thread

Crie um novo thread na conversa especificada. 

Um thread e uma postagem são criados conforme especificado. Use [responder ao thread](conversationthread_reply.md) para incluir postagens adicionais no thread. Ou, se receber a ID de postagem, você também poderá [responder](post_reply.md) a essa postagem no thread.

Observação: Você também pode [Iniciar uma nova conversa criando primeiro um thread](group_post_threads.md).

## <a name="prerequisites"></a>Pré-requisitos
Os seguintes **escopos** são necessários para executar esta API: *Group.ReadWrite.All*
## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/conversations/{id}/threads
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:---------------|:--------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [ConversationThread](../resources/conversationthread.md).

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `201, Created` e um objeto [ConversationThread](../resources/conversationthread.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "create_conversationthread_from_conversation"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/conversations/{id}/threads
Content-type: application/json

{
  "topic": "topic-value",
  "posts": [{
      "body": {
        "contentType": "html",
        "content": "this is body content"
      }
  }]
}
```
No corpo da solicitação, forneça uma representação JSON do objeto [ConversationThread](../resources/conversationthread.md).
##### <a name="response"></a>Resposta

Se for bem-sucedido, este método retornará um código de resposta `201, Created` e o `id` do novo thread no corpo da resposta. Este é um exemplo da resposta. 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationThread"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 346

{
  "id": "thread-id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
