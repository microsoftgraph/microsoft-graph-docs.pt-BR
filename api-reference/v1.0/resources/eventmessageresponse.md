---
title: Tipo de recurso eventMessageResponse
description: Uma mensagem que representa uma resposta a uma solicitação de reunião na caixa de correio do organizador da reunião.
ms.localizationpriority: medium
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 1e07b7cd2271b47605311ce2d58202e844f4c0bc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067386"
---
# <a name="eventmessageresponse-resource-type"></a>Tipo de recurso eventMessageResponse

Namespace: microsoft.graph

Uma mensagem que representa uma resposta a uma solicitação de reunião na caixa de correio do organizador da reunião.

Derivado de [eventMessage](eventmessage.md). 

Um organizador que recebe um **eventMessageResponse** com **o responseType** definido como ou , e que inclui uma propriedade `tentativelyAccepted` `declined` **proposedNewTime,** pode optar por aceitar a proposta. Para fazer isso, primeiro, use a propriedade de navegação de eventos **do eventMessageResponse** para acessar o evento correspondente, conforme mostrado neste [exemplo](../api/eventmessage-get.md#example-2).  Em [seguida,](../api/event-update.md) atualize o evento associado para a hora proposta.

Para obter mais informações sobre como propor uma hora e como receber e aceitar uma nova proposta de hora, consulte [Propor novos horários de reunião.](/graph/outlook-calendar-meeting-proposals)

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
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
|**Anexos**| | |
|[List attachments](../api/eventmessage-list-attachments.md) |Coleção [anexo](attachment.md)| Obtenha todos os anexos em um eventMessage.|
|[Add attachment](../api/eventmessage-post-attachments.md) |[anexo](attachment.md)| Adicionar um novo anexo a um eventMessage postando na coleção attachments.|
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Criar uma extensão aberta e adicionar propriedades personalizadas em uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obter uma extensão aberta identificada pelo nome.|
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[eventMessage](eventmessage.md)  |Criar uma ou mais propriedades estendidas de valor único em uma eventMessage nova ou existente.   |
|[Obter eventMessage com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-get.md)  | [eventMessage](eventmessage.md) | Obter eventMessages que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [eventMessage](eventmessage.md) | Criar uma ou mais propriedades estendidas de vários valores em uma eventMessage nova ou existente.  |
|[Obter eventMessage com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-get.md)  | [eventMessage](eventmessage.md) | Obter um eventMessage que contenha uma propriedade estendida de vários valores usando `$expand`. |


## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|bccRecipients|Coleção [recipient](recipient.md)|Os destinatários Cco: da mensagem.|
|body|[itemBody](itembody.md)|O corpo da mensagem. Pode estar no formato HTML ou no formato de texto.|
|bodyPreview|String|Os primeiros 255 caracteres do corpo da mensagem. Está no formato de texto. |
|categories|String collection|As categorias associadas à mensagem.|
|ccRecipients|Coleção [recipient](recipient.md)|Os destinatários Cc: da mensagem.|
|changeKey|String|A versão da mensagem.|
|conversationId|String|A ID da conversa à qual o email pertence.|
|conversationIndex|Edm.Binary|O Índice da conversa à qual o email pertence.|
|createdDateTime|DateTimeOffset|O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|endDateTime|[dateTimeTimeZone](datetimetimezone.md)|A hora de término da reunião solicitada.|
|flag|[followupFlag](followupflag.md)|O valor do sinalizador que indica o status, a data de início, a data de conclusão ou a data de finalização da mensagem.|
|from|[recipient](recipient.md)|O proprietário da caixa de correio da qual a mensagem foi enviada. Na maioria dos casos, esse valor é o mesmo que o da propriedade **remetente**, exceto para cenários de compartilhamento ou delegação. O valor deve corresponder à caixa de correio real que foi usada. Saiba mais sobre [como definir as propriedades from e sender](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) de uma mensagem.|
|hasAttachments|Booliano|Indica se a mensagem tem anexos.|
|id|Cadeia de caracteres| Identificador exclusivo da mensagem. [!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)] Somente leitura. |
|importância|String| A importância da mensagem: `low`, `normal`, `high`.|
|inferenceClassification|String| Os valores possíveis são: `focused` e `other`.|
|internetMessageHeaders | Coleção [internetMessageHeader](internetmessageheader.md) | A coleção de cabeçalhos da mensagem, definida por [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), que fornece detalhes do caminho de rede adotado por uma mensagem do remetente para o destinatário. Somente leitura.|
|internetMessageId |String |A ID da mensagem no formato especificado por [RFC5322](https://www.ietf.org/rfc/rfc5322.txt). |
|isAllDay |Booliano|Indica se o evento dura o dia inteiro. Ajustar essa propriedade requer o ajuste das **propriedades startDateTime** e **endDateTime** do evento também.|
|isDelegated|Boolean|True se essa resposta de solicitação de reunião estiver acessível a um representante, caso contrário, false. O padrão é falso.|
|isDeliveryReceiptRequested|Boolean|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|isDraft|Boolean|Indica se a mensagem é um rascunho. Uma mensagem é um rascunho quando ela ainda não foi enviada.|
|isOutOfDate|Booliano|Indica se essa solicitação de reunião foi feita fora de data por uma solicitação mais recente.|
|isRead|Boolean|Indica se a mensagem foi lida.|
|isReadReceiptRequested|Boolean|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|lastModifiedDateTime|DateTimeOffset|O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|location|[location](location.md)|O local da reunião solicitada.|
|meetingMessageType|String| O tipo de mensagem de evento: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTentativelyAccepted`, `meetingDeclined`.|
|parentFolderId|String|O identificador exclusivo para a mailFolder pai da mensagem.|
|proposedNewTime|[timeSlot](timeslot.md)|Uma data/hora alternativa proposta por um convidado para que uma solicitação de reunião seja inicial e final. Somente leitura. Não filtre.|
|receivedDateTime|DateTimeOffset|O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|O padrão de recorrência da reunião solicitada.|
|replyTo|Coleção [recipient](recipient.md)|Os endereços de email a serem usados ao responder.|
|responseType|cadeia de caracteres| Especifica o tipo de resposta a uma solicitação de reunião. Os valores possíveis são: `tentativelyAccepted`, `accepted`, `declined`. Para o tipo eventMessageResponse, `none` , e não há `organizer` `notResponded` suporte. Somente leitura. Não filtre.|
|sender|[recipient](recipient.md)|A conta que é realmente usada para gerar a mensagem. Na maioria dos casos, esse valor é o mesmo da propriedade **from**. Você pode definir essa propriedade como um valor diferente ao enviar uma mensagem de uma [caixa de correio compartilhada](/exchange/collaboration/shared-mailboxes/shared-mailboxes), [ou ao enviar uma mensagem como um delegado](/graph/outlook-share-delegate-calendar.md). De qualquer forma, o valor deve corresponder à caixa de correio real que foi usada. Saiba mais sobre [como definir as propriedades from e sender](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) de uma mensagem.|
|sentDateTime|DateTimeOffset|O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|A hora de início da reunião solicitada.|
|assunto|String|O assunto da mensagem.|
|toRecipients|Coleção [recipient](recipient.md)|Os destinatários Para: da mensagem.|
|tipo|Cadeia de caracteres|O tipo de reunião solicitada: `singleInstance` , `occurence` , , `exception` `seriesMaster` .|
|uniqueBody|[itemBody](itembody.md)|A parte do corpo da mensagem que é exclusiva para a mensagem atual.|
|webLink|String|O URL para abrir a mensagem no Outlook na Web.<br><br>Você pode anexar um argumento ispopout ao final do URL para alterar a forma como a mensagem é exibida. Se ispopout não estiver presente ou se estiver definido como 1, a mensagem será exibida em uma janela popout. Se ispopout estiver definido como 0, o navegador mostrará a mensagem no painel de revisão do Outlook na Web.<br><br>A mensagem será aberta no navegador se você estiver conectado à sua caixa de correio através do Outlook na Web. Você será solicitado a fazer o login, se ainda não estiver conectado com o navegador.<br><br>Este URL não pode ser acessado a partir de um iFrame.|


## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|attachments|Coleção [anexo](attachment.md)|A coleção [de anexos fileAttachment,](fileattachment.md) [itemAttachment](itemattachment.md)e [referenceAttachment](referenceattachment.md) para a mensagem. Somente leitura. Anulável.|
|event|[event](event.md)| O evento associado à mensagem de evento. A pressuposição dos participantes ou recursos da sala é que o Atendedor de Calendário esteja definido para atualizar automaticamente o calendário com um evento quando mensagens de evento de solicitação de reunião chegarem. Propriedade de navegação.  Somente leitura.|
|extensions|[extension](extension.md) collection| A coleção de extensões abertas definidas para eventMessage. Somente leitura. Anulável.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a eventMessage. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de valor único definidas para a eventMessage. Somente leitura. Anulável.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.eventMessageResponse",
  "baseType": "microsoft.graph.eventMessage",
  "keyProperty": "id"
}-->

```json
{
  "bccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "String",
  "categories": ["String"],
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "changeKey": "String",
  "conversationId": "String",
  "conversationIndex": "String (binary)",
  "createdDateTime": "String (timestamp)",
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "String (identifier)",
  "importance": "string",
  "inferenceClassification": "string",
  "internetMessageHeaders": [{"@odata.type": "microsoft.graph.internetMessageHeader"}],
  "internetMessageId": "String",
  "isAllDay": true,
  "isDelegated": true,
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isOutOfDate": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "meetingMessageType": "string",
  "parentFolderId": "String",
  "proposedNewTime": {"@odata.type": "microsoft.graph.timeSlot"},
  "receivedDateTime": "String (timestamp)",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "responseType": "string",
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "String",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "type": "string",
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "eventMessageResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
