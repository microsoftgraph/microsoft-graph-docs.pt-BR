---
title: tipo de recurso de mensagem
description: Uma mensagem em uma pasta da caixa de correio.
author: abheek-das
ms.localizationpriority: high
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 783680decf42e15f5814b8edc396a16aca961d15
ms.sourcegitcommit: 1e8ba243e77ca344e267f16dfeb321fb5a7463e8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2022
ms.locfileid: "64733175"
---
# <a name="message-resource-type"></a>tipo de recurso de mensagem

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma mensagem em uma pasta da caixa de correio.

O número máximo de destinatários incluídos nas propriedades **toRecipients**, **ccRecipients** e **bccRecipients** de apenas uma mensagem de e-mail enviada de uma caixa de correio do Exchange Online é 500. Para obter mais informações, consulte [limites de envio](/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#sending-limits).

Esse recurso permite:

- Adicionar seus próprios dados como cabeçalhos personalizados de mensagens da Internet. Adicionar cabeçalhos personalizados somente ao criar uma mensagem e nomes que começam com"x-". Após a mensagem ter sido enviada, não será possível alterar os cabeçalhos. Para obter os cabeçalhos de uma mensagem, aplique o parâmetro de consulta `$select` em uma operação [get message](../api/message-get.md).
- Adicionar seus próprios dados como propriedades personalizadas como [extensions](/graph/extensibility-overview).
- Assinar as [notificações de alteração](/graph/webhooks).
- Usar a [consulta delta](/graph/delta-query-overview) para controlar adições, exclusões e atualizações incrementais oferecendo uma função [delta](../api/message-delta.md).

## <a name="methods"></a>Métodos

| Método | Tipo de retorno |Descrição|
|:-------|:------------|:----------|
|[Listar mensagens](../api/user-list-messages.md) |Coleção [message](message.md) | Obter todas as mensagens na caixa de correio do usuário conectado (incluindo as pastas Itens Excluídos e Email Secundário). |
|[Criar mensagem](../api/user-post-messages.md) | [message](message.md) | Criar um rascunho de uma nova mensagem. |
|[Obter mensagem](../api/message-get.md) | [message](message.md) |Ler propriedades e relações do objeto mensage.|
|[Update](../api/message-update.md) | [message](message.md) |Atualizar o objeto message. |
|[Delete](../api/message-delete.md) | None |Excluir o objeto message. |
|[copy](../api/message-copy.md)|[Message](message.md)|Copiar uma mensagem para uma pasta.|
|[createForward](../api/message-createforward.md)|[Mensagem](message.md)|Crie uma mensagem de encaminhamento de rascunho para incluir um comentário ou atualizar todas as propriedades da mensagem em uma chamada **createForward**. Você pode [atualizar](../api/message-update.md) ou [enviar](../api/message-send.md) o rascunho.|
|[createReply](../api/message-createreply.md)|[Mensagem](message.md)|Crie um rascunho de uma mensagem de resposta para incluir um comentário ou atualizar todas as propriedades da mensagem em uma chamada **createReply**. Você pode [atualizar](../api/message-update.md) ou [enviar](../api/message-send.md) o rascunho.|
|[createReplyAll](../api/message-createreplyall.md)|[Mensagem](message.md)|Crie um rascunho de uma mensagem de resposta a todos para incluir um comentário ou atualizar as propriedades da mensagem, tudo em uma chamada **createReplyAll**. Você pode [atualizar](../api/message-update.md) ou [enviar](../api/message-send.md) o rascunho.|
|[delta](../api/message-delta.md)|Coleção [message](message.md)| Obtenha um conjunto de mensagens que foram adicionadas, excluídas ou atualizadas em uma pasta especificada.|
|[forward](../api/message-forward.md)|Nenhum|Encaminhe uma mensagem, adicione um comentário ou modifique todas as propriedades atualizáveis em uma única chamada **forward**. A mensagem é então salva na pasta Itens Enviados.|
|[move](../api/message-move.md)|[Message](message.md)|Mover a mensagem para uma pasta. Isso cria uma nova cópia da mensagem na pasta de destino.|
|[reply](../api/message-reply.md)|Nenhum|Responda ao remetente de uma mensagem, adicione um comentário ou modifique todas as propriedades atualizáveis em uma única chamada **reply**. A mensagem é então salva na pasta Itens Enviados.|
|[replyAll](../api/message-replyall.md)|Nenhum|Responda a todos os destinatários de uma mensagem especificando um comentário e modificando quaisquer propriedades atualizáveis para a resposta, tudo usando o método **replyAll**. A mensagem é então salva na pasta Itens Enviados.|
|[send](../api/message-send.md)|Nenhum|Envia um rascunho de mensagem anteriormente criado. A mensagem é então salva na pasta Itens Enviados.|
|[unsubscribe](../api/message-unsubscribe.md)|Nenhum|Envie uma mensagem usando os dados e o endereço especificados no primeiro comando mailto no cabeçalho List-Unsubscribe.|
|**Anexos**| | |
|[Listar anexos](../api/message-list-attachments.md) |Coleção [Attachment](attachment.md)| Obtenha todos os anexos em uma mensagem.|
|[Add attachment](../api/message-post-attachments.md) |[Attachment](attachment.md)| Adicione um novo anexo a uma mensagem postando na coleção attachments.|
|**Extensões abertas**| | |
|[Criar extensão aberta](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| Crie uma extensão aberta e adicione propriedades personalizadas a uma instância nova ou existente de um recurso.|
|[Obter extensão aberta](../api/opentypeextension-get.md) |Coleção [openTypeExtension](opentypeextension.md)| Obtenha uma extensão aberta identificada pelo nome da extensão.|
|**Extensões de esquema**| | |
|[Adicionar valores de extensões de esquema](/graph/extensibility-schema-groups) || Cria uma definição para a extensão de esquema e usa-a para adicionar dados digitados personalizados a um recurso.|
|**Propriedades estendidas**| | |
|[Criar uma propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[message](message.md)  |Criar uma ou mais propriedades estendidas de valor único em uma mensagem nova ou existente.   |
|[Obter mensagem com propriedade estendida de valor único](../api/singlevaluelegacyextendedproperty-get.md)  | [message](message.md) | Obter mensagens que contenham uma propriedade estendida de valor único usando `$expand` ou `$filter`. |
|[Criar propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [message](message.md) | Criar uma ou mais propriedades estendidas de vários valores em uma mensagem nova ou existente.  |
|[Obter mensagem com propriedade estendida de vários valores](../api/multivaluelegacyextendedproperty-get.md)  | [message](message.md) | Obter uma mensagem que contenha uma propriedade estendida de vários valores usando `$expand`. |

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
|bccRecipients|Coleção [recipient](recipient.md)|Os destinatários Cco: da mensagem.|
|body|[itemBody](itembody.md)|O corpo da mensagem. Pode estar no formato HTML ou no formato de texto. Saiba mais sobre [HTML seguro no corpo da mensagem](/graph/outlook-create-send-messages#reading-messages-with-control-over-the-body-format-returned).|
|bodyPreview|String|Os primeiros 255 caracteres do corpo da mensagem. Está no formato de texto. Se a mensagem contiver instâncias de [menção](mention.md), essa propriedade também conteria uma concatenação dessas menções. |
|categories|String collection|As categorias associadas à mensagem. Cada categoria corresponde à propriedade **displayName** de uma [outlookCategory](outlookcategory.md) definida para o usuário. |
|ccRecipients|Coleção [recipient](recipient.md)|Os destinatários Cc: da mensagem.|
|changeKey|String|A versão da mensagem.|
|conversationId|String|A ID da conversa à qual o email pertence.|
|conversationIndex|Edm.Binary|Indica a posição da mensagem dentro da conversa.|
|createdDateTime|DateTimeOffset|A data e a hora em que a mensagem foi criada. <br><br> As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|flag|[followupFlag](followupflag.md)|O valor do sinalizador que indica o status, a data de início, a data de conclusão ou a data de finalização da mensagem.|
|from|[recipient](recipient.md)|O proprietário da caixa de correio da qual a mensagem foi enviada. Na maioria dos casos, esse valor é o mesmo que o da propriedade **remetente**, exceto para cenários de compartilhamento ou delegação. O valor deve corresponder à caixa de correio real que foi usada. Saiba mais sobre [como definir as propriedades from e sender](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) de uma mensagem.|
|hasAttachments|Booliano|Indica se a mensagem tem anexos. Esta propriedade não inclui anexos em linha, portanto, se uma mensagem contém somente anexos em linha, essa propriedade é falsa. Para verificar a existência de anexos em linha, analise a propriedade **body** para procurar um atributo `src`, como `<IMG src="cid:image001.jpg@01D26CD8.6C05F070">`. |
|id|Cadeia de caracteres| Identificador exclusivo da mensagem. [!INCLUDE [outlook-beta-id](../../includes/outlook-immutable-id.md)] Somente leitura. |
|importância|importância| A importância da mensagem. Os valores possíveis são `low`, `normal` e `high`.|
|inferenceClassification|inferenceClassificationType| A classificação da mensagem para o usuário, com base na relevância deduzida ou na importância, ou em uma substituição explícita. Os valores possíveis são: `focused` ou `other`.|
|internetMessageHeaders | Coleção [internetMessageHeader](internetmessageheader.md) | Uma coleção de cabeçalhos de mensagens definidos por [RFC5322](https://www.ietf.org/rfc/rfc5322.txt). O conjunto inclui cabeçalhos de mensagens que indicam o caminho de rede adotado por uma mensagem do remetente para o destinatário. Também pode conter cabeçalhos de mensagens personalizados com dados do aplicativo para a mensagem. <br><br> Retornado apenas na aplicação de uma `$select` opção de consulta. Somente leitura.|
|internetMessageId | String | O ID da mensagem no formato especificado por [RFC5322](https://www.ietf.org/rfc/rfc5322.txt). Atualizável somente se **isDraft** for verdadeiro.|
|isDeliveryReceiptRequested|Boolean|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|isDraft|Boolean|Indica se a mensagem é um rascunho. Uma mensagem é um rascunho quando ela ainda não foi enviada.|
|isRead|Boolean|Indica se a mensagem foi lida.|
|isReadReceiptRequested|Boolean|Indica se uma confirmação de leitura foi solicitada para a mensagem.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a mensagem foi alterada pela última vez. <br><br> As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|mentionsPreview|[mentionsPreview](mentionspreview.md)|Informações sobre menções na mensagem. Ao processar uma solicitação `GET` /messages, o servidor define essa propriedade e a inclui na resposta por padrão. O servidor retornará null se não houver menções na mensagem. Opcional. |
|parentFolderId|String|O identificador exclusivo para a mailFolder pai da mensagem.|
|receivedDateTime|DateTimeOffset|A data e a hora em que a mensagem foi recebida. <br><br> As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|replyTo|Coleção [recipient](recipient.md)|Os endereços de email a serem usados ao responder.|
|sender|[recipient](recipient.md)|A conta que é realmente usada para gerar a mensagem. Na maioria dos casos, esse valor é o mesmo da propriedade **from**. Você pode definir essa propriedade como um valor diferente ao enviar uma mensagem de uma [caixa de correio compartilhada](/exchange/collaboration/shared-mailboxes/shared-mailboxes), [ou ao enviar uma mensagem como um delegado](/graph/outlook-share-delegate-calendar.md). De qualquer forma, o valor deve corresponder à caixa de correio real que foi usada. Saiba mais sobre [como definir as propriedades from e sender](/graph/outlook-create-send-messages#setting-the-from-and-sender-properties) de uma mensagem.|
|sentDateTime|DateTimeOffset|A data e a hora em que a mensagem foi enviada. <br><br> As informações de data e hora usam o formato ISO 8601 e estão sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`.|
|assunto|String|O assunto da mensagem.|
|toRecipients|Coleção [recipient](recipient.md)|Os destinatários Para: da mensagem.|
|uniqueBody|[itemBody](itembody.md)|A parte do corpo da mensagem que é exclusiva para a mensagem atual. **uniqueBody** não é fornecido por padrão, mas pode ser recuperado por uma determinada mensagem pelo uso da consulta `?$select=uniqueBody`. Pode estar no formato HTML ou no formato de texto.|
|unsubscribeData|String|As entradas válidas analisadas no cabeçalho List-Unsubscribe.  Esses são os dados para o comando mail no cabeçalho List-Unsubscribe, se a propriedade UnsubscribeEnabled for true.|
|unsubscribeEnabled|Booliano|Indica se a mensagem está habilitada para o cancelamento da assinatura.  valueTrue se o cabeçalho list-Unsubscribe estiver em conformidade com o rfc-2369.|
|webLink|String|O URL para abrir a mensagem no Outlook na Web.<br><br>Você pode anexar um argumento ispopout ao final do URL para alterar a forma como a mensagem é exibida. Se ispopout não estiver presente ou se estiver definido como 1, a mensagem será exibida em uma janela popout. Se ispopout estiver definido como 0, o navegador mostrará a mensagem no painel de revisão do Outlook na Web.<br><br>A mensagem será aberta no navegador se você estiver conectado à sua caixa de correio através do Outlook na Web. Você será solicitado a fazer o login, se ainda não estiver conectado com o navegador.<br><br>Este URL não pode ser acessado a partir de um iFrame.|

## <a name="relationships"></a>Relações

| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
|attachments|Coleção [Attachment](attachment.md)|Os anexos [fileAttachment](fileattachment.md) e [itemAttachment](itemattachment.md) da mensagem.|
|extensions|Coleção [Extension](extension.md)| A coleção de extensões abertas definidas para a mensagem. Anulável.|
|menções|Coleção [mention](mention.md) | Uma coleção de menções na mensagem, ordenada pelo **createdDateTime**, do mais novo para o mais antigo. Por padrão, um `GET` /messages não retorna essa propriedade, a menos que você aplique `$expand` à propriedade.|
|multiValueExtendedProperties|Coleção [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de vários valores definidas para a mensagem. Anulável.|
|singleValueExtendedProperties|Coleção [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)| A coleção de propriedades estendidas de valor único definidas para a mensagem. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "optionalProperties": [
    "attachments",
    "extensions",
    "singleValueExtendedProperties",
    "multiValueExtendedProperties",
    "mentions",

    "internetMessageHeaders"
  ],
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
  "conversationIndex": "String (binary)",
  "createdDateTime": "String (timestamp)",
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "internetMessageHeaders": [{"@odata.type": "microsoft.graph.internetMessageHeader"}],
  "internetMessageId": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "mentionsPreview": {"@odata.type": "microsoft.graph.mentionsPreview"},
  "parentFolderId": "string",
  "receivedDateTime": "String (timestamp)",
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "unsubscribeData": "string",
  "unsubscribeEnabled": true,
  "webLink": "string",

  "attachments": [{"@odata.type": "microsoft.graph.attachment"}],
  "extensions": [{"@odata.type": "microsoft.graph.extension"}],
  "mentions": [{"@odata.type": "microsoft.graph.mention"}],
  "multiValueExtendedProperties": [{"@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"}],
  "singleValueExtendedProperties": [{"@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"}]
}
```

## <a name="see-also"></a>Confira também

- [Get mailbox settings](../api/user-get-mailboxsettings.md)
- [Atualizar configurações da caixa de correio](../api/user-update-mailboxsettings.md)
- [Usar a consulta delta para controlar alterações nos dados do Microsoft Graph](/graph/delta-query-overview)
- [Obter as alterações incrementais para as mensagens em uma pasta](/graph/delta-query-messages)
- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando as extensões do esquema](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}



