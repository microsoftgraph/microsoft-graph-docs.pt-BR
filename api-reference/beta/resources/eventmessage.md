---
title: Tipo de recurso eventMessage
description: 'Uma mensagem que representa uma solicitação, cancelamento ou resposta de reunião (que pode ser uma destas: aceitação, aceitação provisória ou recusa). '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 59651f1d645c3c05a6aaddc1079e72203623302a
ms.sourcegitcommit: 7c017000888a910a0ad85404946f4fc50742c8d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/01/2020
ms.locfileid: "41652211"
---
# <a name="eventmessage-resource-type"></a>Tipo de recurso eventMessage

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma mensagem que representa uma solicitação, cancelamento ou resposta de reunião (que pode ser uma destas: aceitação, aceitação provisória ou recusa).

A entidade **eventMessage** é derivada de [message](message.md). **eventMessage** é o tipo base para [eventMessageRequest](eventmessagerequest.md) e [eventMessageResponse](eventmessageresponse.md). A propriedade **meetingMessageType** identifica o tipo de mensagem do evento.

Quando um organizador ou um aplicativo envia uma solicitação de reunião, a solicitação de reunião chega à caixa de correio de um convidado como uma instância do **eventMessage** com a **meetingMessageType** do **meetingRequest**. Além disso, o Outlook cria automaticamente uma instância de **evento** no calendário do convidado, com a propriedade **ShowAs** como **provisória**.

