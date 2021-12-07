---
title: Tipo de recurso channelDescriptionUpdatedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre uma descrição do canal atualizada.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7abd2a067d89a6c648d0d73e3060a3e4d91d5e9c
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322307"
---
# <a name="channeldescriptionupdatedeventmessagedetail-resource-type"></a>Tipo de recurso channelDescriptionUpdatedEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre uma descrição [do canal](../resources/channel.md) atualizada.
Essa mensagem é gerada quando a **descrição de um** canal é atualizada.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|channelDescription|String|A descrição atualizada do **canal**.|
|channelId|String|Identificador exclusivo do **canal**.|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelDescriptionUpdatedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelDescriptionUpdatedEventMessageDetail",
  "channelId": "String",
  "channelDescription": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre uma descrição **de canal atualizada**](/graph/system-messages/#channel-description-updated)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
