# <a name="message-resource-type"></a>tipo de recurso de mensagem

Uma mensagem em uma mailFolder.

Esse recurso permite:

- Adicionar seus próprios dados às propriedades personalizadas usando [extensions](../../../concepts/extensibility_overview.md).
- Usar a [consulta delta](../../../concepts/delta_query_overview.md) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/message_delta.md).

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Listar mensagens](../api/user_list_messages.md) |Coleção [message](message.md) | Obter todas as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário). |
|[Criar mensagem](../api/user_post_messages.md) | [message](message.md) | [Criar](../api/user_post_messages.md#request-1) um rascunho de uma nova mensagem. |
|[Obter mensagem](../api/message_get.md) | [message](message.md) |Ler propriedades e relações do objeto mensage.|
|[Atualizar](../api/message_update.md) | [message](message.md) |Atualizar o objeto message.|
|[Excluir](../api/message_delete.md) | Nenhum |Excluir o objeto message. |
|[copy](../api/message_copy.md)|[Message](message.md)|Copiar uma mensagem para uma pasta.|
|[createForward](../api/message_createforward.md)|[Message](message.md)|Criar um rascunho da mensagem de encaminhamento. Em seguida, você pode [atualizar](../api/message_update.md) ou [enviar](../api/message_send.md) esse rascunho.|
|[createReply](../api/message_createreply.md)|[Message](message.md)|Criar um rascunho da mensagem de resposta. Em seguida, você pode [atualizar](../api/message_update.md) ou [enviar](../api/message_send.md) esse rascunho.|
|[createReplyAll](../api/message_createreplyall.md)|[Message](message.md)|Criar um rascunho da mensagem Responder a Todos. Em seguida, você pode [atualizar](../api/message_update.md) ou [enviar](../api/message_send.md) esse rascunho.|
|[delta](../api/message_delta.md)|Coleção [message](message.md)| Obtenha um conjunto de mensagens que foram adicionadas, excluídas ou atualizadas em uma pasta especificada.|
|[forward](../api/message_forward.md)|Nenhum|Encaminhar uma mensagem. A mensagem é então salva na pasta Itens Enviados.|
|[move](../api/message_move.md)|[Message](message.md)|Mover a mensagem para uma pasta. Isso cria uma nova cópia da mensagem na pasta de destino.|
|[reply](../api/message_reply.md)|None|Responder ao remetente de uma mensagem. A mensagem é então salva na pasta Itens Enviados.|
|[replyAll](../api/message_replyall.md)|None|Responder a todos os destinatários de uma mensagem. A mensagem é então salva na pasta Itens Enviados.|
|[send](../api/message_send.md)|Nenhum|Envia um rascunho de mensagem anteriormente criado. A mensagem é então salva na pasta Itens Enviados.|
|**Anexos**| | |
|[Listar anexos](../api/message_list_attachments.md) |Coleção [Attachment](attachment.md)| Obtém todos os anexos em uma mensagem.|
|[Add attachment](../api/message_post_attachments.md) |[Attachment](attachment.md)| Adicione um novo anexo a uma mensagem postando na coleção attachments.|
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension_post_opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Criar uma extensão aberta e adicionar propriedades personalizadas em uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension_get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obter um ou mais objetos de extensão ou identificados por nome ou nome totalmente qualificado.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](../../../concepts/extensibility_schema_groups.md) || Crie uma definição para a extensão de esquema e use-a para adicionar dados digitados personalizados a um recurso.|
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[message](message.md)  |Criar uma ou mais propriedades estendidas de valor único em uma mensagem nova ou existente.   |
|[Obter mensagem com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty_get.md)  | [message](message.md) | Obter mensagens que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [message](message.md) | Criar uma ou mais propriedades estendidas de vários valores em uma mensagem nova ou existente.  |
|[Obter mensagem com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty_get.md)  | [message](message.md) | Obter uma mensagem que contenha uma propriedade estendida de vários valores usando `$expand`. |


