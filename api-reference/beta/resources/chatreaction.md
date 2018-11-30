---
title: tipo de recurso de chatMessageReaction
description: 'Representa uma reação a uma entidade chatMessage. '
ms.openlocfilehash: 1ad1f7948405a8891ec9aa13065b71108e9c47c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040849"
---
# <a name="chatmessagereaction-resource-type"></a>tipo de recurso de chatMessageReaction

Representa uma reação a uma entidade [chatMessage](chatmessage.md) . 

Uma entidade do tipo `chatMessageReaction` é retornado como parte de [receber mensagens de canal](../api/channel-get-message.md) API, como parte da entidade [chatMessage](chatmessage.md) .

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|reactionType|string| O tipo de reação. Valores planejados incluem: <br><ul><li>Como - como uma mensagem, conteúdo fica em branco nesse caso.</li><li>Emoji - Emoji reação. Conteúdo é definido como o valor unicode do emoji.</li><li>Rótulo - o conteúdo é definido como a cadeia de caracteres no rótulo.</li></ul>|
|createdDateTime|dateTimeOffset|Carimbo de hora UTC da mensagem raiz no formato ISO 8601.|
|user|identitySet|O usuário que reacted à mensagem.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "content"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageReaction"
}-->

```json
{
  "reactionType": "string ",
  "createdDateTime": "string (timestamp)",
  "user": {"@odata.type": "microsoft.graph.identitySet"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message reaction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
