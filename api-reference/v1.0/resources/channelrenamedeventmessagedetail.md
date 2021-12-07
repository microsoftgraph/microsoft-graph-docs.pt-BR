---
title: Tipo de recurso channelRenamedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre um canal renomeado.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e6f0b2ac19c9f51bbc0cc222bf81470509a2a265
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322315"
---
# <a name="channelrenamedeventmessagedetail-resource-type"></a>Tipo de recurso channelRenamedEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre um canal [renomeado](../resources/channel.md).
Essa mensagem é gerada quando **o nome de um** canal é atualizado.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|channelDisplayName|String|O nome atualizado do **canal**.|
|channelId|String|Identificador exclusivo do **canal**.|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelRenamedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelRenamedEventMessageDetail",
  "channelId": "String",
  "channelDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre um canal **renomeado**](/graph/system-messages/#channel-renamed)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
