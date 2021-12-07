---
title: Tipo de recurso channelSetAsFavoriteByDefaultEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre um canal definido como favorito por padrão.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 011414c5e0030bfcc0936c28de3a6bda1049052e
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322337"
---
# <a name="channelsetasfavoritebydefaulteventmessagedetail-resource-type"></a>Tipo de recurso channelSetAsFavoriteByDefaultEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre um [canal](../resources/channel.md) que o sinalizador `isFavoriteByDefault` está definido.

Um **canal** fica visível para todos os membros da equipe na lista de **canais** em uma [equipe se](../resources/team.md) o sinalizador for `isFavoriteByDefault` `true` .


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
  "@odata.type": "microsoft.graph.channelSetAsFavoriteByDefaultEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelSetAsFavoriteByDefaultEventMessageDetail",
  "channelId": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre um **canal** definido como favorito por padrão](/graph/system-messages/#channel-set-as-favorite-by-default)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
