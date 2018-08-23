# <a name="update-message"></a>Atualizar mensagem

Atualizar as propriedades do objeto message.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Mail.ReadWrite    |
|Delegado (conta pessoal da Microsoft) | Mail.ReadWrite    |
|Aplicativo | Mail.ReadWrite |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | sequência de caracteres  | {token} de portador. Obrigatório. |
| Content-Type | sequência de caracteres  | Natureza dos dados no corpo de uma entidade. Obrigatório. |
## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados. As propriedades graváveis/atualizáveis são

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|bccRecipients|Destinatário|Os destinatários Cco da mensagem. Atualizável somente se isDraft = verdadeiro.|
|categorias|Coleção de sequência de caracteres|As categorias associadas à mensagem.|
|ccRecipients|Coleção de destinatários|Os destinatários Cc da mensagem. Atualizável somente se isDraft = verdadeiro.|
|de|Destinatário|O proprietário da caixa de correio e o remetente da mensagem. Atualizável somente se isDraft = verdadeiro. Deve corresponder à caixa de correio real usada.|
|importância|Sequência de caracteres|A importância da mensagem. Os valores possíveis são: `Low`, `Normal`, `High`.|
|inferenceClassification | Sequência de caracteres | A classificação da mensagem para o usuário, com base na relevância ou na importância deduzida, ou em uma substituição explícita. Os valores possíveis são: `focused` ou `other`. |
|internetMessageId |Sequência de caracteres |A ID da mensagem no formato especificado por [RFC2822](http://www.ietf.org/rfc/rfc2822.txt). Atualizável somente se isDraft = verdadeiro.|
|isRead|Booleano|Indica se a mensagem foi lida.|
|replyTo|Coleção de destinatários|Os endereços de e-mail a serem usados ao responder. Atualizável somente se isDraft = verdadeiro.|
|remetente|Destinatário|A conta que é realmente usada para gerar a mensagem. Atualizável somente se isDraft = verdadeiro, e quando enviar uma mensagem a partir de uma [caixa de correio compartilhada](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes)ou enviar uma mensagem como um [representante](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926). Em qualquer caso, o valor deve corresponder à caixa de correio real usada.|
|toRecipients|Coleção de destinatários|Os destinatários Para da mensagem. Atualizável somente se isDraft = verdadeiro.|
|corpo|ItemBody|O corpo da mensagem. Atualizável somente se isDraft = verdadeiro.|
|isDeliveryReceiptRequested|Booleano|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|isReadReceiptRequested|Booleano|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|assunto|Sequência de caracteres|O assunto da mensagem. Atualizável somente se isDraft = verdadeiro.|

Como o recurso **message** dá suporte a [extensions](../../../concepts/extensibility_overview.md), você pode usar a operação `PATCH` para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo nas propriedades personalizadas de uma extensão em uma instância de **message** existente.

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `200 OK` e o objeto [message](../resources/message.md) atualizado no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "inferenceClassification": "other"
}
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "inferenceClassification": "other"
}
```

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](../../../concepts/extensibility_overview.md)
- [Adicionar dados personalizados aos usuários usando extensões abertas (visualização)](../../../concepts/extensibility_open_users.md)
<!--
- [Add custom data to groups using schema extensions (preview)](../../../concepts/extensibility_schema_groups.md)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
