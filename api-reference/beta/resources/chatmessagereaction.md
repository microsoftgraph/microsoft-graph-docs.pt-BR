---
title: tipo de recurso chatMessageReaction
description: 'Representa uma reação a uma entidade chat. '
localization_priority: Normal
ms.openlocfilehash: 5020653ef02c1604aece46f3ff2c7ea1c82a75ec
ms.sourcegitcommit: 953895b28b6bae6e17eead938565fde289c49ef7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/05/2019
ms.locfileid: "31481381"
---
# <a name="chatmessagereaction-resource-type"></a>tipo de recurso chatMessageReaction

Representa uma reação a uma entidade [chat](chatmessage.md) . 

Uma entidade do tipo `chatMessageReaction` é retornada como parte da API [Get Channel messages](../api/channel-get-message.md) , como parte da entidade [chat](chatmessage.md) .

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|reactiontype|string| O tipo de reação. Os valores planejados incluem: <br><ul><li>Semelhante a uma mensagem, o conteúdo está em branco neste caso.</li><li>Emoji-reação de Emoji. O conteúdo é definido para o valor Unicode do emoji.</li><li>Rótulo-o conteúdo é definido como a cadeia de caracteres no rótulo.</li></ul>|
|createdDateTime|dateTimeOffset|Carimbo de data/hora UTC da mensagem raiz no formato ISO-8601.|
|user|identitySet|O usuário que reajam à mensagem.|

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
