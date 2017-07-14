# Configurando a mensagem de convite
<a id="configuring-the-invitation-message" class="xliff"></a>

O objeto invitedUserMessageInfo permite que você configure a mensagem de [convite](invitation.md).


## Propriedades
<a id="properties" class="xliff"></a>
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|ccRecipients|[Recipient](recipient.md)|Outros destinatários aos quais a mensagem de convite deve ser enviada. No momento, só é possível adicionar mais um destinatário.|
|customizedMessageBody|String|Corpo da mensagem personalizada a ser enviada caso você não queira a mensagem padrão.|
|messageLanguage|String|O idioma no qual você deseja enviar a mensagem padrão. Se customizedMessageBody for especificada, essa propriedade será ignorada, e a mensagem será enviada usando-se customizedMessageBody. O formato do idioma deve estar no ISO 639. O padrão é en-US.|


## Representação JSON
<a id="json-representation" class="xliff"></a>
Veja a seguir uma representação JSON do recurso

<!-- {"blockType": "resource", "@odata.type": "microsoft.graph.invitedUserMessageInfo"} -->
```json
{
  "ccRecipients": [ {"@odata.type": "microsoft.graph.recipient"} ],
  "customizedMessageBody": "string",
  "messageLanguage": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
