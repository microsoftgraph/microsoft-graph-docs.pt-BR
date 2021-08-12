---
title: Tipo de recurso eventMessage
description: 'Uma mensagem que representa uma solicitação, cancelamento ou resposta de reunião (que pode ser uma destas: aceitação, aceitação provisória ou recusa).'
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d704072ac46899ec3158ddd290bbc56a628e3f8c9b8a4cb6d7105505f5cfd969
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212092"
---
# <a name="eventmessage-resource-type"></a>Tipo de recurso eventMessage

Namespace: microsoft.graph

Uma mensagem que representa uma solicitação, cancelamento ou resposta de reunião (que pode ser uma destas: aceitação, aceitação provisória ou recusa).

A entidade **eventMessage** é derivada de [message](message.md). **eventMessage** é o tipo base para [eventMessageRequest](eventmessagerequest.md) e [eventMessageResponse](eventmessageresponse.md). A propriedade **meetingMessageType** identifica o tipo de mensagem do evento.

Quando um organizador ou aplicativo envia uma solicitação de reunião, a solicitação de reunião chega na caixa de correio de um convidado como **uma instância eventMessage** com **o meetingMessageType** de **meetingRequest**. Além disso, Outlook cria automaticamente uma instância de evento no calendário do convidado, com **a** propriedade **showAs** **como tentativa**. 

