# <a name="mailtips-resource-type"></a>tipo de recurso mailTips

Mensagens informativas sobre um destinatário, que são exibidas para os usuários enquanto eles escrevem uma mensagem. Por exemplo, uma mensagem de ausência temporária como uma resposta automática para o destinatário de uma mensagem.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| automaticReplies | [automaticRepliesMailTips](../resources/automaticrepliesmailtips.md) | Dicas de email para a resposta automática, caso ela tenha sido configurada pelo destinatário. |
| customMailTip | Sequência de caracteres | Uma dica de email personalizada que pode ser definida na caixa de correio do destinatário. |
| deliveryRestricted| Booleano | Caso a caixa de correio do destinatário está restrita ou não, por exemplo, aceitando mensagens apenas de uma lista predefinida de remetentes, rejeitando mensagens de uma lista predefinida de remetentes ou aceitando mensagens apenas de remetentes autenticados. |
| emailAddress | [emailAddress](../resources/emailaddress.md) | O endereço de email do destinatário para recebimento das dicas de email. |
| error | [mailTipsError](../resources/mailtipserror.md) | Erros que ocorrem durante a ação [GetMailTips](../api/user_getmailtips.md). |
| externalMemberCount | Int32 | O número de membros externos, caso o destinatário seja uma lista de distribuição. |
| isModerated |Booleano  | Se o envio de mensagens para o destinatário requer aprovação. Por exemplo, se o destinatário for uma grande lista de distribuição e um moderador tiver sido configurado para aprovar mensagens enviadas para essa lista de distribuição ou se o envio de mensagens para um destinatário exigir a aprovação do gerente do destinatário. |
| mailboxFull | Booleano | O status completo da caixa de correio do destinatário. |
| maxMessageSize | Int32 | O tamanho máximo da mensagem que foi configurado para a organização ou a caixa de correio do destinatário. |
| recipientScope | recipientScopeType | O escopo do destinatário. Os valores possíveis são: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`. Por exemplo, um administrador pode definir outra organização como "parceira". O escopo é útil se um administrador quiser que determinadas dicas de e-mail estejam acessíveis a determinados escopos. Também é útil para os remetentes informá-los de que a mensagem pode sair da organização, ajudando-os a tomar as decisões corretas sobre texto, tom e conteúdo.|
| recipientSuggestions | Coleção [recipient](../resources/recipient.md) | Destinatários sugeridos com base em contextos anteriores em que aparecem na mesma mensagem. |
| totalMemberCount | Int32 | O número de membros, caso o destinatário seja uma lista de distribuição. |

### <a name="recipientscopetype-values"></a>Valores de recipientScopeType

| Valor
|:-------------------------
| none
| internal
| external
| externalPartner
| externalNonPartner


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "automaticReplies",
    "customMailTip",
    "deliveryRestricted",
    "emailAddress",
    "error",
    "externalMemberCount",
    "isModerated",
    "mailboxFull",
    "maxMessageSize",
    "recipientScope",
    "recipientSuggestions",
    "totalMemberCount"
  ],
  "@odata.type": "microsoft.graph.mailTips"
}-->

```json
{
  "automaticReplies": {"@odata.type": "microsoft.graph.automaticRepliesMailTips"},
  "customMailTip": "string",
  "deliveryRestricted": "boolean",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "error": {"@odata.type": "microsoft.graph.mailTipsError"},
  "externalMemberCount": 1024,
  "isModerated": "boolean",
  "mailboxFull": "boolean",
  "maxMessageSize": 1024,
  "recipientScope": "string",
  "recipientSuggestions": [{"@odata.type": "microsoft.graph.recipient"}],
  "totalMemberCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