Para obter as propriedades do evento associado na caixa de correio do convidado, o aplicativo pode usar a propriedade de navegação de **evento** do **eventMessage**, conforme mostrado neste [exemplo de mensagem de evento Get](../api/eventmessage-get.md#example-2). O aplicativo também pode responder ao evento em nome do convidado de forma programática, [aceitando](../api/event-accept.md), [aceitando provisoriamente](../api/event-tentativelyaccept.md)ou [recusando](../api/event-decline.md) o evento.

Além de uma solicitação de reunião, uma instância do **eventMessage** pode ser encontrada na caixa de correio de um convidado como resultado de um organizador de eventos cancelando uma reunião ou na caixa de correio do organizador como resultado de um convite responder à solicitação de reunião. Um aplicativo pode atuar em mensagens de evento da mesma maneira que atua em mensagens com poucas diferenças.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.message",
  "optionalProperties": [
    "attachments",
    "event",
    "extensions",
    "mentions",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.eventMessage"
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
  "conversationIndex": "String (binary)",
  "createdDateTime": "DateTimeOffset",
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageHeaders": [{"@odata.type": "microsoft.graph.internetMessageHeader"}],
  "internetMessageId": "String",
  "isAllDay": "Boolean",
  "isDelegated": true,
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isOutOfDate": "Boolean",
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "DateTimeOffset",
  "location": {"@odata.type": "microsoft.graph.location"},
  "meetingMessageType": {"@odata.type": "microsoft.graph.meetingMessageType"},
  "mentionsPreview": {"@odata.type": "microsoft.graph.mentionsPreview"},
  "parentFolderId": "string",
  "receivedDateTime": "DateTimeOffset",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "DateTimeOffset",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "type": "string",
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "UnsubscribeData": "string",
  "UnsubscribeEnabled": true,
  "webLink": "string"
}

```

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|bccRecipients|Coleção [recipient](recipient.md)|Os destinatários Cco: da mensagem.|
|body|[itemBody](itembody.md)|O corpo da mensagem. Pode estar no formato HTML ou no formato de texto.|
|bodyPreview|Cadeia de caracteres|Os primeiros 255 caracteres do corpo da mensagem. Está no formato de texto. |
|categories|String collection|As categorias associadas à mensagem.|
|ccRecipients|Coleção [recipient](recipient.md)|Os destinatários Cc: da mensagem.|
|changeKey|Cadeia de caracteres|A versão da mensagem.|
|conversationId|String|A ID da conversa à qual o email pertence.|
|conversationIndex|Edm.Binary|Indica a posição da mensagem dentro da conversa.|
|createdDateTime|DateTimeOffset|A data e a hora em que a mensagem foi criada.|
|endDateTime|[dateTimeTimeZone](datetimetimezone.md)|A hora de término da reunião solicitada.|
|sinalizar|[followUpFlag](followupflag.md)|O valor do sinalizador que indica o status, a data de início, a data de conclusão ou a data de finalização da mensagem.|
|from|[recipient](recipient.md)|O proprietário da caixa de correio a partir da qual a mensagem é enviada. Na maioria dos casos, esse valor é o mesmo que a propriedade **Sender** , exceto para cenários de compartilhamento ou delegação. O valor deve corresponder à caixa de correio real que foi usada. Saiba mais sobre [como definir as propriedades from e sender](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) de uma mensagem.|
|hasAttachments|Boolean|Indica se a mensagem tem anexos.|
|id|Cadeia de caracteres| Identificador exclusivo da mensagem. [!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)] Somente leitura. |
|importância|Cadeia de caracteres| A importância da mensagem: `low`, `normal`, `high`.|
|inferenceClassification|String| Os valores possíveis são: `focused` e `other`.|
|internetMessageHeaders | Coleção [internetMessageHeader](internetmessageheader.md) | A coleção de cabeçalhos da mensagem, definida por [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), que fornece detalhes do caminho de rede adotado por uma mensagem do remetente para o destinatário. Somente leitura.|
|internetMessageId |String |A ID da mensagem no formato especificado por [RFC5322](https://www.ietf.org/rfc/rfc5322.txt). |
|isAllDay |Booliano|Indica se o evento dura todo o dia. Ajustar essa propriedade requer ajustar as propriedades **StartDateTime** e **EndDateTime** do evento também.|
|IsDelegated foi removida|Booliano|True se essa solicitação de reunião estiver acessível para um representante; caso contrário, false. O padrão é false.|
|isDeliveryReceiptRequested|Booliano|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|isDraft|Boolean|Indica se a mensagem é um rascunho. Uma mensagem é um rascunho quando ela ainda não foi enviada.|
|isOutOfDate|Booliano|Indica se esta solicitação de reunião foi desfeita por uma solicitação mais recente.|
|isRead|Boolean|Indica se a mensagem foi lida.|
|isReadReceiptRequested|Boolean|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a mensagem foi alterada pela última vez.|
|location|[location](location.md)|O local da reunião solicitada.|
|meetingMessageType|String| O tipo de mensagem de evento: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTentativelyAccepted`, `meetingDeclined`.|
|mentionsPreview|[mentionsPreview](mentionspreview.md)|Informações sobre menções na mensagem. Ao processar uma solicitação `GET` /messages, o servidor define essa propriedade e a inclui na resposta por padrão. O servidor retornará null se não houver menções na mensagem. Opcional. |
|parentFolderId|Cadeia de caracteres|O identificador exclusivo para a mailFolder pai da mensagem.|
|receivedDateTime|DateTimeOffset|A data e a hora em que a mensagem foi recebida.|
|recurrence|[patternedRecurrence](patternedrecurrence.md)|O padrão de recorrência da reunião solicitada.|
|replyTo|Coleção [recipient](recipient.md)|Os endereços de email a serem usados ao responder.|
|sender|[recipient](recipient.md)|A conta que é realmente usada para gerar a mensagem. Na maioria dos casos, esse valor é o mesmo da propriedade **from**. Você pode definir essa propriedade para um valor diferente ao enviar uma mensagem de uma [caixa de correio compartilhada](/exchange/collaboration/shared-mailboxes/shared-mailboxes), [para um calendário compartilhado ou como um representante](/graph/outlook-share-delegate-calendar.md). De qualquer forma, o valor deve corresponder à caixa de correio real que foi usada. Saiba mais sobre [como definir as propriedades from e sender](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) de uma mensagem.|
|sentDateTime|DateTimeOffset|A data e a hora em que a mensagem foi enviada.|
|startDateTime|[dateTimeTimeZone](datetimetimezone.md)|O horário de início da reunião solicitada.|
|assunto|Cadeia de caracteres|O assunto da mensagem.|
|toRecipients|Coleção [recipient](recipient.md)|Os destinatários Para: da mensagem.|
|type|Cadeia de caracteres|O tipo de reunião solicitada `singleInstance`: `occurence`, `exception`, `seriesMaster`,.|
|uniqueBody|[itemBody](itembody.md)|A parte do corpo da mensagem que é exclusiva para a mensagem atual.|
|UnsubscribeData|String|As entradas válidas analisadas no cabeçalho List-Unsubscribe.  Esses são os dados para o comando mail no cabeçalho List-Unsubscribe, se a propriedade UnsubscribeEnabled for true.|
|UnsubscribeEnabled|Booliano|Indica se a mensagem está habilitada para o cancelamento da assinatura.  valueTrue se o cabeçalho list-Unsubscribe estiver em conformidade com o rfc-2369.|
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

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Get eventMessage](../api/eventmessage-get.md) | [eventMessage](eventmessage.md) |Ler propriedades e relações do objeto eventMessage.|
|[Update](../api/eventmessage-update.md) | [eventMessage](eventmessage.md)  |Atualizar o objeto eventMessage.|
|[Delete](../api/eventmessage-delete.md) | Nenhum |Excluir o objeto eventMessage.|
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
  "description": "eventMessage resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
