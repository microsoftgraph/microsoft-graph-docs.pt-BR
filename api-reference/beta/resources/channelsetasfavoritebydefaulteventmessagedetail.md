---
title: Tipo de recurso channelSetAsFavoriteByDefaultEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre um canal definido como favorito por padrão.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 35ddf629e82b55bb3ab475d65d6078e4607392a1
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/22/2021
ms.locfileid: "53535659"
---
# <a name="channelsetasfavoritebydefaulteventmessagedetail-resource-type"></a>Tipo de recurso channelSetAsFavoriteByDefaultEventMessageDetail

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os detalhes de uma mensagem de evento sobre um canal que o sinalizador 'isFavoriteByDefault' está definido.
Um canal fica visível para todos os membros da equipe na lista de canais em uma equipe se ele tiver o sinalizador 'isFavoriteByDefault' definido como true.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|channelId|Cadeia de Caracteres|Identificador exclusivo do canal.|
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
- [Resposta de exemplo para uma mensagem de evento sobre um canal definido como favorito por padrão](/graph/system-messages/#channel-set-as-favorite-by-default)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).