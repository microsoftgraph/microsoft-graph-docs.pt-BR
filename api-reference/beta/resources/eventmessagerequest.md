---
title: tipo de recurso de eventMessageRequest
description: Uma mensagem que representa uma solicitação de reunião.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 5350b864ee38774f5b329110de6caf41f23dfe37
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981095"
---
# <a name="eventmessagerequest-resource-type"></a>tipo de recurso de eventMessageRequest

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Uma mensagem que representa uma solicitação de reunião.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "attachments",
    "event",
    "extensions",
    "previousLocation",
    "previousStartDateTime",
    "previousEndDateTime"
  ],
  "@odata.type": "microsoft.graph.eventMessageRequest"
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
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isOutOfDate": "Boolean",
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "meetingMessageType": "microsoft.graph.meetingMessageType",
  "parentFolderId": "string",
  "previousEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "previousLocation": {"@odata.type": "microsoft.graph.location"},
  "previousStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "receivedDateTime": "String (timestamp)",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
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
|bccRecipients|Coleção [recipient](recipient.md)|Os destinatários Cco: da mensagem.|
|body|[itemBody](itembody.md)|O corpo da mensagem.|
|bodyPreview|String|Os primeiros 255 caracteres do corpo da mensagem.|
|categories|String collection|As categorias associadas à mensagem.|
|ccRecipients|Coleção [recipient](recipient.md)|Os destinatários Cc: da mensagem.|
|changeKey|String|A versão da mensagem.|
|conversationId|String|A ID da conversa à qual o email pertence.|
|createdDateTime|DateTimeOffset|A data e a hora em que a mensagem foi criada.|
|endDateTime|[DateTimeTimeZone](datetimetimezone.md)|A hora de término da reunião solicitada.|
|from|[recipient](recipient.md)|O proprietário da caixa de correio e o remetente da mensagem.|
|hasAttachments|Boolean|Indica se a mensagem tem anexos.|
|id|String|Somente leitura.|
|importance|String| A importância da mensagem: `Low`, `Normal`, `High`.|
|inferenceClassification|String| Os valores possíveis são: `Focused` e `Other`.|
|isDeliveryReceiptRequested|Booliano|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|isDraft|Booliano|Indica se a mensagem é um rascunho. Uma mensagem é um rascunho quando ela ainda não foi enviada.|
|isOutOfDate|Booliano|Indica se esta solicitação de reunião foi feita desatualizada por uma solicitação mais recente.|
|isRead|Booliano|Indica se a mensagem foi lida.|
|isReadReceiptRequested|Booliano|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a mensagem foi alterada pela última vez.|
|location|[Location](location.md)|O local da reunião solicitada.|
|meetingMessageType|String| O tipo de mensagem de evento: `None`, `MeetingRequest`, `MeetingCancelled`, `MeetingAccepted`, `MeetingTenativelyAccepted`, `MeetingDeclined`.|
|parentFolderId|String|O identificador exclusivo para a mailFolder pai da mensagem.|
|previousEndDateTime|[DateTimeTimeZone](datetimetimezone.md)|A hora de término anterior da reunião solicitada.|
|previousLocation|[Localização](location.md)|O local anterior da reunião solicitada.|
|previousStartDateTime|[DateTimeTimeZone](datetimetimezone.md)|A hora de início anterior da reunião solicitada.|
|receivedDateTime|DateTimeOffset|A data e a hora em que a mensagem foi recebida.|
|recurrence|[PatternedRecurrence](patternedrecurrence.md)|O padrão de recorrência da reunião solicitada.|
|replyTo|Coleção [recipient](recipient.md)|Os endereços de email a serem usados ao responder.|
|sender|[recipient](recipient.md)|A conta que é realmente usada para gerar a mensagem.|
|sentDateTime|DateTimeOffset|A data e a hora em que a mensagem foi enviada.|
|startDateTime|[DateTimeTimeZone](datetimetimezone.md)|A hora de início da reunião solicitada.|
|subject|String|O assunto da mensagem.|
|toRecipients|Coleção [recipient](recipient.md)|Os destinatários Para: da mensagem.|
|type|String|O tipo de reunião solicitada: `singleInstance`, `occurence`, `exception`, `seriesMaster`.|
|uniqueBody|[itemBody](itembody.md)|A parte do corpo da mensagem que é exclusiva para a mensagem atual.|
|webLink|String|A URL para abrir a mensagem no Outlook Web App.<br><br>Você pode acrescentar um argumento ispopout ao final da URL para alterar como a mensagem é exibida. Se ispopout não houver presente ou estiver definido como 1, a mensagem será mostrada em uma janela pop-up. Se ispopout estiver definido como 0, o navegador mostrará a mensagem no painel de revisão do Outlook Web App.<br><br>A mensagem será aberta no navegador se você estiver conectado à sua caixa de correio por meio do Outlook Web App. Você será solicitado a fazer logon se ainda não estiver conectado no navegador.<br><br>Essa URL pode ser acessada de um iFrame.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|attachments|Coleção [Attachment](attachment.md)| Somente leitura. Anulável.|
|event|[Event](event.md)| O evento associado à mensagem de evento. A pressuposição dos participantes ou recursos da sala é que o Atendedor de Calendário esteja definido para atualizar automaticamente o calendário com um evento quando mensagens de evento de solicitação de reunião chegarem. Propriedade de navegação.  Somente leitura.|
|extensions|Coleção [Extension](extension.md)| Somente leitura. Anulável.|

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Get eventMessage](../api/eventmessage-get.md) | [eventMessage](eventmessage.md) |Ler propriedades e relações do objeto eventMessage.|
|[Criar anexo](../api/eventmessage-post-attachments.md) |[Anexo](attachment.md)| Criar um novo Anexo postando na coleção attachments.|
|[List attachments](../api/eventmessage-list-attachments.md) |Coleção [Attachment](attachment.md)| Obter uma coleção de objetos Attachment.|
|[Update](../api/eventmessage-update.md) | [eventMessage](eventmessage.md)  |Atualizar o objeto eventMessage. |
|[Delete](../api/eventmessage-delete.md) | Nenhum |Excluir o objeto eventMessage. |
|[copy](../api/message-copy.md)|[Message](message.md)||
|[createForward](../api/message-createforward.md)|[Message](message.md)||
|[createReply](../api/message-createreply.md)|[Message](message.md)||
|[createReplyAll](../api/message-createreplyall.md)|[Message](message.md)||
|[forward](../api/message-forward.md)|Nenhum|Encaminha uma mensagem. Em seguida, a mensagem será salva na pasta Itens enviados.|
|[move](../api/message-move.md)|[Message](message.md)|Move a mensagem para um mailFolder.|
|[reply](../api/message-reply.md)|Nenhum|Respostas que ela teve ao remetente de uma mensagem. Em seguida, a mensagem será salva na pasta Itens enviados.|
|[replyAll](../api/message-replyall.md)|Nenhum|Responder a todos os destinatários de uma mensagem. A mensagem é então salva na pasta Itens Enviados.|
|[send](../api/message-send.md)|Nenhum|Envia um rascunho de mensagem anteriormente criado. A mensagem é então salva na pasta Itens Enviados.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "eventMessageRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
