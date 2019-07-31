---
title: tipo de recurso chatMessageReaction
description: 'Representa uma reação a uma entidade chat. '
localization_priority: Normal
doc_type: resourcePageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: e1193e65697187f705f2758c2c195e5519326dc0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973981"
---
# <a name="chatmessagereaction-resource-type"></a>tipo de recurso chatMessageReaction

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma reação a uma entidade [chat](chatmessage.md) . 

Uma entidade do tipo `chatMessageReaction` é retornada como parte da API [obter mensagem de canal](../api/channel-get-message.md) , como parte da entidade [chat](chatmessage.md) .

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|reactiontype|String|Os valores com `like`suporte `angry`são `sad`, `laugh` `heart`,, `surprised`,. |
|user|[identitySet](identityset.md)|O usuário que reajam à mensagem.|

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
