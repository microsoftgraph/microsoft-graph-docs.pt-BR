---
title: tipo de recurso eventMessageRequest
description: Uma mensagem que representa uma solicitação de reunião.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: be7304f603cac5de8256f540b5df31f897c4f1ad
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2020
ms.locfileid: "41652204"
---
# <a name="eventmessagerequest-resource-type"></a>tipo de recurso eventMessageRequest

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma mensagem que representa uma solicitação de reunião na caixa de correio de um convidado.

A entidade **eventMessageRequest** é derivada de [eventMessage](eventmessage.md).

Para responder à solicitação de reunião, primeiro, use a propriedade de navegação **evento** para acessar o evento correspondente, conforme mostrado neste [exemplo](../api/eventmessage-get.md#example-2). Em seguida, [aceite](../api/event-accept.md), [tentativelyAccept](../api/event-tentativelyaccept.md)ou [recuse](../api/event-decline.md) esse evento associado ao **eventMessageRequest**.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.eventMessage",
  "optionalProperties": [
    "attachments",
    "event",
    "extensions",
    "mentions",
    "previousLocation",
    "previousStartDateTime",
    "previousEndDateTime"
  ],
  "@odata.type": "microsoft.graph.eventMessageRequest"
}-->

```json
{
  "allowNewTimeProposals": "Boolean",
  "bccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "changeKey": "string",
  "conversationId": "string",
  "conversationIndex": "String (binary)",
  "createdDateTime": "String (timestamp)",
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "isDelegated": true,
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isOutOfDate": "Boolean",
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "meetingMessageType": "microsoft.graph.meetingMessageType",
  "mentionsPreview": {"@odata.type": "microsoft.graph.mentionsPreview"},
  "parentFolderId": "string",
  "previousEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "previousLocation": {"@odata.type": "microsoft.graph.location"},
  "previousStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "receivedDateTime": "String (timestamp)",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "responseRequested": "Boolean",
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "type": "string",
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowNewTimeProposals| Booliano | `True` se o organizador permite que os convidados proponham um novo horário ao responder, caso contrário,`false`. Opcional. O padrão é `true`. |
|bccRecipients|Coleção [recipient](recipient.md)|Os destinatários Cco: da mensagem.|
|body|[itemBody](itembody.md)|O corpo da mensagem.|
|bodyPreview|Cadeia de caracteres|Os primeiros 255 caracteres do corpo da mensagem.|
|Categorias|String collection|As categorias associadas à mensagem.|
|ccRecipients|Coleção [recipient](recipient.md)|Os destinatários Cc: da mensagem.|
|changeKey|Cadeia de caracteres|A versão da mensagem.|
|conversationId|String|A ID da conversa à qual o email pertence.|
|conversationIndex|Edm.Binary|O índice da conversa à qual o email pertence.|
|createdDateTime|DateTimeOffset|A data e a hora em que a mensagem foi criada.|
|endDateTime|[DateTimeTimeZone](datetimetimezone.md)|A hora de término da reunião solicitada.|
|from|[recipient](recipient.md)|O proprietário da caixa de correio a partir da qual a mensagem é enviada. Na maioria dos casos, esse valor é o mesmo que a propriedade **Sender** , exceto para cenários de compartilhamento ou delegação. O valor deve corresponder à caixa de correio real que foi usada. Saiba mais sobre [como definir as propriedades from e sender](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) de uma mensagem.|
|hasAttachments|Boolean|Indica se a mensagem tem anexos.|
|id|Cadeia de caracteres|Somente leitura.|
|importância|String| A importância da mensagem: `Low`, `Normal`, `High`.|
|inferenceClassification|String| Os valores possíveis são: `Focused` e `Other`.|
|IsDelegated foi removida|Booliano|True se essa resposta de solicitação de reunião estiver acessível a um representante, caso contrário, false. O padrão é false.|
|isDeliveryReceiptRequested|Booliano|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|isDraft|Boolean|Indica se a mensagem é um rascunho. Uma mensagem é um rascunho quando ela ainda não foi enviada.|
|isOutOfDate|Booliano|Indica se esta solicitação de reunião foi desfeita por uma solicitação mais recente.|
|isRead|Boolean|Indica se a mensagem foi lida.|
|isReadReceiptRequested|Boolean|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a mensagem foi alterada pela última vez.|
|location|[Location](location.md)|O local da reunião solicitada.|
|meetingMessageType|String| O tipo de mensagem de evento: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTentativelyAccepted`, `meetingDeclined`.|
|mentionsPreview|[mentionsPreview](mentionspreview.md)|Informações sobre menções na mensagem. Ao processar uma solicitação `GET` /messages, o servidor define essa propriedade e a inclui na resposta por padrão. O servidor retornará null se não houver menções na mensagem. Opcional. |
|parentFolderId|Cadeia de caracteres|O identificador exclusivo para a mailFolder pai da mensagem.|
|previousEndDateTime|[DateTimeTimeZone](datetimetimezone.md)| Se a atualização da reunião alterar a hora de término da reunião, esta propriedade especificará a hora de término da reunião anterior.|
|previousLocation|[Location](location.md)| Se a atualização da reunião alterar o local da reunião, essa propriedade especificará o local da reunião anterior.|
|previousStartDateTime|[DateTimeTimeZone](datetimetimezone.md)| Se a atualização da reunião alterar a hora de início da reunião, esta propriedade especificará a hora de início da reunião anterior.|
|receivedDateTime|DateTimeOffset|A data e a hora em que a mensagem foi recebida.|
|recurrence|[PatternedRecurrence](patternedrecurrence.md)|O padrão de recorrência da reunião solicitada.|
|replyTo|Coleção [recipient](recipient.md)|Os endereços de email a serem usados ao responder.|
|responseRequested|Booliano|Defina como true se o remetente quiser que o convidado envie uma resposta para a reunião solicitada.|
|sender|[recipient](recipient.md)|A conta que é realmente usada para gerar a mensagem. Na maioria dos casos, esse valor é o mesmo da propriedade **from**. Você pode definir essa propriedade para um valor diferente ao enviar uma mensagem de uma [caixa de correio compartilhada](/exchange/collaboration/shared-mailboxes/shared-mailboxes), [para um calendário compartilhado ou como um representante](/graph/outlook-share-delegate-calendar.md). De qualquer forma, o valor deve corresponder à caixa de correio real que foi usada. Saiba mais sobre [como definir as propriedades from e sender](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) de uma mensagem.|
|sentDateTime|DateTimeOffset|A data e a hora em que a mensagem foi enviada.|
|startDateTime|[DateTimeTimeZone](datetimetimezone.md)|O horário de início da reunião solicitada.|
|assunto|String|O assunto da mensagem.|
|toRecipients|Coleção [recipient](recipient.md)|Os destinatários Para: da mensagem.|
|type|Cadeia de caracteres|O tipo de reunião solicitada `singleInstance`: `occurence`, `exception`, `seriesMaster`,.|
|uniqueBody|[itemBody](itembody.md)|A parte do corpo da mensagem que é exclusiva para a mensagem atual.|
|webLink|String|A URL para abrir a mensagem no Outlook Web App.<br><br>Você pode acrescentar um argumento ispopout ao final da URL para alterar como a mensagem é exibida. Se ispopout não houver presente ou estiver definido como 1, a mensagem será mostrada em uma janela pop-up. Se ispopout estiver definido como 0, o navegador mostrará a mensagem no painel de revisão do Outlook Web App.<br><br>A mensagem será aberta no navegador se você estiver conectado à sua caixa de correio por meio do Outlook Web App. Você será solicitado a fazer logon se ainda não estiver conectado no navegador.<br><br>Essa URL pode ser acessada de um iFrame.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|attachments|Coleção [attachment](attachment.md)|O conjunto de anexos de [Fileattachment](fileattachment.md), [hiperattachment](itemattachment.md)e [referenceAttachment](referenceattachment.md) para a mensagem. Somente leitura. Anulável.|
|event|[event](event.md)| O evento associado à mensagem de evento. A pressuposição dos participantes ou recursos da sala é que o Atendedor de Calendário esteja definido para atualizar automaticamente o calendário com um evento quando mensagens de evento de solicitação de reunião chegarem. Propriedade de navegação.  Somente leitura.|
|extensions|Coleção [extension](extension.md)| A coleção de extensões abertas definidas para eventMessage. Somente leitura. Anulável.|
|menções|Coleção [mention](mention.md) | Uma coleção de menções na mensagem, ordenada pelo **createdDateTime**, do mais novo para o mais antigo. Por padrão, um `GET` /messages não retorna essa propriedade, a menos que você aplique `$expand` à propriedade.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a eventMessage. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de valor único definidas para a eventMessage. Somente leitura. Anulável.|


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get eventMessage](../api/eventmessage-get.md) | [eventMessage](eventmessage.md) |Ler propriedades e relações do objeto eventMessage.|
|[Update](../api/eventmessage-update.md) | [eventMessage](eventmessage.md)  |Atualizar o objeto eventMessage.|
|[Delete](../api/eventmessage-delete.md) | None |Excluir o objeto eventMessage.|
|[copy](../api/message-copy.md)|[message](message.md)|Copiar uma mensagem para uma pasta.|
|[createForward](../api/message-createforward.md)|[message](message.md)|Criar um rascunho da mensagem de encaminhamento. Em seguida, você pode [atualizar](../api/message-update.md) ou [enviar](../api/message-send.md) esse rascunho.|
|[createReply](../api/message-createreply.md)|[message](message.md)|Criar um rascunho da mensagem de resposta. Em seguida, você pode [atualizar](../api/message-update.md) ou [enviar](../api/message-send.md) esse rascunho.|
|[createReplyAll](../api/message-createreplyall.md)|[message](message.md)|Criar um rascunho da mensagem Responder a Todos. Em seguida, você pode [atualizar](../api/message-update.md) ou [enviar](../api/message-send.md) esse rascunho.|
|[forward](../api/message-forward.md)|Nenhum|Encaminhar uma mensagem. A mensagem é então salva na pasta Itens Enviados.|
|[move](../api/message-move.md)|[message](message.md)|Mover uma mensagem para uma pasta. Isso cria uma nova cópia da mensagem na pasta de destino.|
|[reply](../api/message-reply.md)|Nenhum|Responder ao remetente de uma mensagem. A mensagem é então salva na pasta Itens Enviados.|
|[replyAll](../api/message-replyall.md)|Nenhum|Responder a todos os destinatários de uma mensagem. A mensagem é então salva na pasta Itens Enviados.|
|[send](../api/message-send.md)|Nenhum|Envia um rascunho de mensagem anteriormente criado. A mensagem é então salva na pasta Itens Enviados.|
|[unsubscribe](../api/message-unsubscribe.md)|Nenhum|Envie uma mensagem usando os dados e o endereço especificados no primeiro comando mailto no cabeçalho List-Unsubscribe.|
|**Anexos**| | |
|[List attachments](../api/eventmessage-list-attachments.md) |Coleção [attachment](attachment.md)| Obtenha todos os anexos em um eventMessage.|
|[Add attachment](../api/eventmessage-post-attachments.md) |[attachment](attachment.md)| Adicionar um novo anexo a um eventMessage postando na coleção attachments.|
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Criar uma extensão aberta e adicionar propriedades personalizadas em uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome.|
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[eventMessage](eventmessage.md)  |Criar uma ou mais propriedades estendidas de valor único em uma eventMessage nova ou existente.   |
|[Obter eventMessage com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-get.md)  | [eventMessage](eventmessage.md) | Obter eventMessages que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [eventMessage](eventmessage.md) | Criar uma ou mais propriedades estendidas de vários valores em uma eventMessage nova ou existente.  |
|[Obter eventMessage com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-get.md)  | [eventMessage](eventmessage.md) | Obter um eventMessage que contenha uma propriedade estendida de vários valores usando `$expand`. |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "eventMessageRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