## <a name="properties"></a>Propriedades
| Propriedade       | Tipo    |Descrição|
|:---------------|:--------|:----------|
|bccRecipients|Coleção [recipient](recipient.md)|Os destinatários Cco: da mensagem.|
|body|[itemBody](itembody.md)|O corpo da mensagem. Pode estar no formato HTML ou no formato de texto.|
|bodyPreview|String|Os primeiros 255 caracteres do corpo da mensagem. Está no formato de texto.|
|categories|Coleção de cadeias de caracteres|As categorias associadas à mensagem.|
|ccRecipients|Coleção [recipient](recipient.md)|Os destinatários Cc: da mensagem.|
|changeKey|String|A versão da mensagem.|
|conversationId|String|A ID da conversa à qual o email pertence.|
|createdDateTime|DateTimeOffset|A data e a hora em que a mensagem foi criada.|
|from|[recipient](recipient.md)|O proprietário da caixa de correio e o remetente da mensagem.|
|hasAttachments|Boolean|Indica se a mensagem tem anexos.|
|id|String|Identificador exclusivo da mensagem (observe que esse valor pode mudar se uma mensagem é movida ou alterada)|
|importance|String| A importância da mensagem: `Low`, `Normal`, `High`.|
|inferenceClassification | String | A classificação da mensagem para o usuário, com base na relevância deduzida ou na importância, ou em uma substituição explícita. Os valores possíveis são: `focused` ou `other`. |
|internetMessageId |String |A ID da mensagem no formato especificado por [RFC2822](http://www.ietf.org/rfc/rfc2822.txt). |
|isDeliveryReceiptRequested|Boolean|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|isDraft|Booliano|Indica se a mensagem é um rascunho. Uma mensagem é um rascunho quando ela ainda não foi enviada.|
|isRead|Boolean|Indica se a mensagem foi lida.|
|isReadReceiptRequested|Boolean|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a mensagem foi alterada pela última vez.|
|parentFolderId|String|O identificador exclusivo para a mailFolder pai da mensagem.|
|receivedDateTime|DateTimeOffset|A data e a hora em que a mensagem foi recebida.|
|replyTo|Coleção [recipient](recipient.md)|Os endereços de email a serem usados ao responder.|
|sender|[recipient](recipient.md)|A conta que é realmente usada para gerar a mensagem.|
|sentDateTime|DateTimeOffset|A data e a hora em que a mensagem foi enviada.|
|subject|String|O assunto da mensagem.|
|toRecipients|Coleção [recipient](recipient.md)|Os destinatários Para: da mensagem.|
|uniqueBody|[itemBody](itembody.md)|A parte do corpo da mensagem que é exclusiva para a mensagem atual. **uniqueBody** não é fornecido por padrão, mas pode ser recuperado por uma determinada mensagem pelo uso da consulta `?$select=uniqueBody`. Pode estar no formato HTML ou no formato de texto.|
|webLink|String|A URL para abrir a mensagem no Outlook Web App.<br><br>Você pode acrescentar um argumento ispopout ao final da URL para alterar como a mensagem é exibida. Se ispopout não houver presente ou estiver definido como 1, a mensagem será mostrada em uma janela pop-up. Se ispopout estiver definido como 0, o navegador mostrará a mensagem no painel de revisão do Outlook Web App.<br><br>A mensagem será aberta no navegador se você estiver conectado à sua caixa de correio por meio do Outlook Web App. Você será solicitado a fazer logon se ainda não estiver conectado no navegador.<br><br>Essa URL pode ser acessada de um iFrame.|

**Removendo o script da propriedade de corpo**

O corpo da mensagem pode estar em HTML ou em texto. Se o corpo for HTML, por padrão, qualquer HTML potencialmente não seguro (por exemplo, JavaScript) inserido na propriedade **body** será removido antes que o conteúdo do corpo seja retornado em uma resposta REST. Para obter o conteúdo HTML completo original, inclua o seguinte cabeçalho da solicitação HTTP:
```
Prefer: outlook.allow-unsafe-html
```

**Definindo as propriedades from e sender**

Quando uma mensagem está sendo redigida, na maioria dos casos, as propriedades From e Sender representam o mesmo usuário conectado, a menos que ele seja atualizado conforme descrito nos seguintes cenários:

- A propriedade **from** poderá ser alterada se o administrador do Exchange tiver atribuído direitos **sendAs** da caixa de correio a alguns outros usuários. O administrador pode fazer isso selecionando as **Permissões de Caixa de Correio** do proprietário da caixa de correio no Portal de Gerenciamento do Azure ou usando o Centro de Administração do Exchange ou um cmdlet Add-ADPermission do Windows PowerShell. Em seguida, você pode definir programaticamente a propriedade **from** como um desses usuários com direitos **sendAs** para essa caixa de correio.
- A propriedade **sender** poderá ser alterada se o proprietário da caixa de correio tiver delegado o envio de mensagens dessa caixa de correio para um ou mais usuários. O proprietário da caixa de correio pode delegar no Outlook. Quando um representante envia uma mensagem em nome do proprietário da caixa de correio, a propriedade **sender** é definida como a conta desse representante, enquanto a propriedade **from** Você pode definir programaticamente a propriedade **sender** para um usuário com direito de representante para essa caixa de correio.

## <a name="relationships"></a>Relações
| Relação | Tipo    |Descrição|
|:---------------|:--------|:----------|
|attachments|Coleção [attachment](attachment.md)|Os anexos [fileAttachment](fileattachment.md) e [itemAttachment](itemattachment.md) da mensagem.|
|extensions|Coleção [extension](extension.md)|A coleção de extensões abertas definidas para a mensagem. Somente leitura. Anulável.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a mensagem. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de valor único definidas para a mensagem. Somente leitura. Anulável.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "extensions",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.message"
}-->

```json
{
  "bccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "changeKey": "string",
  "conversationId": "string",
  "createdDateTime": "String (timestamp)",
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageId": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "parentFolderId": "string",
  "receivedDateTime": "String (timestamp)",
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "string"
}

```

## <a name="see-also"></a>Veja também

- [Get mailbox settings](../api/user_get_mailboxsettings.md) 
- [Atualizar configurações da caixa de correio](../api/user_update_mailboxsettings.md)
- [Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](../../../concepts/delta_query_overview.md)
- [Obter as alterações incrementais para as mensagens em uma pasta](../../../concepts/delta_query_messages.md)
- [Adicionar dados personalizados a recursos usando extensões](../../../concepts/extensibility_overview.md)
- [Adicionar dados personalizados aos usuários usando extensões abertas](../../../concepts/extensibility_open_users.md)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
