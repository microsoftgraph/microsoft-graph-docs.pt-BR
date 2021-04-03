---
title: Tipo de recurso chatMessageReaction
description: 'Representa uma reação a uma entidade chatMessage. '
localization_priority: Normal
doc_type: resourcePageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: e696069b9913b89fafea178c7cf95e099e288c46
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582873"
---
# <a name="chatmessagereaction-resource-type"></a>Tipo de recurso chatMessageReaction

Namespace: microsoft.graph

Representa uma reação a uma [entidade chatMessage.](chatmessage.md) 

Uma entidade de tipo é retornada como parte da API de mensagem get `chatMessageReaction` [channel,](../api/chatmessage-get.md) como parte da [entidade chatMessage.](chatmessage.md)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|reactionType|String|Os valores suportados `like` são , , , , , `angry` `sad` `laugh` `heart` `surprised` . |
|usuário|[identitySet](identityset.md)|O usuário que reagia à mensagem.|

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
  "user": {"@odata.type": "microsoft.graph.identitySet"}
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


