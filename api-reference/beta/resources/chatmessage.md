---
title: Tipo de recurso chatMessage
description: Representa uma mensagem de chat individual dentro de uma entidade de canal ou chat. A mensagem pode ser uma mensagem raiz ou parte de um thread que seja definido pela propriedade **replyToId** na mensagem.
localization_priority: Priority
ms.openlocfilehash: a74f422c6bf60e1293d8620b440152be77dacdc7
ms.sourcegitcommit: cd4bdb2c6754b1d5658e68909ea6c219466da6df
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2019
ms.locfileid: "30644318"
---
# <a name="chatmessage-resource-type"></a>Tipo de recurso chatMessage

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma mensagem de chat individual dentro de uma entidade de [canal](channel.md) ou chat. A mensagem pode ser uma mensagem raiz ou parte de um thread que seja definido pela propriedade **replyToId** na mensagem.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[List Channel messages](../api/channel-list-messages.md) | [chatmessage](chatmessage.md) collection | Obtenha uma lista de todas as mensagens raiz em um canal.|
|[Get Channel message](../api/channel-get-message.md) | [chatmessage](chatmessage.md) | Obtenha uma mensagem raiz única de um canal.|
|[List replies to a message](../api/channel-list-messagereplies.md) | [chatmessage](chatmessage.md) collection| Obtenha a lista de todas as respostas a uma mensagem no canal.|
|[Get a reply to a message](../api/channel-get-messagereply.md) | [chatmessage](chatmessage.md)| Obtenha uma resposta a uma mensagem única em um canal.|
|[Enviar uma mensagem em um canal](../api/channel-post-chatmessage.md) | [chatmessage](chatmessage.md)| Crie uma nova mensagem de nível superior em um canal.|
|[Responder a uma mensagem em um canal](../api/channel-post-messagereply.md) | [chatmessage](chatmessage.md)| Responder a uma mensagem existente em um canal.|


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|id|String| Somente leitura. ID única da mensagem.|
|replyToId| string | ID da mensagem pai/raiz do thread. |
|from|[identitySet](identityset.md)| Somente leitura. Detalhes do remetente da mensagem.|
|etag| string | O número de versão da mensagem. |
|messageType|String|Os valores de tipo de mensagem com suporte atualmente são: message, chatEvent, Typing.|
|createdDateTime|dateTimeOffset|Somente leitura. Carimbo de data/hora de quando a mensagem foi criada.|
|lastModifiedDateTime|dateTimeOffset|Somente leitura. Carimbo de data/hora de quando a mensagem foi editada/atualizada.|
|deleted|Boolean|Indica se uma mensagem foi excluída de modo reversível.|
|deletedDateTime|dateTimeOffset|Somente leitura. Carimbo de data/hora em que a mensagem foi excluída. |
|Assunto|string|Linha de assunto da mensagem. Opcional.|
|corpo|[itemBody](itembody.md)|Representação de texto sem formatação/HTML do conteúdo da mensagem. Retorna o texto sem formatação por padrão, o aplicativo pode escolher HTML como parte de um parâmetro de consulta|
|summary|string|Texto de resumo da mensagem que poderia ser usado para notificações por push e modos de exibição de resumo ou de fallback|
|mentions|[chatMessageMention](chatmention.md) collection| Lista de entidades mencionada na mensagem. Atualmente, dá suporte a usuário, bot, equipe, canal.|
|importância| string | A importância da mensagem: Normal, Alta.|
|reactions| [chatMessageReaction](chatreaction.md) collection | Reações para essa mensagem (por exemplo, Curtir)|
|locale|string|Localidade da mensagem definida pelo cliente|
|attachments|[chatMessageAttachment](chatattachment.md) collection |Arquivos anexos. No momento, os anexos são somente leitura, não há suporte para o envio de anexos. |


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
  "isDeleted": "boolean",
  "deletedDateTime": "string (timestamp)",
  "subject": "string",
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "summary": "string",
  "attachments": [{"@odata.type": "microsoft.graph.chatMessageAttachment"}],
  "mentions": [{"@odata.type": "microsoft.graph.chatMessageMention"}],
  "importance": "string",
  "reactions": [{"@odata.type": "microsoft.graph.chatMessageReaction"}],
  "locale": "string"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
