---
title: Tipo de recurso chatMessageReaction
description: 'Representa uma reação a uma entidade chatMessage. '
ms.localizationpriority: medium
doc_type: resourcePageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: 7eb1aad41417bcbde320c04f5b93b466430911fa
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109378"
---
# <a name="chatmessagereaction-resource-type"></a>Tipo de recurso chatMessageReaction

Namespace: microsoft.graph

Representa uma reação a uma [entidade chatMessage.](chatmessage.md) 

Uma entidade de tipo é retornada como parte da API de mensagem get `chatMessageReaction` [channel,](../api/chatmessage-get.md) como parte da [entidade chatMessage.](chatmessage.md)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|reactionType|String|Os valores suportados `like` são , , , , , `angry` `sad` `laugh` `heart` `surprised` . |
|usuário|[chatMessageReactionIdentitySet](chatmessagereactionidentityset.md)|O usuário que reagia à mensagem.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageReaction",
  "baseType": null
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "reactionType": "String",
  "user": {"@odata.type": "microsoft.graph.chatMessageReactionIdentitySet"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessageReaction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