Para obter as propriedades do evento associado na caixa de correio  do convidado, o aplicativo pode usar a propriedade de navegação de eventos **do eventMessage**, conforme mostrado neste exemplo de mensagem de evento get [.](../api/eventmessage-get.md#example-2) O aplicativo também pode responder ao evento em nome do convidado [](../api/event-tentativelyaccept.md)programaticamente, aceitando [,](../api/event-accept.md)aceitando ou [diminuindo](../api/event-decline.md) o evento.

Além de uma solicitação de reunião, uma instância **eventMessage** pode ser encontrada na caixa de correio de um convidado como resultado de um organizador de eventos cancelar uma reunião ou na caixa de correio do organizador como resultado de um convite respondendo à solicitação de reunião. Um aplicativo pode atuar em mensagens de evento da mesma maneira que atua em mensagens com poucas diferenças.
## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Get eventMessage](../api/eventmessage-get.md) | [eventMessage](eventmessage.md) |Ler propriedades e relações do objeto eventMessage.|
|[Update](../api/eventmessage-update.md) | [eventMessage](eventmessage.md)  |Atualizar o objeto eventMessage. |
|[Delete](../api/message-delete.md) | None |Excluir o objeto eventMessage. |
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
|[List attachments](../api/eventmessage-list-attachments.md) |Coleção [attachment](attachment.md)| Obtenha todos os anexos em um eventMessage.|
|[Add attachment](../api/eventmessage-post-attachments.md) |[attachment](attachment.md)| Adicionar um novo anexo a um eventMessage postando na coleção attachments.|
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Criar uma extensão aberta e adicionar propriedades personalizadas em uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obter um ou mais objetos de extensão ou identificados por nome ou nome totalmente qualificado.|
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[eventMessage](eventmessage.md)  |Criar uma ou mais propriedades estendidas de valor único em uma eventMessage nova ou existente.   |
|[Obter eventMessage com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-get.md)  | [eventMessage](eventmessage.md) | Obter eventMessages que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [eventMessage](eventmessage.md) | Criar uma ou mais propriedades estendidas de vários valores em uma eventMessage nova ou existente.  |
|[Obter eventMessage com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-get.md)  | [eventMessage](eventmessage.md) | Obter um eventMessage que contenha uma propriedade estendida de vários valores usando `$expand`. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|bccRecipients|Coleção [recipient](recipient.md)|Os destinatários Cco: da mensagem.|
|body|[itemBody](itembody.md)|O corpo da mensagem. Pode estar no formato HTML ou no formato de texto.|
|bodyPreview|String|Os primeiros 255 caracteres do corpo da mensagem. Está no formato de texto.|
|categories|String collection|As categorias associadas à mensagem.|
|ccRecipients|Coleção [recipient](recipient.md)|Os destinatários Cc: da mensagem.|
|changeKey|String|A versão da mensagem.|
|conversationId|String|A ID da conversa à qual o email pertence.|
|conversationIndex|Edm.Binary|Indica a posição da mensagem dentro da conversa.|
|createdDateTime|DateTimeOffset|A data e a hora em que a mensagem foi criada.|
|flag|[followupFlag](followupflag.md)|O valor do sinalizador que indica o status, a data de início, a data de conclusão ou a data de finalização da mensagem.|
|from|[recipient](recipient.md)|O proprietário da caixa de correio da qual a mensagem foi enviada. Na maioria dos casos, esse valor é o mesmo que o da propriedade **remetente**, exceto para cenários de compartilhamento ou delegação. O valor deve corresponder à caixa de correio real que foi usada. Saiba mais sobre [como definir as propriedades from e sender](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) de uma mensagem.|
|hasAttachments|Booliano|Indica se a mensagem tem anexos.|
|id|Cadeia de caracteres|Identificador exclusivo da mensagem de evento (observe que esse valor pode mudar se uma mensagem for movida ou alterada)|
|importância|String| A importância da mensagem: `low`, `normal`, `high`.|
|inferenceClassification|String| Os valores possíveis são: `focused` , `other` .|
|internetMessageHeaders | Coleção [internetMessageHeader](internetmessageheader.md) | A coleção de cabeçalhos da mensagem, definida por [RFC5322](https://www.ietf.org/rfc/rfc5322.txt), que fornece detalhes do caminho de rede adotado por uma mensagem do remetente para o destinatário. Somente leitura.|
|internetMessageId |String |A ID da mensagem no formato especificado por [RFC2822](https://www.ietf.org/rfc/rfc2822.txt). |
|isDelegated|Booliano|True se essa solicitação de reunião estiver acessível a um representante, caso contrário, false. O padrão é false.|
|isDeliveryReceiptRequested|Boolean|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|isDraft|Boolean|Indica se a mensagem é um rascunho. Uma mensagem é um rascunho quando ela ainda não foi enviada.|
|isRead|Boolean|Indica se a mensagem foi lida.|
|isReadReceiptRequested|Boolean|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a mensagem foi alterada pela última vez.|
|meetingMessageType|meetingMessageType| O tipo de mensagem de evento: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTenativelyAccepted`, `meetingDeclined`.|
|parentFolderId|String|O identificador exclusivo para a mailFolder pai da mensagem.|
|receivedDateTime|DateTimeOffset|A data e a hora em que a mensagem foi recebida.|
|replyTo|Coleção [recipient](recipient.md)|Os endereços de email a serem usados ao responder.|
|sender|[recipient](recipient.md)|A conta que é realmente usada para gerar a mensagem. Na maioria dos casos, esse valor é o mesmo da propriedade **from**. Você pode definir essa propriedade como um valor diferente ao enviar uma mensagem de uma [caixa de correio compartilhada](/exchange/collaboration/shared-mailboxes/shared-mailboxes), [ou ao enviar uma mensagem como um delegado](/graph/outlook-share-delegate-calendar.md). De qualquer forma, o valor deve corresponder à caixa de correio real que foi usada. Saiba mais sobre [como definir as propriedades from e sender](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) de uma mensagem.|
|sentDateTime|DateTimeOffset|A data e a hora em que a mensagem foi enviada.|
|subject|String|O assunto da mensagem.|
|toRecipients|Coleção [recipient](recipient.md)|Os destinatários Para: da mensagem.|
|uniqueBody|[itemBody](itembody.md)|A parte do corpo da mensagem que é exclusiva para a mensagem atual.|
|webLink|String|O URL para abrir a mensagem no Outlook na Web.<br><br>Você pode acrescentar um argumento ispopout ao final da URL para alterar como a mensagem é exibida. Se ispopout não houver presente ou estiver definido como 1, a mensagem será mostrada em uma janela pop-up. Se a entrada for definida como 0, o navegador mostrará a mensagem no painel de revisão do Outlook na Web.<br><br>A mensagem será aberta no navegador se você estiver conectado à sua caixa de correio através do Outlook na Web. Você será solicitado a fazer o login, se ainda não estiver conectado com o navegador.<br><br>Este URL não pode ser acessado a partir de um iFrame.|

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|attachments|Coleção [attachment](attachment.md)| Somente leitura. Anulável.|
|event|[event](event.md)| O evento associado à mensagem de evento. A pressuposição dos participantes ou recursos da sala é que o Atendedor de Calendário esteja definido para atualizar automaticamente o calendário com um evento quando mensagens de evento de solicitação de reunião chegarem. Propriedade de navegação.  Somente leitura.|
|extensions|[extension](extension.md) collection|A coleção de extensões abertas definidas para eventMessage. Somente leitura. Anulável.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a eventMessage. Somente leitura. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de valor único definidas para a eventMessage. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso  

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.message",
  "optionalProperties": [
    "attachments",
    "event",
    "extensions",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "baseType": "microsoft.graph.message",
  "@odata.type": "microsoft.graph.eventMessage",
  "@odata.annotations": [
    {
      "property": "event",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "insertable": false,
        "searchable": false,
        "updatable": false
      }
    }
  ]
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
  "event": { "@odata.type": "microsoft.graph.event" },
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageHeaders": [{"@odata.type": "microsoft.graph.internetMessageHeader"}],
  "internetMessageId": "String",
  "isDelegated": true,
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "DateTimeOffset",
  "meetingMessageType": "String",
  "parentFolderId": "string",
  "receivedDateTime": "DateTimeOffset",
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "DateTimeOffset",
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "string"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "eventMessage resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

