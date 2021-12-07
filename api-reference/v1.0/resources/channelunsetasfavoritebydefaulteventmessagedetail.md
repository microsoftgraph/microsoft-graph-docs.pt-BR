---
title: Tipo de recurso channelUnsetAsFavoriteByDefaultEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre um canal desajustado como favorito por padrão.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4f9dab965db79fe08086af3327d727ac97713f3f
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322322"
---
# <a name="channelunsetasfavoritebydefaulteventmessagedetail-resource-type"></a>Tipo de recurso channelUnsetAsFavoriteByDefaultEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre um [canal](../resources/channel.md) que o sinalizador `isFavoriteByDefault` não está.

Um **canal** não será mais visível para todos os membros da equipe na lista **de** canais em uma [equipe](../resources/team.md) se o sinalizador `isFavoriteByDefault` for `false` .

Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|channelId|String|Identificador exclusivo do **canal**.|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelUnsetAsFavoriteByDefaultEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelUnsetAsFavoriteByDefaultEventMessageDetail",
  "channelId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre um **canal** não sereado como favorito por padrão](/graph/system-messages/#channel-unset-as-favorite-by-default)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
