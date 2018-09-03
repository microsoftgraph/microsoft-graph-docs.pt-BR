# <a name="messagerulepredicates-resource-type"></a>Tipo de recurso messageRulePredicates


Representa o conjunto de condições e exceções disponíveis para uma regra.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| bodyContains | Collection(String) | Representa as cadeias de caracteres que devem aparecer no corpo de uma mensagem de entrada para que a exceção ou condição seja aplicada. |
| bodyOrSubjectContains | Collection(String) | Representa as cadeias de caracteres que devem aparecer no corpo ou assunto de uma mensagem de entrada para que a exceção ou condição seja aplicada. |
| categories | Collection(String) | Representa as categorias com as quais a mensagem de entrada deve ser rotulada para que a exceção ou condição seja aplicada. |
| fromAddresses | Collection([recipient](recipient.md)) | Representa os endereços de email específicos do remetente de uma mensagem de entrada para que a condição ou exceção seja aplicada. |
| hasAttachments | Booleano | Indica se uma mensagem de entrada deve ter anexos para que a exceção ou condição seja aplicada. |
| headerContains | Collection(String) | Representa as cadeias de caracteres que são exibidas nos cabeçalhos de uma mensagem de entrada para que a exceção ou condição seja aplicada. |
| importance | importance | A importância que é marcada em uma mensagem de entrada para que a exceção ou condição seja aplicada: `low`, `normal`, `high`. |
| isApprovalRequest | Booleano | Indica se uma mensagem de entrada deve ter uma solicitação de aprovação para que a exceção ou condição seja aplicada. |
| isAutomaticForward | Booleano | Indica se uma mensagem de entrada deve ser encaminhada automaticamente para que a exceção ou condição seja aplicada. |
| isAutomaticReply | Booleano | Indica se uma mensagem de entrada deve ser uma resposta automática para que a exceção ou condição seja aplicada. |
| isEncrypted | Booleano | Indica se uma mensagem de entrada deve estar criptografada para que a exceção ou condição seja aplicada. |
| isMeetingRequest | Booleano | Indica se uma mensagem de entrada deve ser uma solicitação de reunião para que a exceção ou condição seja aplicada. |
| isMeetingResponse | Booleano | Indica se uma mensagem de entrada deve ser uma resposta à solicitação de reunião para que a exceção ou condição seja aplicada. |
| isNonDeliveryReport | Booleano | Indica se uma mensagem de entrada deve ser uma notificação de falha na entrega para que a exceção ou condição seja aplicada. |
| isPermissionControlled | Booleano | Indica se uma mensagem de entrada deve ser uma permissão controlada (protegida por RMS) para que a exceção ou condição seja aplicada. |
| isReadReceipt | Booleano | Indica se uma mensagem de entrada deve ser uma confirmação de leitura para que a exceção ou condição seja aplicada. |
| isSigned | Booleano | Indica se uma mensagem de entrada deve ser assinada por S/MIME para que a exceção ou condição seja aplicada. |
| isVoicemail | Booleano | Indica se uma mensagem de entrada deve ser uma caixa postal para que a exceção ou condição seja aplicada. |
| messageActionFlag | messageActionFlag  | Representa o valor do sinalizador de ações que é exibido em uma mensagem de entrada para que a exceção ou condição seja aplicada. Os valores possíveis são: `any`, `call`, `doNotForward`, `followUp`, `fyi`, `forward`, `noResponseNecessary`, `read`, `reply`, `replyToAll`, `review`. |
| notSentToMe | Booleano | Indica se o proprietário da caixa de correio não deve ser um destinatário de uma mensagem de entrada para que a condição ou exceção seja aplicada. |
| recipientContains | Collection(String) | Representa as cadeias de caracteres que são exibidas nas propriedades **toRecipients** ou **ccRecipients** de uma mensagem de entrada para que a exceção ou condição seja aplicada. |
| senderContains | Collection(String) | Representa as cadeias de caracteres que são exibidas na propriedade **from** de uma mensagem de entrada para que a exceção ou condição seja aplicada. |
| sensitivity | sensitivity | Representa o nível de sensibilidade que deve ser marcado em uma mensagem de entrada para que a condição ou exceção seja aplicada. Os valores possíveis são: `normal`, `personal`, `private`, `confidential`. |
| sentCcMe | Booleano | Indica se o proprietário da caixa de correio deve estar na propriedade **ccRecipients** de uma mensagem de entrada para que a condição ou exceção seja aplicada. |
| sentOnlyToMe | Booleano | Indica se o proprietário da caixa de correio deve ser o único destinatário em uma mensagem de entrada para que a condição ou exceção seja aplicada. |
| sentToAddresses | Collection([recipient](recipient.md)) | Representa os endereços de e-mail para os quais uma mensagem de entrada deve ter sido enviada para que a condição ou exceção seja aplicada. |
| sentToMe | Booleano | Indica se o proprietário da caixa de correio deve estar na propriedade **toRecipients** de uma mensagem de entrada para que a condição ou exceção seja aplicada. |
| sentToOrCcMe | Booleano | Indica se o proprietário da caixa de correio deve estar na propriedade **toRecipients** ou **ccRecipients** de uma mensagem de entrada para que a condição ou exceção seja aplicada. |
| subjectContains | Collection(String) | Representa as cadeias de caracteres que são exibidas no assunto de uma mensagem de entrada para que a exceção ou condição seja aplicada. |
| withinSizeRange | [sizeRange](sizerange.md) | Representa os tamanhos mínimo e máximo (em kilobytes) nos quais uma mensagem de entrada deve se enquadrar para que a condição ou exceção seja aplicada. |

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRulePredicates"
}-->

```json
{
  "bodyContains": ["String"],
  "bodyOrSubjectContains": ["String"],
  "categories": ["String"],
  "fromAddresses": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": "Boolean",
  "headerContains": ["String"],
  "importance": "String",
  "isApprovalRequest": "Boolean",
  "isAutomaticForward": "Boolean",
  "isAutomaticReply": "Boolean",
  "isEncrypted": "Boolean",
  "isMeetingRequest": "Boolean",
  "isMeetingResponse": "Boolean",
  "isNonDeliveryReport": "Boolean",
  "isPermissionControlled": "Boolean",
  "isReadReceipt": "Boolean",
  "isSigned": "Boolean",
  "isVoicemail": "Boolean",
  "messageActionFlag": "String",
  "notSentToMe": "Boolean",
  "recipientContains": ["String"],
  "senderContains": ["String"],
  "sensitivity": "String",
  "sentCcMe": "Boolean",
  "sentOnlyToMe": "Boolean",
  "sentToAddresses": [{"@odata.type": "microsoft.graph.recipient"}],
  "sentToMe": "Boolean",
  "sentToOrCcMe": "Boolean",
  "subjectContains": ["String"],
  "withinSizeRange": {"@odata.type": "microsoft.graph.sizeRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRulePredicates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
