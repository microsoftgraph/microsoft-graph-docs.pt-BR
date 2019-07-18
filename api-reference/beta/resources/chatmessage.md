---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual dentro de uma entidade de canal ou chat. A mensagem pode ser uma mensagem raiz ou parte de um thread que seja definido pela propriedade **replyToId** na mensagem.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
ms.openlocfilehash: 99e69bd51a661b67fd4cb325fffe80db91214714
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778667"
---
# <a name="chatmessage-resource-type"></a>Tipo de recurso chatMessage

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma mensagem de bate-papo individual em um [canal](channel.md) ou [bate-papo](chat.md).
A mensagem pode ser uma mensagem raiz ou parte de um thread definido pela propriedade **replyToId** na mensagem.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List Channel messages](../api/channel-list-messages.md) | [chatMessage](chatmessage.md) collection | Lista de todas as mensagens raiz em um canal.|
|[Get Channel message](../api/channel-get-message.md) | [chatMessage](chatmessage.md) | Obtenha uma mensagem raiz única de um canal.|
|[List replies to a message](../api/channel-list-messagereplies.md) | [chatMessage](chatmessage.md) collection| Lista de todas as respostas a uma mensagem no canal.|
|[Get a reply to a message](../api/channel-get-messagereply.md) | [chatMessage](chatmessage.md)| Obtenha uma resposta a uma mensagem única em um canal.|
|[Criar chat em um canal](../api/channel-post-messages.md) | [chatMessage](chatmessage.md)| Crie uma nova mensagem de nível superior em um canal.|
|[Responder a uma mensagem em um canal](../api/channel-post-messagereply.md) | [chatMessage](chatmessage.md)| Responder a uma mensagem existente em um canal.|
|[Listar mensagens em um bate-papo](../api/chatmessage-list.md)  | [chatMessage](../resources/chatmessage.md) | Listar mensagens em um bate-papo de grupo ou 1:1. |
|[Receba uma mensagem no bate-papo](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | Receba uma única mensagem em um bate-papo. |
|[Listar todas as imagens hospedadas](../api/chatmessagehostedimage-list-hostedimages.md) | coleção [hostedImage](../resources/chatmessagehostedimage.md)| Obter todas as imagens hospedadas em uma mensagem.|
|[Obter imagem hospedada](../api/chatmessagehostedimage-get.md) | [hostedImage](../resources/chatmessagehostedimage.md) | Obter uma imagem hospedada de uma mensagem.|
|[Obter bytes de imagem hospedado](../api/chatmessagehostedimage-getbytes.md) | dados de imagem binária | Obtém dados de imagem binária de uma imagem hospedada de uma mensagem.|

## <a name="properties"></a>Propriedades

| Propriedade   | Tipo |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID exclusiva da mensagem.|
|replyToId| cadeia de caracteres | Somente leitura. ID da mensagem pai/raiz do thread. (Aplica-se apenas a mensagens em canais e não em bate-papos) |
|from|[identitySet](identityset.md)| Somente leitura. Detalhes do remetente da mensagem.|
|etag| cadeia de caracteres | Somente leitura. O número de versão da mensagem. |
|messageType|chatMessageType|O tipo de mensagem. Os valores possíveis são: `message`.|
|createdDateTime|dateTimeOffset|Somente leitura. Carimbo de data/hora de quando a mensagem foi criada.|
|lastModifiedDateTime|dateTimeOffset|Somente leitura. Carimbo de data/hora de quando a mensagem é criada ou editada, incluindo quando uma resposta é feita (se é uma mensagem raiz em um canal) ou uma reação é adicionada ou removida. |
|deletedDateTime|dateTimeOffset|Somente leitura. Carimbo de hora em que a mensagem foi excluída ou nulo se não foi excluído. |
|assunto|string| O assunto da mensagem, em texto simples.|
|corpo|[itemBody](itembody.md)|Representação de texto sem formatação/HTML do conteúdo da mensagem. A representação é especificada pelo contentType dentro do corpo. O conteúdo está sempre em HTML se a mensagem contiver um [chatMessageMention](chatmessagemention.md). |
|summary|string| Texto de resumo da mensagem que pode ser usado para notificações por push e visualizações resumidas ou de fallback. Aplica-se apenas às mensagens de canal, não às mensagens de bate-papo. |
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
