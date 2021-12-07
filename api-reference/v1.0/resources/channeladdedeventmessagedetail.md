---
title: Tipo de recurso channelAddedEventMessageDetail
description: Representa os detalhes de uma mensagem de evento sobre um canal adicionado a uma equipe.
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2a93e6f24992d361f92eb0831f8334a225fc95bf
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322319"
---
# <a name="channeladdedeventmessagedetail-resource-type"></a>Tipo de recurso channelAddedEventMessageDetail

Namespace: microsoft.graph

Representa os detalhes de uma mensagem de evento sobre um [canal](../resources/channel.md) adicionado a uma [equipe](../resources/team.md).
Essa mensagem é gerada quando um canal **padrão** é adicionado a uma **equipe**.


Herda de [eventMessageDetail](../resources/eventmessagedetail.md).

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|channelDisplayName|String|Nome de exibição do **canal**.|
|channelId|String|Identificador exclusivo do **canal**.|
|Iniciador|[identitySet](../resources/identityset.md)|Iniciador do evento.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.channelAddedEventMessageDetail",
  "baseType": "microsoft.graph.eventMessageDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.channelAddedEventMessageDetail",
  "channelId": "String",
  "channelDisplayName": "String",
  "initiator": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


## <a name="see-also"></a>Confira também
- [Resposta de exemplo para uma mensagem de evento sobre **um canal** adicionado a uma **equipe**](/graph/system-messages/#channel-added)
- Para obter mais informações sobre outros tipos de eventos, consulte [System messages](/graph/system-messages).
