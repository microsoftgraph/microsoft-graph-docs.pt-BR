---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual dentro de uma entidade de canal ou chat. A mensagem pode ser uma mensagem raiz ou parte de um thread que seja definido pela propriedade **replyToId** na mensagem.
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: ea21d57134643c83406f449ee7cdad192afc0326
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2019
ms.locfileid: "34709408"
---
# <a name="chatmessage-resource-type"></a>Tipo de recurso chatMessage

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma mensagem de bate-papo individual em um [canal](channel.md) ou [bate-papo](chat.md).
A mensagem pode ser uma mensagem raiz ou parte de um thread definido pela propriedade **replyToId** na mensagem.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List Channel messages](../api/channel-list-messages.md) | [chatmessage](chatmessage.md) collection | Obtenha uma lista de todas as mensagens raiz em um canal.|
|[Get Channel message](../api/channel-get-message.md) | [chatmessage](chatmessage.md) | Obtenha uma mensagem raiz única de um canal.|
|[List replies to a message](../api/channel-list-messagereplies.md) | [chatmessage](chatmessage.md) collection| Obtenha a lista de todas as respostas a uma mensagem no canal.|
|[Get a reply to a message](../api/channel-get-messagereply.md) | [chatmessage](chatmessage.md)| Obtenha uma resposta a uma mensagem única em um canal.|
|[Criar uma chatMessage em um canal](../api/channel-post-messages.md) | [chatmessage](chatmessage.md)| Crie uma nova mensagem de nível superior em um canal.|
|[Criar uma resposta chatMessage em um canal](../api/channel-post-messagereply.md) | [chatmessage](chatmessage.md)| Responder a uma mensagem existente em um canal.|
|[Listar mensagens em um bate-papo](../api/chat-list-messages.md)  | [chatMessage](../resources/chatmessage.md) | Receba mensagens em um bate-papo de um para um ou de grupo. |
|[Receba uma mensagem no bate-papo](../api/chat-get-message.md)  | [chatMessage](../resources/chatmessage.md) | Receba uma única mensagem em um bate-papo. |

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID exclusivo da mensagem.|
|replyToId| cadeia de caracteres | Somente leitura. ID da mensagem pai/raiz do thread. (Aplica-se apenas a mensagens em canais e não em bate-papos) |
|from|[identitySet](identityset.md)| Somente leitura. Detalhes do remetente da mensagem.|
|etag| cadeia de caracteres | Somente leitura. O número de versão da mensagem. |
|messageType|chatMessageType|O tipo de mensagem. Os valores possíveis são: `message`.|
|createdDateTime|dateTimeOffset|Somente leitura. Carimbo de data/hora de quando a mensagem foi criada.|
|lastModifiedDateTime|dateTimeOffset|Somente leitura. Carimbo de data/hora de quando a mensagem foi editada/atualizada.|
|deletedDateTime|dateTimeOffset|Somente leitura. Carimbo de hora em que a mensagem foi excluída ou nulo se não foi excluído. |
|assunto|cadeia de caracteres| O assunto da mensagem, em texto simples.|
|corpo|[itemBody](itembody.md)|Representação de texto sem formatação/HTML do conteúdo da mensagem. A representação é especificada pelo contentType dentro do corpo. O conteúdo está sempre em HTML se a mensagem contiver um [chatMessageMention](chatmessagemention.md). |
|summary|cadeia de caracteres| Texto de resumo da mensagem que pode ser usado para notificações por push e visualizações resumidas ou de fallback. Aplica-se apenas às mensagens de canal, não às mensagens de bate-papo. |
|attachments|[chatMessageAttachment](chatmessageattachment.md) collection |Arquivos anexos. No momento, os anexos são somente leitura, não há suporte para o envio de anexos. |
|mentions|[chatMessageMention](chatmessagemention.md) collection| Lista de entidades mencionada na mensagem. Atualmente, dá suporte a usuário, bot, equipe, canal.|
|importância| chatMessageImportance | A importância da mensagem. Os valores possíveis são: `normal`, `high`, `urgent`.|
|reactions| [chatMessageReaction](chatmessagereaction.md) collection | Reações para esta mensagem (por exemplo, Curtir).|
|localidade|cadeia de caracteres|Local da mensagem definido pelo cliente.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deleted",
    "deletedDateTime",
    "attachments",
    "importance",
    "reactions",
    "mentions",
    "subject",
    "summary"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessage"
}-->

```json
{
  "id": "string (identifier)",
  "replyToId": "string (identifier)",
  "from": {"@odata.type": "microsoft.graph.identitySet"},
  "etag": "string",
  "messageType": "string",
  "createdDateTime": "string (timestamp)",
  "lastModifiedDateTime": "string (timestamp)",
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "policyViolation": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string",
  "deleted": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat message resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
